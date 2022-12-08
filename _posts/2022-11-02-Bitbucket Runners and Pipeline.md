---
layout: post
title: Bitbucket Runners i Pipeline
subtitle: Działanie od strony Dockera
cover-img: /assets/img/bitbucket_1.png
thumbnail-img: /assets/img/bitbucket_1.png
share-img: /assets/img/bitbucket.png
tags: [Bitbucket, Runners, Pipeline]
---

**Runners**
Program Runners umożliwia uruchamianie kompilacji w Pipelines we własnej infrastrukturze i nie zostanie naliczona opłata za minuty kompilacji wykorzystane przez samodzielnie hostowanych runnerów. Poniższe przewodniki pomagają skonfigurować system operacyjny za pomocą Pipelines, aby używać modułów uruchamiających w repozytoriach.

**Obsługiwane platformy**
1. Linux z architekturą x64 i jądrem Linux 4.0.0+. Runery zostały przetestowane na następujących dystrybucjach Linuksa:
2. Windows 10+ lub Windows Server 2019+
3. MacOS Catalina 10.15+

**Minimalne wymagania**

Doker Linuksa:
1. 64-bitowa instancja Linux z co najmniej 8 GB pamięci RAM jako hostem dla runnera.
2. Docker v19.03 i nowsze


Bitbucket Pipelines umożliwia tworzenie obrazu platformy Docker z pliku Docker w repozytorium i wypychanie go do rejestru platformy Docker przez  uruchamianie poleceń platformy Docker  w potoku kompilacji. Zanurz się prosto – środowisko potoku jest dostarczane domyślnie i nie musisz go dostosowywać!

**Włączenie dostepu do Dockerza**
Aby umożliwić dostęp do demona Docker, można dodać dockera jako usługę w kroku lub dodać opcję globalną w pliku bitbucket-pipelines.yml.


**Żeby skonfigurować Bitbucket Runners komendami ze strony Docker Linux należy:**
**Pierwszy ze sposobów:**
1. Wyłączyć swap w środowisku Linux

Poniżej znajdują się kroki, aby wyłączyć swap dla większości dystrybucji Linuksa . Jeśli poniższe polecenia nie są zainstalowane, będziesz musiał je zainstalować. Zapoznaj się z dokumentacją dystrybucji, aby skonfigurować swap.

{% highlight javascript linenos %}
sudo swapon -sv
{% endhighlight %}

Jeśli zamiana jest włączona, powinieneś zobaczyć dane wyjściowe podobne do następujących:
{% highlight javascript linenos %}
NAME      TYPE      SIZE   USED PRIO
/dev/sda3 partition   2G 655.2M   -1
{% endhighlight %}

2. Jeśli zamiana jest włączona, będziesz musiał ją wyłączyć

3. Skonfiguruj vm.swappiness w środowisku Linux

Poniżej znajdują się kroki, aby skonfigurować vm.swappiness dla większości dystrybucji Linuksa . Jeśli poniższe polecenia nie są zainstalowane, będziesz musiał je zainstalować. Zapoznaj się z dokumentacją dystrybucji, aby skonfigurować swap.

Użyj następującego polecenia, aby sprawdzić wartość vm.swappiness:

{% highlight javascript linenos %}
sudo sysctl -n vm.swappiness
{% endhighlight %}

Jeśli wartość swappiness jest inna niż 1 , skonfiguruj ją za pomocą następującego procesu:
Uruchom następujące polecenie, upewniając się, że dane wyjściowe są teraz 1:

{% highlight javascript linenos %}
sudo sysctl -n vm.swappiness
{% endhighlight %}

**Drugi ze sposobów:**
Ten sposób jest o wiele prostszy. Polega on na tym, że Bitbucket Runners wydaje polecenie, które trzeba po prostu uruchomić w konsoli Linux. Polecenie wygladą nastepująco:
# Copy this command with the token to run on the command line
{% highlight javascript linenos %}
docker container run -it -v /tmp:/tmp -v /var/run/docker.sock:/var/run/docker.sock -v /var/lib/docker/containers:/var/lib/docker/containers:ro -e ACCOUNT_UUID={c09fffc4-c0e4-4c0d-bd98-ef23d2aa6dca} -e REPOSITORY_UUID={49ca6428-767f-4f57-95ec-84cb0fd05c08} -e RUNNER_UUID={4b3b8bf3-c323-536f-b2ba-797e0aa721b9} -e RUNTIME_PREREQUISITES_ENABLED=true -e OAUTH_CLIENT_ID=sLwWKhotz990WnKjNhNK1ouD5HKKkA9I -e OAUTH_CLIENT_SECRET=8MEOpdDBBFpwENUr518EcEUJWHZFiIh3miEu1OzmZ2AyWMSkB0wCrpdbA9ElfpxC -e WORKING_DIRECTORY=/tmp --name runner-4b3b8bf3-c323-536f-b2ba-797e0aa721b9 docker-public.packages.atlassian.com/sox/atlassian/bitbucket-pipelines-runner:1
{% endhighlight %}


Po czym konfiguracja pliku bitbucket-pipelines.yml tworzy się samodzielnie:
{% highlight javascript linenos %}
pipelines:
  default:
      - step:
          runs-on:
            - self.hosted
            - linux
          script:
{% endhighlight %}

{% highlight javascript linenos %}
**Notatka**
Jeśli nie określisz etykiety linux.shell, nasz program planujący przyjmie, że jest to krok Linux Docker i spróbuje uruchomić go jako Linux Docker Runner.

Jeśli wszystkie pasujące Linux Shell Runners są zajęte, Twój krok zostanie umieszczony w kolejce, dopóki jeden nie stanie się ponownie dostępny.

Jeśli nie masz w swoim repozytorium żadnych biegaczy online, które pasują do wszystkich Twoich etykiet, krok się nie powiedzie.
{% endhighlight %}

### **Jak stworzyć Runner?**

### **Utwórz nowy Workspace Runner w Bitbucket**

**Przejdź do ustawień obszaru roboczego**

Kliknij swoje zdjęcie profilowe i wybierz obszar roboczy

![Photo](https://itgcommerce.com/wp-content/uploads/2021/09/1-workspace-settings-1536x824.jpg)

Kliknij Ustawienia i przewiń w dół do Workspace Runners i kliknij Dodaj Runnera:

![Photo](https://itgcommerce.com/wp-content/uploads/2021/09/2-workspace-runners-1536x837.jpg)

Nadaj swojemu biegaczowi imię i kliknij Dalej.

![Photo](https://itgcommerce.com/wp-content/uploads/2021/09/3-new-runner.jpg)

To da ci wynik polecenia taki:

{% highlight javascript linenos %}
docker container run -it -v /tmp:/tmp -v /var/run/docker.sock:/var/run/docker.sock \
  -v /var/lib/docker/containers:/var/lib/docker/containers:ro \
  -e ACCOUNT_UUID={__ACCOUNT_UUID__} \
  -e RUNNER_UUID={__RUNNER_UUID__} \
  -e OAUTH_CLIENT_ID=__OAUTH_CLIENT_ID__ \
  -e OAUTH_CLIENT_SECRET=__OAUTH_CLIENT_SECRET__ \
  -e WORKING_DIRECTORY=/tmp \
  --name runner-7deb7740-f86b-50d0-9c85-671fcb3c9038 \
  docker-public.packages.atlassian.com/sox/atlassian/bitbucket-pipelines-runner:1
{% endhighlight %}

**Zapisz go** i kliknij Zakończ.

Musisz wyodrębnić zmienne ACCOUNT_UUID, RUNNER_UUID, OAUTH_CLIENT_ID i OAUTH_CLIENT_SECRET z polecenia.

Uważaj na następujące rzeczy:

- Skopiuj ACCOUNT_UUID i RUNNER_UUID bez nawiasów klamrowych.
- Pamiętaj, aby skopiować cały OAUTH_CLIENT_SECRET (może zawierać znaki specjalne, takie jak myślniki lub podkreślenia).
- Zmienne OAUTH muszą zostać przekonwertowane na base64.

Możesz wypełnić następujący skrypt, a później wygenerować zasoby k8s za pomocą tych zmiennych:

{% highlight javascript linenos %}
export ACCOUNT_UUID=__ACCOUNT_UUID__
export RUNNER_UUID=__RUNNER_UUID__
export OAUTH_CLIENT_ID=__OAUTH_CLIENT_ID__
export OAUTH_CLIENT_SECRET=__OAUTH_CLIENT_SECRET__

export BASE64_OAUTH_CLIENT_ID=$(echo -n $OAUTH_CLIENT_ID | base64)
export BASE64_OAUTH_CLIENT_SECRET=$(echo -n $OAUTH_CLIENT_SECRET | base64)
{% endhighlight %}

### **Wdrożenie w Kubernetes**
Teraz interesująca część. Zastąp symbole zastępcze ${VAR_NAME} zawartością tych zmiennych.

Ważne:

- użyj zakodowanych w base64 wersji zmiennych OAUTH w pliku secret.yaml
- zachowaj cudzysłowy i nawiasy klamrowe („, {, }”) w liniach job.yaml 17 i 19

Następujące skrypty bash wygenerują pliki secret.yaml i job.yaml w bieżącym katalogu roboczym.

secret.yaml:

{% highlight javascript linenos %}
cat > ./secret.yaml <<EOF
apiVersion: v1
kind: Secret
metadata:
  name: runner-oauth-credentials
  labels:
    accountUuid: ${ACCOUNT_UUID}
    runnerUuid: ${RUNNER_UUID}
data:
  oauthClientId: ${BASE64_OAUTH_CLIENT_ID}
  oauthClientSecret: ${BASE64_OAUTH_CLIENT_SECRET}
EOF
{% endhighlight %}

job.yaml:

{% highlight javascript linenos %}
cat > ./job.yaml <<EOF
apiVersion: batch/v1
kind: Job
metadata:
  name: runner
spec:
  template:
    metadata:
      labels:
        accountUuid: ${ACCOUNT_UUID}
        runnerUuid: ${RUNNER_UUID}
    spec:
      containers:
        - name: bitbucket-k8s-runner
          image: docker-public.packages.atlassian.com/sox/atlassian/bitbucket-pipelines-runner
          env:
            - name: ACCOUNT_UUID
              value: "{${ACCOUNT_UUID}}"
            - name: RUNNER_UUID
              value: "{${RUNNER_UUID}}"
            - name: OAUTH_CLIENT_ID
              valueFrom:
                secretKeyRef:
                  name: runner-oauth-credentials
                  key: oauthClientId
            - name: OAUTH_CLIENT_SECRET
              valueFrom:
                secretKeyRef:
                  name: runner-oauth-credentials
                  key: oauthClientSecret
            - name: WORKING_DIRECTORY
              value: "/tmp"
          volumeMounts:
            - name: tmp
              mountPath: /tmp
            - name: docker-containers
              mountPath: /var/lib/docker/containers
              readOnly: true
            - name: var-run
              mountPath: /var/run
        - name: docker-in-docker
          image: docker:20.10.7-dind
          securityContext:
            privileged: true
          volumeMounts:
            - name: tmp
              mountPath: /tmp
            - name: docker-containers
              mountPath: /var/lib/docker/containers
            - name: var-run
              mountPath: /var/run
      restartPolicy: OnFailure
      volumes:
        - name: tmp
        - name: docker-containers
        - name: var-run
  backoffLimit: 6
  completions: 1
  parallelism: 1
EOF
{% endhighlight %}job.yaml:

{% highlight javascript linenos %}
cat > ./job.yaml <<EOF
apiVersion: batch/v1
kind: Job
metadata:
  name: runner
spec:
  template:
    metadata:
      labels:
        accountUuid: ${ACCOUNT_UUID}
        runnerUuid: ${RUNNER_UUID}
    spec:
      containers:
        - name: bitbucket-k8s-runner
          image: docker-public.packages.atlassian.com/sox/atlassian/bitbucket-pipelines-runner
          env:
            - name: ACCOUNT_UUID
              value: "{${ACCOUNT_UUID}}"
            - name: RUNNER_UUID
              value: "{${RUNNER_UUID}}"
            - name: OAUTH_CLIENT_ID
              valueFrom:
                secretKeyRef:
                  name: runner-oauth-credentials
                  key: oauthClientId
            - name: OAUTH_CLIENT_SECRET
              valueFrom:
                secretKeyRef:
                  name: runner-oauth-credentials
                  key: oauthClientSecret
            - name: WORKING_DIRECTORY
              value: "/tmp"
          volumeMounts:
            - name: tmp
              mountPath: /tmp
            - name: docker-containers
              mountPath: /var/lib/docker/containers
              readOnly: true
            - name: var-run
              mountPath: /var/run
        - name: docker-in-docker
          image: docker:20.10.7-dind
          securityContext:
            privileged: true
          volumeMounts:
            - name: tmp
              mountPath: /tmp
            - name: docker-containers
              mountPath: /var/lib/docker/containers
            - name: var-run
              mountPath: /var/run
      restartPolicy: OnFailure
      volumes:
        - name: tmp
        - name: docker-containers
        - name: var-run
  backoffLimit: 6
  completions: 1
  parallelism: 1
EOF
{% endhighlight %}


Zastosuj wygenerowane manifesty do Kubernetes:

{% highlight javascript linenos %}
kubectl create namespace bitbucket-runner --dry-run -o yaml | kubectl apply -f -
kubectl -n bitbucket-runner apply -f secrets.yaml
kubectl -n bitbucket-runner apply -f job.yaml
{% endhighlight %}

Jeśli wszystko poszło dobrze, wkrótce zobaczysz biegacza ze statusem ONLINE na stronie Workspace Runners.

![Photo](https://itgcommerce.com/wp-content/uploads/2021/09/4-registered-runner-1536x840.jpg)

Jeśli zdecydujesz się usunąć biegacza z Kubernetes, wykonaj następujące kroki:

{% highlight javascript linenos %}
kubectl -n bitbucket-runner delete -f job.yaml            
kubectl -n bitbucket-runner delete -f secret.yaml 
kubectl delete namespace bitbucket-runner
{% endhighlight %}

## **Jak używać tego runnera w potoku Bitbucket?**
To całkiem proste, dodaj etykiety runnera do etapu potoku.

{% highlight javascript linenos %}
pipelines:
  custom:
    pipeline:
      - step:
          name: Step1
          size: 8x # default 4gb, 8x for 32gb
          runs-on: 
            - 'self.hosted'
            - 'my.custom.label'
          script:
            - echo "This step will run on a self hosted runner with 32 GB of memory.";
      - step:
          name: Step2
          script:
            - echo "This step will run on Atlassian's infrastructure as usual.";
{% endhighlight %}


## **Błąd: status 500 w potokach Bitbucket**
Ponieważ chcieliśmy zbudować obrazy Dockera (za pomocą Dockera w Dockerze lub dind) w naszym potoku, napotkaliśmy następujący problem:

{% highlight javascript linenos %}
Status 500: {"message":"io.containerd.runc.v2: failed to adjust OOM score for shim: set shim OOM score: write /proc/PROC_ID/oom_score_adj: invalid argument\n: exit status 1: unknown"}
{% endhighlight %}


### **Jak to naprawić**
Najpierw próbowałem znaleźć główną przyczynę tego komunikatu o błędzie, ale nie mogłem znaleźć niczego poza kilkoma komentarzami na ten temat, które zostały już naprawione w ostatnim wydaniu containerd, i tak dalej… Postanowiłem więc sprawdzić, czy wersje oprogramowania się zgadzają. Nawet gdy containerd pasował do wymaganej wersji, stwierdziłem, że Docker na serwerach jest nieco przestarzały (19.03), więc postanowiłem go zaktualizować.

Po aktualizacji nadal widziałem wcześniej wspomniane komunikaty o błędach w potokach Bitbucket.

Zweryfikowałem wersję Dockera uruchomioną na serwerze:

{% highlight javascript linenos %}
# docker --version    
Docker version 20.10.7, build f0df350   
{% endhighlight %}


Wymieniłem docker w wersji obrazu kontenera docker (dind), aby używał dokładnie tej samej wersji, co zainstalowana w naszym klastrze k8s!

{% highlight javascript linenos %}
- name: docker-in-docker
  image: docker:20.10.5-dind  ->  docker:20.10.7-dind
{% endhighlight %}

I magicznie błąd zniknął i wszystko działa zgodnie z oczekiwaniami.

