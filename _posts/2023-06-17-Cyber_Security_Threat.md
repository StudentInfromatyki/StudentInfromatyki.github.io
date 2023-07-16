---
layout: post
title: Książka
subtitle: Cyber Security Threat
author: Oleh Danchivskyi
cover-img: /assets/img/Cyber/Logo-1.jpg
thumbnail-img: /assets/img/Cyber/Logo.png
share-img: /assets/img/Cyber/Logo-1.jpg
tags: [Cyberbezpieczeństwo, Bezpieczeńswto, Ataki, Metody]
---


# 1. Wprowadzenie

Dzisiejszy świat sprawia, że wszyscy są bardziej podatni na cyberataki. Niezależnie od tego, czy interesuje nas relatywnie nowy świat cyberbezpieczeństwa jako profesjonalista, czy po prostu interesuje nas ochrona w Internecie i mediach społecznościowych.

## 1.1. Podstawowe terminy i definicje

#### Poniżej przedstawiono podstawowe terminy i definicje:
+ Uwierzytelnianie (ang. Authentication) – proces identyfikacji tożsamości użytkownika, upewniając się, że może on mieć dostęp do systemu i/lub plików.
+ Botnet (and. Botnet) – połączenie słów „robot” i „sieć”, botnet to sieć komputerów, które zostały zainfekowane wirusem i teraz nieprzerwanie pracują w celu stworzenia luk w zabezpieczeniach. Ataki te mają formę wydobywania bitcoinów, wysyłania spamu i ataków DDoS.
+ Domena (ang. Domain) – szereg komputerów i powiązanych z nimi urządzeń peryferyjnych (routerów, drukarek, skanerów), które są połączone jako jedna całość.
+ Szyfrowanie (ang. Encryption) – kodowanie używane do ochrony informacji przed hakerami. Pomyśl o tym jak o szyfrze używanym do wysyłania ściśle tajnej zaszyfrowanej wiadomości szpiegowskiej.
+ Firewall – każda technologia, czy to oprogramowanie, czy sprzęt, używana do powstrzymywania intruzów.
+ Haker, Czarny Kapelusz (ang. Black Hat) – każdy haker, który próbuje uzyskać nieautoryzowany dostęp do systemu z zamiarem wyrządzenia szkody, zniszczenia lub kradzieży. Mogą być motywowane chciwością, agendą polityczną lub po prostu nudą.
+ Haker, Biały Kapelusz (ang. White Hat) – haker zapraszany do testowania systemów komputerowych i serwerów w poszukiwaniu luk w celu poinformowania hosta, gdzie należy poprawić zabezpieczenia.
+ Złośliwe oprogramowanie (ang. Malware) – połączenie słów „złośliwe” i „oprogramowanie”, opisujące szeroką gamę złego oprogramowania używanego do infekowania i/lub uszkadzania systemu. Ransomware, robaki, wirusy i trojany są uważane za złośliwe oprogramowanie. Najczęściej dostarczany za pośrednictwem wiadomości e-mail ze spamem.
+ Koń trojański (ang. Trojan Horse) – jeszcze jedna forma złośliwego oprogramowania, tym razem wprowadzający w błąd program komputerowy, który wygląda niewinnie, ale w rzeczywistości pozwala hakerowi dostać się do twojego systemu przez tylne drzwi, umożliwiając mu kontrolowanie twojego komputera.
+ Wirus (and. Virus) – złośliwe oprogramowanie, które zmienia, uszkadza lub niszczy informacje, a następnie jest przekazywane do innych systemów, zwykle w inny sposób nieszkodliwy (np. wysyłanie wiadomości e-mail).
+ Robak (ang. Worm) – złośliwe oprogramowanie, które może się powielać w celu rozprzestrzeniania się na inne komputery w sieci. Szczególnie paskudne robaki mogą być po prostu sposobem na spowolnienie systemu poprzez pochłanianie zasobów lub popełnianie exploitów, takich jak instalowanie tylnych drzwi lub kradzież danych.
+ Inżynieria społeczna (ang. Social Engineering) – ta strategia opiera się na manipulacji użytkownikami i psychologii człowieka. Pracownik może otrzymać wiadomość e-mail od socjotechnika, który rzekomo pracuje w dziale IT, aby skłonić go do ujawnienia prywatnych informacji zamiast próby wykrycia słabości oprogramowania w systemie firmowym.
+ Etyczne hakowanie (ang. Ethical Hacking) – za zgodą właściciela włamuje się do sieci w celu uzyskania poufnych informacji – całkowicie legalnie. Zazwyczaj ta technika jest używana do sprawdzania słabych punktów infrastruktury.
+ Cyber ataki (ang. Cyber Attack) – każda próba naruszenia granicy bezpieczeństwa środowiska logicznego. Atak może koncentrować się na zbieraniu danych wywiadowczych, zakłócaniu działalności firmy, wykorzystywaniu słabych punktów, śledzeniu celów, przerywaniu pracy, uzyskiwaniu wartości, szkodzeniu zasobom logicznym lub fizycznym lub wykorzystywaniu zasobów systemowych w celu umożliwienia ataków na inne cele.


## 1.2. Logi systemowe

Logi systemowe – to są zdarzenie, które miało miejsce w określonym czasie i może zawierać metadane, które nadają mu kontekst. Innymi słowami logi to są zapisy wszystkiego co się dzieje w systemie, w tym zdarzeń takich jak transakcje, błędy i włamania. Dane te mogą być przesyłane na różne sposoby i mogą być w formacie ustrukturyzowanym, częściowo ustrukturyzowanym i nieustrukturyzowanym. 

<p align="center">
  Rys.1.2.1. Wygląd logów systemowych
<br>
  <img src="\assets\img\Cyber\1.png" width="650" alt="logi">
  <br>
  Źródło: https://tiny.pl/c71cb
</p>

#### Podstawowa struktura logów: 
+ Sygnatura czasowa (ang. The timestamp) – dokładny czas wystąpienia zarejestrowanego zdarzenia. 
+ Informacje o użytkowniku (ang. User Information)
+ Informacje o zdarzeniu (ang. Event Information) – jaka została podjęta akcja.

#### Skąd pochodzą logi?
Prawie wszystko tworzy jakąś wersję logów, np.: 
•	Aplikacje
•	Kontenery
•	Bazy danych 
•	Zapory ogniowe 
•	Punkty końcowe 
•	Urządzenia IoT
•	Sieci
•	Serwery
•	Usługi internetowe


<p align="center">
  Rys.1.2.2. Rodzaje logów
<br>
  <img src="\assets\img\Cyber\2.png" width="650" alt="logi-1">
  <br>
  Źródło: https://www.crowdstrike.com/wp-content/uploads/2022/09/logfilesources-768x713.webp
</p>

#### Rodzaje dzienników:
+ Każdy komponent generuje inny typ danych i każdy komponent gromadzi te dane we własnych zapisach logów. Istnieje wiele rodzajów dzienników, np.:
+ Dziennik zdarzeń : dziennik wysokiego poziomu, w którym rejestrowane są informacje o ruchu sieciowym i użytkowaniu, takie jak próby logowania, nieudane próby podania hasła i zdarzenia aplikacji.
+ Dziennik serwera : dokument tekstowy zawierający zapis działań związanych z określonym serwerem w określonym przedziale czasu.
+ Dziennik systemowy (syslog) : zapis zdarzeń systemu operacyjnego. Obejmuje komunikaty startowe, zmiany systemowe, nieoczekiwane zamknięcia, błędy i ostrzeżenia oraz inne ważne procesy. Systemy Windows, Linux i macOS generują dzienniki systemowe.
+ Dzienniki autoryzacji i dzienniki dostępu : zawierają listę osób lub botów uzyskujących dostęp do określonych aplikacji lub plików.
+ Dzienniki zmian : zawierają chronologiczną listę zmian wprowadzonych w aplikacji lub pliku.
+ Dzienniki dostępności : śledź wydajność, czas pracy i dostępność systemu.
+ Dzienniki zasobów : dostarczają informacji o problemach z łącznością i ograniczeniach pojemności.
+ Dzienniki zagrożeń : zawierają informacje o ruchu w systemie, plikach lub aplikacjach, które pasują do predefiniowanego profilu zabezpieczeń w zaporze.


### Jak to działa dokładnie?

#### Proces generowania logów zazwyczaj obejmuje następujące kroki:
+ Zdarzenie: W pewnym momencie występuje zdarzenie, które jest wartościowe do zarejestrowania w logach. Może to być na przykład inicjalizacja systemu, żądanie użytkownika, błąd, informacja diagnostyczna itp.
+ Logowanie: Gdy zdarzenie wystąpi, aplikacja lub komponent odpowiedzialny za logowanie zapisuje informacje na temat zdarzenia w logach. Informacje te mogą zawierać czas zdarzenia, identyfikator zdarzenia, priorytet, opis zdarzenia, informacje diagnostyczne itp.
+ Składowanie: Zapisane logi są przechowywane w określonym miejscu, takim jak pliki na dysku, baza danych lub system logów. Mogą być również przesyłane do zdalnych serwerów logów w przypadku rozproszonych systemów.
+ Analiza i monitorowanie: Administratorzy systemów i programiści mogą przeglądać, analizować i monitorować zapisane logi. Mogą korzystać z różnych narzędzi do przeszukiwania i filtrowania logów w celu znalezienia informacji potrzebnych do rozwiązywania problemów lub monitorowania działania systemu.

#### Przykładem logu może być następujący wpis:
~~~
2023-06-08 10:30:15 [INFO] Aplikacja została pomyślnie uruchomiona.
~~~

W powyższym przykładzie mamy informację o czasie zdarzenia (10:30:15, 8 czerwca 2023 roku), priorytecie logu (INFO) oraz opisie zdarzenia (Aplikacja została pomyślnie uruchomiona). Ten wpis może być przydatny podczas monitorowania systemu, aby potwierdzić, że aplikacja została poprawnie uruchomiona o określonym czasie.

Logi mogą być bardziej rozbudowane i zawierać dodatkowe informacje, takie jak identyfikatory sesji, informacje o żądaniach użytkownika, ślad stosu błędu, szczegółowe informacje diagnostyczne itp. Wszystko zależy od potrzeb i konfiguracji systemu logowania.


## 2. Ataki modelu ISO/OSI

Ataki mogą miec miejsce na różnych poziomach modeli sieci z różnymi protokołami. Poniżej przedstawiam ataki z każdej warstwy. 

<p align="center">
  Rys.2.1. Ataki na różne warstwy modelu OSI
<br>
  <img src="\assets\img\Cyber\3.png" width="650" alt="iso/osi">
  <br>
  Źródło: https://miro.medium.com/v2/resize:fit:720/format:webp/1*eWE2QWWS6jS9o3EqTibncw.png
</p>


## 2.1. Ataki na warstwie aplikacji

Osoba atakująca może zaatakować aplikację za pomocą ataku warstwy 7 lub warstwy aplikacji. W tych atakach, podobnie jak w przypadku ataków na infrastrukturę SYN flood, osoba atakująca próbuje przeciążyć określone funkcje aplikacji, aby uniemożliwić dostęp do aplikacji lub uniemożliwić jej reagowanie dla uprawnionych użytkowników. Poniżej przedstawiam listę ataków wraz z wyjaśnieniem i przykładami.


### 2.1.1. XSS 

Cross-site scripting (znany również jako XSS) to luka w zabezpieczeniach internetowych, która umożliwia atakującemu naruszenie interakcji użytkowników z podatną aplikacją. Umożliwia atakującemu obejście tej samej zasady pochodzenia, która ma na celu oddzielenie różnych witryn internetowych od siebie. Luki w zabezpieczeniach związane z atakami typu cross-site scripting zwykle umożliwiają atakującemu podszywanie się pod użytkownika będącego ofiarą, wykonywanie wszelkich czynności, które użytkownik jest w stanie wykonać, oraz uzyskiwanie dostępu do dowolnych danych użytkownika. Jeśli użytkownik będący ofiarą ma uprzywilejowany dostęp do aplikacji, osoba atakująca może uzyskać pełną kontrolę nad wszystkimi funkcjami i danymi aplikacji.

#### Jak działa XSS?

Cross-site scripting polega na manipulowaniu podatną na ataki witryną internetową, tak aby zwracała użytkownikom szkodliwy kod JavaScript. Kiedy złośliwy kod jest wykonywany w przeglądarce ofiary, atakujący może całkowicie zagrozić swojej interakcji z aplikacją.


<p align="center">
  Rys.2.1.1.1. Działanie XSS
<br>
  <img src="\assets\img\Cyber\4.png" width="650" alt="xss">
  <br>
  Źródło: https://portswigger.net/web-security/images/cross-site-scripting.svg
</p>


### Rodzaje ataków XSS:
+ Odzwierciedlający XSS – złośliwy skrypt pochodzi z bieżącego żądania http

##### Oto prosty przykład odzwierciedlonej luki w zabezpieczeniach XSS:
~~~
https://insecure-website.com/status?message=All+is+well.
<p>Status: All is well.</p>
~~~

Aplikacja nie wykonuje żadnego innego przetwarzania danych, więc osoba atakująca może łatwo skonstruować taki atak:

~~~
https://insecure-website.com/status?message=<script>/*+Bad+stuff+here...+*/</script>

<p>Status: <script>/* Bad stuff here...*/</script></p>
~~~

<br>

+ Zapisany XSS – złośliwy skrypt pochodzi z bazy danych serwisu

Oto prosty przykład zapisanej luki XSS. Aplikacja tablicy ogłoszeń umożliwia użytkownikom przesyłanie wiadomości, które są wyświetlane innym użytkownikom:

~~~
<𝑝>𝐻𝑒𝑙𝑙𝑜,𝑡ℎ𝑖𝑠 𝑖𝑠 𝑚𝑦 𝑚𝑒𝑠𝑠𝑎𝑔𝑒!</𝑝>
~~~

Aplikacja nie wykonuje żadnego innego przetwarzania danych, więc osoba atakująca może łatwo wysłać wiadomość, która atakuje innych użytkowników:
~~~
<𝑝><𝑠𝑐𝑟𝑖𝑝𝑡>/∗ 𝐵𝑎𝑑 𝑠𝑡𝑢𝑓𝑓 ℎ𝑒𝑟𝑒...∗/</𝑠𝑐𝑟𝑖𝑝𝑡></𝑝>
~~~

<br>

+ XSS oparty na DOM – luka występuje w kodzie po stronie klienta, a nie w kodzie po stronie serwera

W poniższym przykładzie aplikacja używa kodu JavaScript do odczytania wartości z pola wejściowego i zapisania tej wartości do elementu w kodzie HTML:
~~~
var search = document.getElementById('search').value;

var results = document.getElementById('results');

results.innerHTML = 'You searched for: ' + search;
~~~

Jeśli atakujący może kontrolować wartość pola wejściowego, może łatwo skonstruować złośliwą wartość, która spowoduje wykonanie własnego skryptu:
~~~
You searched for: <img src=1 onerror='/* Bad stuff here...*/'>
~~~



## 2.1.2. SQL Injection

Wstrzyknięcie SQL (SQLi) to luka w zabezpieczeniach sieci Web, która umożliwia atakującemu ingerowanie w zapytania kierowane przez aplikację do jej bazy danych. W niektórych sytuacjach osoba atakująca może eskalować atak polegający na wstrzykiwaniu kodu SQL w celu skompromitowania bazowego serwera lub innej infrastruktury zaplecza lub przeprowadzić atak typu „odmowa usługi”.


<p align="center">
  Rys.2.1.2.1. Działanie SQL Injection
<br>
  <img src="\assets\img\Cyber\5.png" width="650" alt="sqli">
  <br>
  Źródło: https://portswigger.net/web-security/images/sql-injection.svg
</p>


Udany atak SQL injection może spowodować nieautoryzowany dostęp do poufnych danych, takich jak hasła, dane karty kredytowej lub dane osobowe użytkownika.

#### Jak wykryć luki w zabezpieczeniach SQL Injection?

Większość luk w zabezpieczeniach typu SQL injection można znaleźć szybko i niezawodnie za pomocą internetowego skanera luk w zabezpieczeniach pakietu Burp Suite.

Wstrzyknięcie SQL można wykryć ręcznie, stosując systematyczny zestaw testów dla każdego punktu wejścia w aplikacji. Zwykle obejmuje to:
+ Przesyłanie znaku pojedynczego cudzysłowu 'i szukanie błędów lub innych anomalii.
+ Przesyłanie pewnej składni specyficznej dla języka SQL, która ocenia wartość podstawową (oryginalną) punktu wejścia i inną wartość, oraz szukanie systematycznych różnic w wynikowych odpowiedziach aplikacji.
+ Przesyłanie warunków boolowskich, takich jak OR 1=1i OR 1=2, oraz szukanie różnic w odpowiedziach aplikacji.
+ Przesyłanie ładunków zaprojektowanych w celu wywołania opóźnień czasowych podczas wykonywania w zapytaniu SQL i szukanie różnic w czasie potrzebnym na odpowiedź.
+ Przesyłanie ładunków OAST zaprojektowanych do wyzwalania interakcji sieciowej poza pasmem, gdy jest wykonywane w ramach zapytania SQL, oraz monitorowanie wszelkich wynikających z tego interakcji.

#### Wstrzyknięcie SQL drugiego rzędu:

Iniekcja SQL pierwszego rzędu ma miejsce, gdy aplikacja pobiera dane wejściowe użytkownika z żądania HTTP i w trakcie przetwarzania tego żądania włącza dane wejściowe do zapytania SQL w niebezpieczny sposób.

W przypadku iniekcji SQL drugiego rzędu (znanej również jako iniekcja zapisanego SQL) aplikacja pobiera dane wejściowe użytkownika z żądania HTTP i przechowuje je do wykorzystania w przyszłości. Zwykle odbywa się to poprzez umieszczenie danych wejściowych w bazie danych, ale nie powstaje żadna luka w punkcie, w którym dane są przechowywane. Później, podczas obsługi innego żądania HTTP, aplikacja pobiera zapisane dane i włącza je do zapytania SQL w niebezpieczny sposób.


<p align="center">
  Rys.2.1.2.2. Wstrzyknięcie SQL Injection drugiego rzędu
<br>
  <img src="\assets\img\Cyber\6.png" width="650" alt="sqli-1">
  <br>
  Źródło: https://portswigger.net/web-security/images/second-order-sql-injection.svg
</p>

Wstrzykiwanie SQL drugiego rzędu często pojawia się w sytuacjach, gdy programiści są świadomi luk w zabezpieczeniach wstrzykiwania SQL, więc bezpiecznie obsługują początkowe umieszczanie danych wejściowych w bazie danych. Gdy dane są później przetwarzane, uważa się je za bezpieczne, ponieważ zostały wcześniej bezpiecznie umieszczone w bazie danych. W tym momencie dane są traktowane w niebezpieczny sposób, ponieważ programista błędnie uznaje je za zaufane.

#### Jak zapobiegać SQL Injection?

Większości przypadków iniekcji SQL można zapobiec, używając sparametryzowanych zapytań (znanych również jako przygotowane instrukcje) zamiast konkatenacji ciągów w zapytaniu.

Poniższy kod jest podatny na wstrzyknięcie kodu SQL, ponieważ dane wejściowe użytkownika są bezpośrednio łączone z zapytaniem:

~~~
String query = "SELECT * FROM products WHERE category = '"+ input + "'";

Statement statement = connection.createStatement();

ResultSet resultSet = statement.executeQuery(query);
~~~

Ten kod można łatwo przepisać w sposób, który zapobiega ingerencji użytkownika w strukturę zapytania:
~~~
𝑃𝑟𝑒𝑝𝑎𝑟𝑒𝑑𝑆𝑡𝑎𝑡𝑒𝑚𝑒𝑛𝑡 𝑠𝑡𝑎𝑡𝑒𝑚𝑒𝑛𝑡 = 𝑐𝑜𝑛𝑛𝑒𝑐𝑡𝑖𝑜𝑛.𝑝𝑟𝑒𝑝𝑎𝑟𝑒𝑆𝑡𝑎𝑡𝑒𝑚𝑒𝑛𝑡("𝑆𝐸𝐿𝐸𝐶𝑇 ∗ 

𝐹𝑅𝑂𝑀 𝑝𝑟𝑜𝑑𝑢𝑐𝑡𝑠 𝑊𝐻𝐸𝑅𝐸 𝑐𝑎𝑡𝑒𝑔𝑜𝑟𝑦 = ?");

𝑠𝑡𝑎𝑡𝑒𝑚𝑒𝑛𝑡.𝑠𝑒𝑡𝑆𝑡𝑟𝑖𝑛𝑔(1,𝑖𝑛𝑝𝑢𝑡);

𝑅𝑒𝑠𝑢𝑙𝑡𝑆𝑒𝑡 𝑟𝑒𝑠𝑢𝑙𝑡𝑆𝑒𝑡 = 𝑠𝑡𝑎𝑡𝑒𝑚𝑒𝑛𝑡 𝑒𝑥𝑒𝑐𝑢𝑡𝑒𝑄𝑢𝑒𝑟𝑦();
~~~

Zapytań sparametryzowanych można używać w każdej sytuacji, w której jako dane w zapytaniu pojawiają się niezaufane dane wejściowe, w tym klauzula WHERE i wartości w instrukcji INSERT lub UPDATE. Nie można ich używać do obsługi niezaufanych danych wejściowych w innych częściach zapytania, takich jak nazwy tabel lub kolumn lub klauzula ORDER BY. Funkcjonalność aplikacji, która umieszcza niezaufane dane w tych częściach zapytania, będzie musiała przyjąć inne podejście, takie jak umieszczenie dozwolonych wartości wejściowych na białej liście lub użycie innej logiki w celu zapewnienia wymaganego zachowania.


Aby sparametryzowana kwerenda była skuteczna w zapobieganiu iniekcji SQL, ciąg używany w kwerendzie musi zawsze być stałą zakodowaną na stałe i nigdy nie może zawierać żadnych zmiennych danych z dowolnego źródła. Nie ulegaj pokusie decydowania o tym, czy dany element danych jest zaufany, i kontynuuj stosowanie konkatenacji ciągów w zapytaniu w przypadkach, które są uważane za bezpieczne. Bardzo łatwo jest popełnić błąd co do możliwego pochodzenia danych lub wprowadzić zmiany w innym kodzie, aby naruszyć założenia dotyczące tego, jakie dane są skażone.


### 2.1.3. CSRF

Cross-Site Request Forgery to atak, który zmusza uwierzytelnionych użytkowników do przesłania żądania do aplikacji internetowej, względem której są aktualnie uwierzytelnieni. Ataki CSRF wykorzystują zaufanie aplikacji internetowej do uwierzytelnionego użytkownika. 


<p align="center">
  Rys.2.1.3.1. Działanie CSRF
<br>
  <img src="\assets\img\Cyber\8.png" width="650" alt="CSRF">
  <br>
  Źródło: https://portswigger.net/web-security/images/cross-site%20request%20forgery.svg
</p>

Załóżmy na przykład, że aplikacja zawiera funkcję umożliwiającą użytkownikowi zmianę adresu e-mail na koncie. Gdy użytkownik wykonuje tę czynność, wysyła żądanie HTTP w następujący sposób:

~~~
POST /email/change HTTP/1.1
Host: vulnerable-website.com
Content-Type: application/x-www-form-urlencoded
Content-Length: 30
Cookie: session=yvthwsztyeQkAPzeQ5gHgTvlyxHfsAfE
email=wiener@normal-user.com
~~~

#### Spełnia to warunki wymagane dla CSRF:
+ Akcja zmiany adresu e-mail na koncie użytkownika jest interesująca dla atakującego. Po wykonaniu tej czynności osoba atakująca zazwyczaj będzie w stanie wywołać resetowanie hasła i przejąć pełną kontrolę nad kontem użytkownika.
+ Aplikacja wykorzystuje sesyjny plik cookie do identyfikacji użytkownika, który wysłał żądanie. Nie ma żadnych innych tokenów ani mechanizmów do śledzenia sesji użytkowników.
+ Atakujący może łatwo określić wartości parametrów żądania, które są potrzebne do wykonania akcji.

Po spełnieniu tych warunków osoba atakująca może utworzyć stronę internetową zawierającą następujący kod HTML:

~~~
<html>
    <body>
        <form action="https://vulnerable-website.com/email/change" method="POST">
            <input type="hidden" name="email" value="pwned@evil-user.net" />
        </form>
        <script>
            document.forms[0].submit();
        </script>
    </body>
</html>
~~~

Jeśli użytkownik będący ofiarą odwiedzi stronę internetową atakującego, nastąpią następujące zdarzenia:
+ Strona atakującego wywoła żądanie HTTP do podatnej witryny sieci Web.
+ Jeśli użytkownik jest zalogowany w witrynie podatnej na ataki, jego przeglądarka automatycznie uwzględni w żądaniu plik cookie sesji (zakładając, że pliki cookie Cross-Site nie są używane).
+ Podatna strona internetowa przetworzy żądanie w normalny sposób, potraktuje je jako wysłane przez użytkownika ofiary i zmieni jego adres e-mail.

#### Przykład – bankowość elektroniczna:

Jeszcze jeden często przeczytany przykład wykorzystania CSRF wymagający uwierzytelnienia: 

<p align="center">
  Rys.2.1.3.2. XSRF - bankowość elektroniczna
<br>
  <img src="\assets\img\Cyber\9.png" width="650" alt="csrf-1">
  <br>
  Źródło: https://sekurak.pl/wp-content/uploads/2015/04/csrf-admin3.gif
</p>


#### W tym przypadku:
+ Atakujący umieszcza na stronie eeeevil-zite.com tag *<img>* realizujący request odpowiadający realizacji przelewu w bankowości elektronicznej – na swoje konto. Równie dobrze mógłby to być również samoczynnie wysyłający się formularz typu POST.
+ Ofiara loguje się do bankowości elektronicznej.
+ Ofiara wchodzi w innej zakładce przeglądarki na eeeevil-zite.com
+ Ofiara poprzez punkt 3. realizuje nieświadomie request (przelew) do swojej zalogowanej sesji w bankowości elektronicznej.

Oczywiście większość systemów bankowości elektronicznej jest w obecnie chroniona zarówno przed samą podatnością CSRF jak i dodatkowo wymaga dodatkowej autoryzacji przy przelewie na nieznane konto. 

Zauważmy również, że gdyby bankowośc przyjmowała requesty HTTP tylko metodą POST –  na eeeevil-zite.com moglibyśmy po prostu użyć odpowiednio spreparowany i samoczynnie wysyłający się formularz typu POST. Zatem korzystanie tylko requestów typu POST nie chroni przed CSRF. W tym przypadku OWASP podaje taki prosty przykład:


~~~
<body onload="document.forms[0].submit()">
<form action="http://bank.com/transfer.do" method="POST">
<input type="hidden" name="acct" value="MARIA"/>
<input type="hidden" name="amount" value="100000"/>
<input type="submit" value="View my pictures"/>
</form>
~~~

### 2.1.4. MitM

Atak typu Man in the Middle to atak, w którym sprawca ustawia się w rozmowie między użytkownikiem a aplikacją – albo w celu podsłuchania, albo podszycia się pod jedną ze stron, co sprawia wrażenie normalnej wymiany informacji jest w toku. 
Celem ataku jest kradzież danych osobowych, takich jak dane logowania, dane konta i numery kart kredytowych. 

<p align="center">
  Rys.2.1.4.1. Przykład ataku człowieka w środku
<br>
  <img src="\assets\img\Cyber\10.png" width="650" alt="mitm">
  <br>
  Źródło: https://www.imperva.com/learn/wp-content/uploads/sites/13/2017/09/man-in-the-middle-mitm-attack.png.webp
</p>

#### Atak składa się z dwóch odrębnych faz:

*Przechwycenie* – jest to pierwszy krok, w którym jest przechwytywany ruch użytkownika w sieci atakującego, zanim dotrze on do zamierzonego miejsca docelowego.

Najczęstszym sposobem na to jest atak pasywny, w którym osoba udostępnia publicznie bezpłatne, złośliwe hotspoty Wi-Fi. 

Atakujący, którzy chcą przyjąć bardziej aktywne podejście do przechwytywania, mogą przeprowadzić jeden z następujących ataków: 
+ Fałszowanie adresów IP  polega na tym, że atakujący podszywa się pod aplikację, zmieniając nagłówki pakietów w adresie IP. W rezultacie użytkownicy próbujący uzyskać dostęp do adresu URL połączonego z aplikacją są odsyłani na stronę atakującego.
+ Fałszowanie ARP  to proces łączenia adresu MAC osoby atakującej z adresem IP legalnego użytkownika w sieci lokalnej za pomocą fałszywych wiadomości ARP. W rezultacie dane wysyłane przez użytkownika na adres IP hosta są zamiast tego przesyłane do atakującego.
+ Fałszowanie DNS , znane również jako zatruwanie pamięci podręcznej DNS, polega na infiltracji serwera DNS i zmianie rekordu adresu strony internetowej. W rezultacie użytkownicy próbujący uzyskać dostęp do witryny są wysyłani przez zmieniony rekord DNS do witryny atakującego.



*Deszyfrowanie* – po przechwyceniu każdy dwukierunkowy ruch SSL musi zostać odszyfrowywany bez powiadomienia użytkownika lub aplikacji. Aby to osiągnąć, istnieje kilka metod:

+ Spoofing HTTPS  wysyła fałszywy certyfikat do przeglądarki ofiary po wysłaniu początkowego żądania połączenia z bezpieczną witryną. Przechowuje cyfrowy odcisk palca powiązany z zaatakowaną aplikacją, który przeglądarka weryfikuje zgodnie z istniejącą listą zaufanych witryn. Atakujący może wtedy uzyskać dostęp do wszelkich danych wprowadzonych przez ofiarę, zanim zostaną one przekazane do aplikacji.
+ SSL BEAST  (exploit przeglądarki przeciwko SSL/TLS) atakuje lukę TLS w wersji 1.0 w SSL. W tym przypadku komputer ofiary jest infekowany złośliwym kodem JavaScript, który przechwytuje zaszyfrowane pliki cookie wysyłane przez aplikację internetową. Następnie naruszono łańcuch bloków szyfrowania (CBC) aplikacji, aby odszyfrować jej pliki cookie i tokeny uwierzytelniające.
+ Przejęcie SSL  ma miejsce, gdy osoba atakująca przekazuje sfałszowane klucze uwierzytelniające zarówno użytkownikowi, jak i aplikacji podczas uzgadniania protokołu TCP. To ustanawia coś, co wydaje się być bezpiecznym połączeniem, podczas gdy w rzeczywistości mężczyzna w środku kontroluje całą sesję.
+ Usuwanie protokołu SSL  obniża jakość połączenia HTTPS do HTTP poprzez przechwycenie uwierzytelniania TLS wysyłanego z aplikacji do użytkownika. Atakujący wysyła niezaszyfrowaną wersję strony aplikacji do użytkownika, utrzymując jednocześnie zabezpieczoną sesję z aplikacją. Tymczasem cała sesja użytkownika jest widoczna dla atakującego.


#### Przykład 1: Przechwytywanie danych
+ Atakujący instaluje sniffer pakietów, aby analizować ruch sieciowy pod kątem niezabezpieczonej komunikacji.
+ Gdy użytkownik loguje się do witryny, osoba atakująca pobiera informacje o użytkowniku i przekierowuje go do fałszywej witryny, która naśladuje prawdziwą.
+ Fałszywa strona atakującego zbiera dane od użytkownika, które atakujący może następnie wykorzystać na prawdziwej stronie, aby uzyskać dostęp do informacji o celu.

#### Przykład 2: Uzyskanie dostępu do funduszy
+ Atakujący konfiguruje fałszywą usługę czatu, która naśladuje dobrze znany bank.
+ Wykorzystując wiedzę zdobytą z danych przechwyconych w pierwszym scenariuszu, atakujący podszywa się pod bank i rozpoczyna czat z celem.
+ Następnie atakujący rozpoczyna czat na prawdziwej stronie banku, podszywając się pod cel i przekazując potrzebne informacje, aby uzyskać dostęp do konta celu.

W tym scenariuszu osoba atakująca przechwytuje rozmowę, przekazując jej część obu uprawnionym uczestnikom.

<p align="center">
  Rys.2.1.4.2. Przykład ataku MitM
<br>
  <img src="\assets\img\Cyber\11.png" width="650" alt="mitm-1">
  <br>
  Źródło: https://www.veracode.com/sites/default/files/2021-07/veracode-mitm-remake.png
</p>


### 2.1.5. DoS i DDoS ataki na warstwie aplikacji

Celem tych ataków są protokoły warstwy aplikacji, takie jak HTTP i DNS, często z zamiarem zakłócenia usług lub przejęcia protokołów aplikacji. Typowe techniki ataków obejmują zalewy żądań, wykorzystywanie lub w zabezpieczeniach aplikacji, ataki specyficzne dla aplikacji, takie jak zalewy XML-RPC i ataki zero-day wykorzystywanie luk w zabezpieczeniach. 

Taki atak może doprowadzić do zakłócenia działania serwisu, a nawet całkowitego zamknięcia serwisu. Atak w warstwie aplikacji wykorzystuje protokoły komunikacyjne używane do wymiany danych między dwiema aplikacjami działającymi w Internecie. Zasadniczo wymaga mniej zasobów do przeprowadzenia udanego ataku w warstwie aplikacji w porównaniu z innymi typami ataków DDoS, ponieważ powoduje więcej szkód ze względu na swój dostosowany charakter ukierunkowany na określone usługi lub protokoły, na przykład HTTP, SMTP lub FTP. To sprawia, że ataki w warstwie aplikacji są powszechną taktyką zakłócania usług o znaczeniu krytycznym.

<p align="center">
  Rys.2.1.5.1. Działanie ataku DDoS 
<br>
  <img src="\assets\img\Cyber\12.png" width="650" alt="ddos">
  <br>
  Źródło: https://www.onelogin.com/images/patterns/text-image/ddos-app-layer-attack.png
</p>


### 2.1.6. Phising 

Atak phishing – jest to wyłudzanie informacji, czyli jest to rodzaj ataku socjotechnicznego często wykorzystywanego do kradzieży danych użytkownika. Występuje, gdy atakujący, podszywając się pod zaufaną jednostkę, nakłania ofiarę do otwarcia wiadomości e-mail lub innych rodzajów wiadomości tekstowych. Następnie odbiorca zostaje nakłoniony do kliknięcia złośliwego łącza, co może doprowadzić do instalacji złośliwego oprogramowania, zawieszenia systemu w ramach ataku ransomware lub ujawnienia poufnych informacji. 

#### Przykłady ataków phishingowych

Poniżej przedstawiam przykłady typowe próby wyłudzenia informacji: 

+ Sfałszowany e-mail rzekomo z  myuniversity.edu  jest masowo dystrybuowany do jak największej liczby członków wydziału.
+ Wiadomość e-mail zawiera informację, że hasło użytkownika wkrótce wygaśnie. Podano instrukcje, aby przejść do  myuniversity.edu/renewal  w celu odnowienia hasła w ciągu 24 godzin.


<p align="center">
  Rys.2.1.6.1. Przykład ataku phishingowego 
<br>
  <img src="\assets\img\Cyber\13.png" width="650" alt="phishing">
  <br>
  Źródło: https://www.imperva.com/learn/wp-content/uploads/sites/13/2019/01/phishing-attack-email-example.png
</p>


#### Kliknięcie łącza może spowodować kilka rzeczy. Na przykład:
+ Użytkownik jest przekierowywany do  myuniversity.edurenewal.com , fałszywej strony wyglądającej dokładnie tak samo jak prawdziwa strona odnowienia, na której wymagane są zarówno nowe, jak i istniejące hasła. Atakujący, monitorując stronę, przejmuje oryginalne hasło, aby uzyskać dostęp do zabezpieczonych obszarów sieci uniwersyteckiej.
+ Użytkownik zostaje przekierowany na właściwą stronę odnowienia hasła. Jednak podczas przekierowania złośliwy skrypt aktywuje się w tle, aby przejąć plik cookie sesji użytkownika. Efektem jest  odbity atak XSS  , dający sprawcy uprzywilejowany dostęp do sieci uniwersyteckiej.

#### Techniki phishingowe:
+ Oszustwa związane z phishingiem w wiadomościach e-mail

Osoba atakująca wysyła tysiące wiadomości, które mogą wykraść znaczące informacje i sumy pieniędzy. Linki w wiadomości przypominają ich legalne odpowiedniki, ale zazwyczaj mają błędnie napisaną nazwę domeny lub dodatkowe subdomeny. 


<p align="center">
  Rys.2.1.6.2. Błędna domena 
<br>
  <img src="\assets\img\Cyber\14.png" width="650" alt="phishing-1">
  <br>
  Źródło: https://www.imperva.com/learn/wp-content/uploads/sites/13/2019/01/phishing-scam-techniques-link.png.webp
</p>

+ Wyłudzanie informacji – celem jest konkretna osoba lub firma, a nie losowi użytkownicy. Jest to bardziej dogłębna wersja phishingu, która wymaga specjalnej wiedzy o organizacji, w tym o jej strukturze władzy. 

#### Atak może przebiegać w następujący sposób: 
+ Sprawca wyszukuje nazwiska pracowników działu marketingu organizacji i uzyskuje dostęp do najnowszych faktur projektowych.
+ Podając się za dyrektora marketingu, atakujący wysyła wiadomość e-mail do departamentalnego kierownika projektu (PM), używając wiersza tematu, który brzmi: Zaktualizowana faktura za kampanie w trzecim kwartale. Tekst, styl i dołączone logo powielają standardowy szablon wiadomości e-mail organizacji.
+ Łącze w wiadomości e-mail przekierowuje do chronionego hasłem wewnętrznego dokumentu, który w rzeczywistości jest sfałszowaną wersją skradzionej faktury.
+ PM jest proszony o zalogowanie się w celu przeglądania dokumentu. Atakujący kradnie jego dane uwierzytelniające, uzyskując pełny dostęp do wrażliwych obszarów w sieci organizacji.

Dostarczając atakującemu ważne dane logowania, spear phishing jest skuteczną metodą wykonania pierwszego etapu APT.


### 2.1.7. Brute Force

Atak Brute Force to metoda hakerska polegająca na „zgadywaniu” nazwy użytkownika i hasła w celu uzyskania nieautoryzowanego dostępu do systemu. Haker wypróbowuje wiele nazw użytkownika i haseł, często używając komputera do testowania szerokiej gamy kombinacji, dopóki nie znajdzie prawidłowych danych logowania.

Niektórzy używają aplikacji i skryptów jako narzędzi brutalnej siły. Narzędzia te wypróbowują wiele kombinacji haseł, aby ominąć procesy uwierzytelniania. W innych przypadkach osoby atakujące próbują uzyskać dostęp do aplikacji internetowych, wyszukując odpowiedni identyfikator sesji. 

Podczas gdy niektórzy atakujący nadal wykonują ataki siłowe ręcznie, obecnie wszystkie ataki siłowe są wykonywane przez boty. 


#### Rodzaje ataków Brute Force: 

<p align="center">
  Rys.2.1.7.1. Rodzaje ataków Brute Force 
<br>
  <img src="\assets\img\Cyber\15.png" width="650" alt="brute-force">
  <br>
  Źródło: https://tiny.pl/c71fx
</p>

+ Proste ataki Brute Force – jest to atak siłowy, w którym haker próbuje ręcznie odgadnąć dane logowania użytkownika bez użycia oprogramowania. Ataki te są proste, ponieważ wiele osób nadal używa słabych haseł lub stosuje złą etykietę dotyczącą haseł, na przykład używając tego samego hasła do wielu witryn internetowych. 
+ Ataki słownikowe – jest to rodzaj, w którym atakujący wybiera cel, a następnie sprawdza możliwe hasła pod kątem nazwy użytkownika tej osoby. Ten rodzaj ataku jest zwykle czasochłonny i ma małe szanse powodzenia z nowszymi, bardziej skutecznymi metodami ataku.
+ Ataki hybrydowe Brute Force – jest to połączenie ataku słownikowego z atakiem siłowym. Zaczyna się od tego, że haker zna nazwę użytkownika, a następnie przeprowadza atak słownikowy i proste metody brutalnej siły, aby odkryć kombinację logowania do konta. Atakujący zaczyna od listy potencjalnych słów, a następnie eksperymentuje z kombinacjami znaków, liter i cyfr, aby znaleźć prawidłowe hasło.
+ Odwrotny atak Brute Force – polega na tym, że osoba atakująca rozpoczyna proces ze znanym hasłem, które zwykle jest wykrywane podczas naruszenia sieci. Używają tego hasła do wyszukiwania pasujących danych logowania, korzystając z list milionów nazw użytkowników.
+ Upychanie poświadczeń – wykorzystuje znane wcześniej pary hasło-nazwa użytkownika, wypróbowując je na wielu stronach internetowych. Wykorzystuje fakt, że wielu użytkowników ma tę samą nazwę użytkownika i hasło w różnych systemach.


#### Narzędzia ataku Brute Force: 
+ Hydra – analitycy bezpieczeństwa używają narzędzia THC-Hydra do identyfikowania luk w systemach klienckich. Hydra szybko przechodzi przez dużą liczbę kombinacji haseł, zarówno prostych, brutalnych, jak i opartych na słownikach. Może atakować ponad 50 protokołów i wiele systemów operacyjnych. Hydra to otwarta platforma; społeczność zajmująca się bezpieczeństwem i osoby atakujące stale opracowują nowe moduły.


<p align="center">
  Rys.2.1.7.2. Narzędzie Hydra
<br>
  <img src="\assets\img\Cyber\16.png" width="650" alt="hydra">
  <br>
  Źródło: https://www.imperva.com/learn/wp-content/uploads/sites/13/2018/01/hydra-brute-force-attack.png.webp
</p>

+ Aircrack-ng – wykorzystuje słownik powszechnie używanych haseł do włamań do sieci bezprzewodowych.
+ John the Ripper – próbuje wszystkich możliwych kombinacji przy użyciu słownika możliwych haseł.
+ L0phtCrack – wykorzystuje tęczowe tabele, słowniki i algorytmy wieloprocesorowe.
+ Hashcat – może przeprowadzać proste ataki siłowe, oparte na regułach i ataki hybrydowe.
+ DaveGrohl – może być dystrybuowany na wielu komputerach.
+ Ncrack – narzędzie do łamania uwierzytelniania sieciowego. 

### 2.1.8. Fuzzing

Fuzzing – jest to technika używana do wykrywania błędów kodowania i luk w zabezpieczeniach oprogramowania, systemów operacyjnych lub sieci. Działa, próbując zawiesić system lub wywołać błędy, dostarczając dużą liczbę losowych danych wejściowych.

Systemy fuzzingowe bardzo dobrze radzą sobie z wykrywaniem pewnych rodzajów luk, w tym przepełnienia bufora, odmowy usługi (DoS), cross-site scripting i wstrzykiwania kodu . Są jednak mniej skuteczne w radzeniu sobie z cichymi zagrożeniami bezpieczeństwa, które powodują awarie lub widoczne błędy, takimi jak oprogramowanie szpiegujące , robaki, konie trojańskie i rootkity.

<p align="center">
  Rys.2.1.8.1. Procesy Fuzzing
<br>
  <img src="\assets\img\Cyber\17.png" width="650" alt="fuzzing">
  <br>
  Źródło: https://journals.plos.org/plosone/article/figure/image?size=large&id=10.1371/journal.pone.0237749.g001
</p>


#### Rodzaje Fuzzingu:
+ Fuzzing aplikacji – testuje funkcje interfejsu użytkownika, takie jak przyciski, pola wprowadzania w formularzach lub opcje w programach wiersza poleceń. Działa, uzyskując dostęp do funkcji z niezwykle wysoką częstotliwością, dostarczając nieprawidłowe treści, takie jak zbyt dużo tekstu w polach wejściowych, i próbując różnych losowych danych wejściowych.
+ Fuzzing protokołu – służy do testowania zachowania serwera, gdy zła treść jest wysyłana przez dany protokół. Głównym celem jest zapobieganie błędnej interpretacji żądań protokołów jako poleceń i wykonywaniu ich na serwerze. 
+ Rozmycie formatu pliku – tworzy uszkodzony plik i przedstawia go oprogramowaniu docelowemu do przetworzenia. Pliki są zwykle w standardowych formatach, takich jak .jpg, 
+ .docx lub .xml. Fuzzer może przetestować aplikację, dostarczając pliki, które nie pasują do oczekiwanego formatu lub zawierają nieoczekiwaną zawartość.

#### Narzędzia bezpieczeństwa Fuzzer:
+ Generative Fuzzers – może być wszystko, od całkowicie losowych danych po dane lekko zmanipulowane. Na przykład podczas testowania fuzz ruchu HTTP możliwe jest fuzzowanie całego pakietu, co oznacza, że prawdopodobnie nie dotarłby on do miejsca docelowego. Alternatywnie, generatywny fuzzer może rozbić pakiet na jego poszczególne komponenty i spróbować rozmyć każdy z nich osobno, zachowując nienaruszoną strukturę pakietu. Pozwala to na testowanie nieprawidłowej zawartości pakietu przy zachowaniu nagłówków TCP/IP i HTTP.
+ Mutation Fuzzers – pobierają zestaw prawidłowych danych wejściowych i wykonują na nich mutacje, aby wywołać błędy lub awarie w testowanym oprogramowaniu. Oto kilka przykładów technik mutacji:
- Odwracanie najmniej znaczącego bitu (LSB) — zmiana bitu na końcu każdej binarnej liczby całkowitej.
- Zaciemnianie żądań HTTP — dołączanie losowej wartości do każdej wartości nagłówka HTTP. Może to być bardzo skuteczne w wykrywaniu luk w zabezpieczeniach i zapewnia wysokie pokrycie kodu, ponieważ dane wejściowe są wystarczająco podobne do oryginalnych prawidłowych danych wejściowych.
- Szablony — użycie prawidłowej struktury lub formatu danych w celu zwiększenia szansy, że rozmyte dane wejściowe zostaną zaakceptowane przez system docelowy. Może to skrócić czas i zasoby testu rozmytego, zapewniając, że dane wejściowe są dobrze sformułowane.
+ Evolution Fuzzers – opera się na wykorzystaniu programowania genetycznego, zaprojektowanego w celu zbieżności w kierunku danych wejściowych, które doprowadzą do błędu. Algorytmy genetyczne wykorzystują koncepcje mutacji, krzyżowania i selekcji, aby znaleźć rozwiązania złożonych problemów.


### 2.1.9. Pharming

Atak Pharming to forma cyberataku, w której cyberprzestępca wysyła fałszywą stronę internetową zamiast prawdziwej, a ta fałszywa strona wygląda podobnie do prawdziwej strony internetowej. Cyberprzestępcy wykorzystują luki w zabezpieczeniach serwera DNS. Serwer DNS jest odpowiedzialny za konwersję nazwy domeny na adres IP. Pharming mógł odbywać się na dwa sposoby albo poprzez wykorzystanie luki w oprogramowaniu serwera DNS, albo poprzez zmianę pliku hosta na komputerze ofiary. Cyberprzestępcy celowo przekierowują użytkowników do fałszywej wersji strony internetowej w celu uzyskania dostępu i kradzieży nazw użytkowników i haseł.

<p align="center">
  Rys.2.1.9.1. Działanie ataku pharmingowego
<br>
  <img src="\assets\img\Cyber\18.png" width="650" alt="pharming">
  <br>
  Źródło: https://media.geeksforgeeks.org/wp-content/uploads/20211018205404/pharmingattack1.png
</p>

+ Za każdym razem, gdy użytkownik odwiedza oszukańcze strony internetowe, złośliwe oprogramowanie jest instalowane na komputerze i uszkadza informacje, co okazuje się być atakiem typu pharming.
+ Za każdym razem, gdy użytkownik odwiedza dowolny adres URL za pośrednictwem dowolnej przeglądarki, takiej jak Chrome, Mozilla Firefox, Opera itp., przeglądarka kontaktuje się z serwerem DNS i żąda adresu IP żądanej domeny. Spowoduje to zmianę samego serwera DNS i zamieni się w atak typu pharming.


### 2.1.10. Remote Code Execution (RCE)

Remote Code Execution – to rodzaj luki w zabezpieczeniach, która umożliwia atakującym uruchomienie dowolnego kodu na komputerze zdalnym, łącząc się z nim za pośrednictwem sieci publicznych lub prywatnych.

#### Jak działa RCE?

Atakujący RCE skanują Internet w poszukiwaniu wrażliwych aplikacji. Gdy zauważą lukę w zdalnym kodzie, atakują ją przez sieć. Po uzyskaniu dostępu do systemu atakujący często próbują podnieść swoje uprawnienia z użytkownika na administratora.

<p align="center">
  Rys.2.1.10.1. Działanie ataku RCE
<br>
  <img src="\assets\img\Cyber\19.png" width="650" alt="RCE">
  <br>
  Źródło: https://tblocks.com/wp-content/uploads/2023/06/How-Does-A-LOG4J-JNDI-Attack-Happen.jpg
</p>

#### Rodzaje ataków RCE:
+ Atak iniekcyjny – różne aplikacje umożliwiają wprowadzanie danych wejściowych przez użytkownika w celu wykonywania poleceń. Atakujący mogą celowo podawać zniekształcone dane wejściowe w celu wykonania dowolnego kodu.
+ Atak deserializacji – aplikacje często wykorzystują serializację do organizowania danych w celu ułatwienia komunikacji. Programy do deserializacji mogą interpretować dane serializowane dostarczone przez użytkownika jako kod wykonywalny.
+ Zapis poza zakresem – aplikacje często przydzielają stałe fragmenty pamięci do przechowywania danych. Luki w alokacji pamięci umożliwiają atakującym dostarczanie danych wejściowych, które zapisują poza buforem — pamięć przechowuje kod wykonywalny, w tym złośliwy kod.

#### Techniki exploitów do zdalnego wykonywania kodu: 
+ Zdalna ocena kodu – ocena kodu ma miejsce, gdy funkcje oceniające kod akceptują dane wejściowe użytkownika. Na przykład niektóre aplikacje umożliwiają użytkownikom generowanie nazw zmiennych przy użyciu ich nazw użytkowników — użytkownicy kontrolują swoje nazwy użytkowników, dzięki czemu mogą tworzyć nazwy użytkowników zawierające złośliwy kod i wpływać na aplikacje, które umożliwiają ocenę danych wejściowych dla określonego języka programowania.
+ Ocena zapianego kodu – opiera się na przetwarzaniu plików przez tłumacza, a nie na określonych funkcjach językowych. Na przykład aplikacja może mieć panel sterowania dla każdego użytkownika z określonymi ustawieniami zmiennych językowych, które są przechowywane w pliku konfiguracyjnym. Atakujący mogą zmodyfikować parametr języka, aby wstrzyknąć kod do pliku konfiguracyjnego, umożliwiając im wykonanie dowolnych poleceń.


### 2.1.11. Clickjacking / UI Redressing

Clickjacking to atak polegający na nakłonieniu użytkownika do kliknięcia elementu strony internetowej, który jest niewidoczny lub zamaskowany jako inny element. Zazwyczaj przechwytywanie kliknięć polega na wyświetlaniu niewidocznej strony lub elementu HTML w ramce iframe na górze strony, którą widzi użytkownik. 

<p align="center">
  Rys.2.1.11.1. Atack Clickjacking
<br>
  <img src="\assets\img\Cyber\20.png" width="650" alt="clickjacking">
  <br>
  Źródło: https://portswigger.net/web-security/images/clickjacking-infographic.svg
</p>

#### Istnieje kilka odmian ataku typu clickjacking, takie jak:
+ Likejacking – technika polegająca na manipulacji przyciskiem „Lubię to” Facebooka, powodująca „polubienie” przez użytkowników strony, której tak naprawdę nie zamierzali polubić.
+ Cursorjacking – technika zmiany interfejsu użytkownika, która zmienia kursor pozycji postrzeganej przez użytkownika na inną pozycję. Cursorjacking opiera się na lukach we Flashu i przeglądarce Firefox, które zostały już naprawione.

#### Przykład ataku typu clickjacking:
+ Atakujący tworzy atrakcyjną stronę, która obiecuje użytkownikowi darmową wycieczkę na Tahiti.
+ W tle atakujący sprawdza, czy użytkownik jest zalogowany do swojego serwisu bankowego, a jeśli tak, ładuje ekran umożliwiający przelew środków, używając parametrów zapytania do wstawienia danych bankowych atakującego do formularza.
+ Strona przelewu bankowego jest wyświetlana w niewidocznej ramce iframe nad stroną z darmowymi prezentami, z przyciskiem „Potwierdź przelew” dokładnie ustawionym nad przyciskiem „Odbierz prezent” widocznym dla użytkownika.
+ Użytkownik wchodzi na stronę i klika przycisk „Zarezerwuj moją darmową podróż”.
+ W rzeczywistości użytkownik klika niewidoczny element iframe i klika przycisk „Potwierdź transfer”. Środki są przekazywane atakującemu.
+ Użytkownik zostaje przekierowany na stronę z informacją o darmowym prezencie (nie wiedząc, co się stało w tle).

<p align="center">
  Rys.2.1.11.2. Przykład ataku typu clickjacking
<br>
  <img src="\assets\img\Cyber\21.png" width="650" alt="clickjacking-1">
  <br>
  Źródło: https://www.imperva.com/learn/wp-content/uploads/sites/13/2019/01/Clickjacking.png.webp
</p>

#### Jak skonstruować podstawowy atak typu clickjacking?

Ataki typu „clickjacking” wykorzystują CSS do tworzenia warstw i manipulowania nimi. Atakujący włącza docelową stronę internetową jako warstwę iframe nałożoną na wabiącą stronę internetową. Przykład użycia znacznika stylu i parametrów jest następujący:

~~~
<head>
	<style>
		#target_website {
			position:relative;
			width:128px;
			height:128px;
			opacity:0.00001;
			z-index:2;
			}
		#decoy_website {
			position:absolute;
			width:300px;
			height:400px;
			z-index:1;
			}
	</style>
</head>
...
<body>
	<div id="decoy_website">
	...decoy web content here...
	</div>
	<iframe id="target_website" src="https://vulnerable-website.com">
	</iframe>
</body>
~~~

Element iframe witryny docelowej jest umieszczany w przeglądarce w taki sposób, że akcja docelowa dokładnie pokrywa się z witryną wabiącą przy użyciu odpowiednich wartości pozycji szerokości i wysokości. Bezwzględne i względne wartości pozycji są używane w celu zapewnienia, że docelowa witryna dokładnie pokrywa się z przynętą, niezależnie od rozmiaru ekranu, typu przeglądarki i platformy. Z-index określa kolejność układania warstwy elementu iframe i strony internetowej. Wartość krycia jest zdefiniowana jako 0,0 (lub bliska 0,0), dzięki czemu zawartość elementu iframe jest przezroczysta dla użytkownika. Ochrona przeglądarki przed przechwytywaniem kliknięć może stosować wykrywanie przezroczystości ramek iframe na podstawie wartości progowych. Atakujący wybiera wartości krycia tak, aby osiągnąć pożądany efekt bez wyzwalania zachowań ochronnych.


### 2.1.12. Server-Side Request Forgery (SSRF)

Atak Server-Side Request Forgery – polega na tym, że osoba atakująca nadużywa funkcjonalności serwera w celu uzyskania dostępu do zasobów lub ich modyfikacji. Celem atakującego jest aplikacja obsługująca import danych z adresów URL lub umożliwiająca odczytywanie danych z adresów URL. Adresami URL można manipulować, zastępując je nowymi lub modyfikując przechodzenie przez ścieżkę URL. 


<p align="center">
  Rys.2.1.12.1. Działanie ataku SSRF
<br>
  <img src="\assets\img\Cyber\22.png" width="650" alt="ssrf">
  <br>
  Źródło: https://portswigger.net/web-security/images/server-side%20request%20forgery.svg
</p>

#### Rodzaje ataków SSRF:
+ Ataki SSRF na serwery – polega na tym, że osoba atakująca wykorzystuje proces, w którym przeglądarka lub inny system kliencki uzyskuje bezpośredni dostęp do adresu URL na serwerze. Osoba atakująca zastąpi oryginalny adres URL innym, zazwyczaj używając adresu IP 127.0.0.1 lub nazwy hosta „localhost”, które wskazują na lokalny system plików na serwerze. Pod tą nazwą hosta atakujący znajduje ścieżkę do pliku, która prowadzi do wrażliwych plików. 

<p align="center">
  Rys.2.1.12.2. Działanie ataku SSRF na serwery
<br>
  <img src="\assets\img\Cyber\23.png" width="650" alt="ssrf-2">
  <br>
  Źródło: https://www.imperva.com/learn/wp-content/uploads/sites/13/2021/12/How-Server-SSRF-works.png
</p>

+ Back-endowe ataki SSRF – atak, w którym serwer ma zaufaną relację z komponentem zaplecza. Jeśli serwer, który połączy się z tym komponentem, ma pełne prawa dostępu, osoba atakująca może sfałszować żądanie i uzyskać dostęp do wrażliwych danych lub wykonać nieautoryzowane operacje. Komponenty zaplecza często mają słabe zabezpieczenia, ponieważ są uważane za chronione wewnątrz obwodu sieci.

#### Omijanie typowych mechanizmów obronnych SSRF:
+ SSRF z filtrami wejściowymi opartymi na czarnej liście – niektóre aplikacje blokują dane wejściowe zawierające nazwy hostów, takie jak 127.0.0.1 i localhost, lub wrażliwe adresy URL, takie jak /admin. W takiej sytuacji można obejść filtr w następujący sposób: 
- Użyć alternatywnej reprezentacji adresu IP 127.0.0.1, takie jak 2130706433, 017700000001, lub 127.1
- Zarejestrować własną nazwę domeny, która jest tłumaczona na 127.0.0.1 (można użyć spoofed.burpcollaborator.netw tym celu)
- Zaciemnianie zablokowanych ciągów przy użyciu kodowania adresów URL lub zmiany wielkości liter.
- Podanie kontrolowanego adresu URL, który następnie przekierowuje do docelowego adresu URL
+ SSRF z filtrami wejściowymi opartymi na białej liście – niektóre aplikacje zezwalają tylko na dane wejściowe, które pasują do białej listy dozwolonych wartości, zaczynają się od niej lub zawierają. W takiej sytuacji można czasami obejść filtr, wykorzystując niespójności w analizie adresów URL. Specyfikacja adresu URL zawiera szereg funkcji, które można przeoczyć podczas implementacji analizowania ad hoc i sprawdzania poprawności adresów URL:
+ Można osadzić poświadczenia w adresie URL przed nazwą hosta, używając @znaku. Na przykład: https://expected-host:fakepassword@evil-host
- Można użyć #znaku, aby wskazać fragment adresu URL. Na przykład: https://evil-host#expected-host
o	Można wykorzystać hierarchię nazw DNS, aby umieścić wymagane dane wejściowe we w pełni kwalifikowanej nazwie DNS, którą można kontrolować. Na przykład: https://expected-host.evil-host
- Można zakodować znaki w adresie URL, a by zmylić kod analizujący adres URL. 
+ Omijanie filtrów SSRF poprzez otwarte przekierowanie – czasami możliwe jest obejście wszelkiego rodzaju zabezpieczeń opartych na filtrach, wykorzystując lukę w zabezpieczeniach polegającą na otwartym przekierowaniu. 

Załóżmy na przykład, że aplikacja zawiera lukę umożliwiającą otwarcie przekierowania, w której następujący adres URL: 

~~~
/product/nextProduct?currentProductId=6&path=http://evil-user.net
~~~

Zwraca przekierowanie: 

~~~
http://evil-user.net
~~~

Można wykorzystać lukę w zabezpieczeniach związaną z otwartym przekierowaniem, aby ominąć filtr adresów URL i wykorzystać lukę w zabezpieczeniach SSRF w następujący sposób: 

~~~
POST /product/stock HTTP/1.0
Content-Type: application/x-www-form-urlencoded
Content-Length: 118

stockApi=http://weliketoshop.net/product/nextProduct?currentProductId=6&path=http://192.168.0.68/admin
~~~

Ten exploit SSRF działa, ponieważ aplikacja najpierw sprawdza, czy podany stockAPIadres URL znajduje się w dozwolonej domenie, co jest prawdą. Następnie aplikacja żąda podanego adresu URL, co wyzwala otwarte przekierowanie. Podąża za przekierowaniem i wysyła żądanie do wewnętrznego adresu URL wybranego przez atakującego.

### 2.1.13. XML Ecternal Entity (XXE) Injection 

XM External Entity Injection – to luka w zabezpieczeniach, która umożliwia atakującemu wstrzyknięcie niebezpiecznych jednostek XML do aplikacji internetowej przetwarzającej dane XML. Luki w zabezpieczeniach XXE są spowodowane przez parsery XML, które są przestarzałe lub nieprawidłowo skonfigurowane. 

<p align="center">
  Rys.2.1.13.1. Działanie ataku XXE
<br>
  <img src="\assets\img\Cyber\24.png" width="650" alt="xxe">
  <br>
  Źródło: https://portswigger.net/web-security/images/xxe-injection.svg
</p>

#### Rodzaje ataków XXE:
+ Wykorzystanie XXE do pobierania plików – definiowana jest zewnętrzna jednostka zawierająca zawartość pliku i zwracana w odpowiedzi aplikacji. 
+ Wykorzystanie XXE do przeprowadzania ataków SSRF – podmiot zewnętrzny jest definiowany na podstawie adresu URL do systemu zaplecza. 
+ Eksfiltracja danych poza pasmem wykorzystując Blind XXE – poufne dane są przesyłane z serwera aplikacji do systemu kontrolowanego przez atakującego. 
+ Pobieranie danych za pośrednictwem komunikatów o błędach wykorzystując Blind XXE – osoba atakująca może wywołać komunikat o błędzie analizy składniowej zawierający poufne dane. 

#### Przykład ataku XXE:

Na przykład osoba atakująca może wykonać następujące żądanie przy użyciu identyfikatora URI wskazującego na poufny plik na serwerze. Jeśli parser XML jest skonfigurowany do przetwarzania jednostek zewnętrznych, serwer WWW zwróci zawartość tego pliku.

<p align="center">
  Rys.2.1.13.2. Prośba o dołączenie
<br>
  <img src="\assets\img\Cyber\25.png" width="650" alt="xxe-1">
  <br>
  Źródło: https://www.imperva.com/learn/wp-content/uploads/sites/13/2023/01/Screen-Shot-2023-01-30-at-14.27.42.png.webp
</p>


<p align="center">
  Rys.2.1.13.3. Odpowiedź
<br>
  <img src="\assets\img\Cyber\26.png" width="650" alt="xxe-2">
  <br>
  Źródło: https://www.imperva.com/learn/wp-content/uploads/sites/13/2023/01/Screen-Shot-2023-01-30-at-14.34.18.png.webp
</p>


### Remote File Inclusion (RFI)

Remote File Inclusion – to atak ukierunkowany na luki w aplikacjach internetowych, które dynamicznie odwołują się do zewnętrznych skryptów. Celem sprawcy jest wykorzystanie funkcji odwoływania się w aplikacji do przesyłania złośliwego oprogramowania ze zdalnego adresu URL znajdującego się w innej domenie.

<p align="center">
  Rys.2.1.13.4. Przebieg ataku RFI
<br>
  <img src="\assets\img\Cyber\27.png" width="650" alt="rfi">
  <br>
  Źródło: https://www.imperva.com/learn/wp-content/uploads/sites/13/2019/01/what-is-rfi-attack.png
</p>

#### Przykład dołączania plików zdalnych:

Strona JSP zawiera następujący wiersz kodu: 

~~~
<jsp:include page=”<%=(String)request.getParmeter(“ParamName”)%>”>
~~~

którym można manipulować za pomocą następującego żądania: 

~~~
Page1.jsp?ParamName= /WEB-INF/DB/hasło
~~~

przetworzenie żądania ujawni sprawcy zawartość pliku z hasłami.


### 2.1.15. Local File Inclusion (LFI)

Local File Inclusion to technika ataku polegająca na nakłanianiu aplikacji internetowej do uruchomienia lub ujawnienia plików na serwerze WWW. Ataki LFI mogą ujawnić poufne informacje, a w poważnych przypadkach mogą prowadzić do skryptów krzyżowych (XSS) i zdalnego wykonania kodu.

<p align="center">
  Rys.2.1.15.1. Działanie ataku LFI
<br>
  <img src="\assets\img\Cyber\28.png" width="650" alt="Lfi">
  <br>
  Źródło: https://miro.medium.com/v2/resize:fit:720/format:webp/1*UPMlwBWgKMSUzSvY5mt5uw.png
</p>

#### Przykład ataku LFI:
~~~
https://example-site.com/?module=contact.php
~~~

Osoba atakująca może zmienić adres URL, aby wyglądał następująco

~~~
https://example-site.com/?module=/etc/passwd
~~~

A w przypadku braku odpowiedniego filtrowania serwer wyświetli wrażliwą zawartość pliku /etc/passwd. 


### 2.1.16. Directory Travel

Directory Traversal – to luka w zabezpieczeniach sieci WEB, która umożliwia osobie atakującej odczytanie dowolnych plików na serwerze, na którym działa aplikacja. 

<p align="center">
  Rys.2.1.16.1. Działanie ataku Directory Travel
<br>
  <img src="\assets\img\Cyber\29.png" width="650" alt="DT">
  <br>
  Źródło: https://portswigger.net/web-security/images/directory-traversal.svg
</p>

#### Odczytywanie dowolnych plików poprzez przeglądanie katalogów

Weźmy dla przykładu aplikację zakupową, która wyświetla obrazy przedmiotów na sprzedaż. Obrazy ładowane za pomocą kodu HTML, jak poniżej:

~~~
<img src="/loadImage?filename=218.png">
~~~

Aplikacja czyta z następującej ścieżki: 

~~~
/var/www/images/218.png
~~~

Aplikacja nie implementuje mechanizmów obronnych przed atakami polegającymi na przeglądaniu katalogów, więc osoba atakująca może zażądać następującego adresu URL w celu pobrania dowolnego pliku z systemu plików serwera:

~~~
https://insecure-website.com/loadImage?filename=../../../etc/passwd
~~~

Powoduje to, że aplikacja odczytuje z następującej ścieżki pliku:

~~~
/var/www/images/../../../etc/passwd
~~~

### 2.1.17. Credential Stuffing

Credential Stuffing (ang. upychanie poświadczeń) – to metoda, w której napastnicy wykorzystują listy przejętych poświadczeń użytkownika w celu włamania się do systemu. Atak wykorzystuje boty do automatyzacji i skalowania oraz opiera się na założeniu, że wielu użytkowników ponownie używa nazw użytkowników i haseł w wielu usługach. 

#### Jak działają ataki polegające na upychaniu poświadczeń

Oto typowy proces, po którym przeprowadza się atakujący w ataku polegającym na upychaniu poświadczeń na dużą skalę. Atakujący:
+ Konfiguruje bota, który może automatycznie logować się równolegle do wielu kont użytkowników, jednocześnie fałszując różne adresy IP.
+ Uruchamia zautomatyzowany proces sprawdzania, czy skradzione dane uwierzytelniające działają na wielu stronach internetowych. Uruchamiając proces równolegle w wielu witrynach, zmniejszając potrzebę wielokrotnego logowania się do jednej usługi.
+ Monitoruje pomyślne logowanie i uzyskuje dane osobowe, dane kart kredytowych lub inne cenne dane ze zhakowanych kont.
+ Przechowuje informacje o koncie do wykorzystania w przyszłości, na przykład w przypadku ataków typu phishing lub innych transakcji umożliwionych przez zaatakowaną usługę.


<p align="center">
  Rys.2.1.17.1. Przykład ataku
<br>
  <img src="\assets\img\Cyber\30.png" width="650" alt="CS">
  <br>
  Źródło: https://www.imperva.com/learn/wp-content/uploads/sites/13/2020/01/credentials.png.webp
</p>


### 2.1.18. Server-Side Template Injection (SSTI)

Server-Side Template Injection (ang. wstrzykiwanie szablonu po stronie serwera) – atak polegający na wstrzykiwaniu szablonu po stronie serwera ma miejsce, gdy ugrupowanie cyberprzestępcze wykorzystuje natywną składnię szablonu i wstrzykuje do niego złośliwe ładunki. Zaatakowany szablon jest następnie wykonywany po stronie serwera. Silnik szablonów generuje stronę internetową, łącząc stały szablon z niestabilnymi danymi.

Atakujący wykorzystują technikę wstrzykiwania szablonów po stronie serwera, aby bezpośrednio wstawiać dane wejściowe użytkownika do szablonów, co pozwala im na wprowadzanie dowolnych dyrektyw, które zmieniają zachowanie silnika szablonów. Może pozwolić cyberprzestępcom na uzyskanie pełnej kontroli nad docelowym serwerem.

#### Konstruowanie ataku polegającego na wstrzyknięciu szablonu po stronie serwera

Identyfikacja podatności na wstrzyknięcie szablonu po stronie serwera i przygotowanie udanego ataku zazwyczaj obejmuje następujący proces wysokiego poziomu.

<p align="center">
  Rys.2.1.18.1. Konstruowanie ataku
<br>
  <img src="\assets\img\Cyber\31.png" width="650" alt="SSTI">
  <br>
  Źródło: https://portswigger.net/web-security/images/ssti-methodology-diagram.png
</p>

+ Wykryć
Jak w przypadku każdej luki w zabezpieczeniach, pierwszym krokiem w kierunku wykorzystania jest możliwość jej znalezienia. Najprostszym podejściem jest próba rozmycia szablonu przez wstrzyknięcie sekwencji znaków specjalnych powszechnie używanych w wyrażeniach szablonów, takich jak ${{<%[%'"}}%\. Jeśli zostanie zgłoszony wyjątek, oznacza to, że wstrzyknięta składnia szablonu jest potencjalnie w jakiś sposób interpretowana przez serwer. Jest to jedna z oznak, że może istnieć podatność na wstrzyknięcie szablonu po stronie serwera.
+ Zidentyfikować
Po wykryciu potencjału wstrzyknięcia szablonu następnym krokiem jest zidentyfikowanie silnika szablonu. Samo przesłanie nieprawidłowej składni jest często wystarczające, ponieważ wynikowy komunikat o błędzie powie dokładnie, jaki jest silnik szablonu, a czasem nawet, która wersja. W przeciwnym razie należy przetestować różne ładunki specyficzne dla języka i zbadać, w jaki sposób są one interpretowane przez silnik szablonów. Powszechnym sposobem na sprawdzenie jest wstrzykiwanie dowolnych operacji matematycznych przy użyciu składni z różnych silników szablonów. Aby wspomóc ten proces, można użyć drzewa decyzyjnego podobnego do następujących: 

<p align="center">
  Rys.2.1.18.1. Drzewo decyzyjne
<br>
  <img src="\assets\img\Cyber\32.png" width="650" alt="SSTI-1">
  <br>
  Źródło: https://portswigger.net/web-security/images/template-decision-tree.png
</p>

+ Wykorzystać
Po wykryciu potencjalnej luki w zabezpieczeniach i pomyślnym zidentyfikowaniu mechanizmu szablonów można przystąpić do poszukiwania sposobów jego wykorzystania.



### 2.1.19. Business Logic Attack

Ataki na logikę biznesową (ang. business logic attacks) to rodzaj cyberataków, które polegają na wykorzystaniu i manipulowaniu procesami i regułami biznesowymi systemów informatycznych w celu uzyskania nieautoryzowanych korzyści. Odróżniają się one od tradycyjnych ataków, które skupiają się na podatnościach technicznych, takich jak błędy w oprogramowaniu czy słabe zabezpieczenia.

<p align="center">
  Rys.2.1.19.1. Działanie luki w logice biznesowej
<br>
  <img src="\assets\img\Cyber\33.png" width="650" alt="BLA">
  <br>
  Źródło: https://portswigger.net/web-security/images/logic-flaws.jpg
</p>

Celem atakujących jest wprowadzenie systemu w stan, w którym będzie generował nieprawidłowe wyniki lub umożliwiał wykonanie działań, które normalnie byłyby niedozwolone. Przykładowo, atakujący może próbować zmodyfikować warunki rabatów w sklepie internetowym, aby uzyskać wyższe zniżki niż przysługujące, lub zmieniać parametry transakcji w bankowości elektronicznej, aby manipulować saldem konta.

#### Jak chronić się przed tym atakiem?

Aby chronić się przed atakami na logikę biznesową, organizacje powinny podjąć kilka działań. Przede wszystkim należy odpowiednio projektować i testować logikę biznesową, aby minimalizować możliwość manipulacji i błędów. Należy również wprowadzić mechanizmy kontroli i monitorowania, które pozwolą wykryć nieprawidłowości w działaniu systemu. Ważne jest również szkolenie personelu, aby zwiększyć świadomość zagrożeń i umożliwić identyfikację podejrzanych aktywności.

## 2.2. Ataki na warstwie prezentacji

Warstwa prezentacji, zwana także „warstwą składni”, odpowiada za formatowanie i tłumaczenie danych do formatu określonego przez warstwę aplikacji. Oznacza to, że działa jako translator danych w sieci, aby zapewnić, że dane wysyłane przez warstwę aplikacji są czytelne dla warstwy aplikacji systemu odbierającego.

### 2.2.1. Man-in-the-browser (MitB)

Man-in-the-browser (MitB) – jest to atak, w którym sprawca instaluje na komputerze ofiary konia trojańskiego, który jest w stanie modyfikować transakcje internetowe tego użytkownika. Z tej racji, że ataki tego typu wymagają zainstalowanego złośliwego oprogramowania trojana na docelowym komputerze, sprawcy często wykorzystują luki w zabezpieczeniach lub taktyki phishingu, aby zainicjować atak. Ataki MitB są przeprowadzane za pośrednictwem skryptu użytkownika, obiektu pomocniczego przeglądarki lub niezabezpieczonego rozszerzenia przeglądarki. 
Atak MitB ma miejsce, gdy ofiara samodzielnie wpisze adres URL w przeglądarce, bez zewnętrznego monitu. 

<p align="center">
  Rys.2.2.1.1. Działanie ataku MitB
<br>
  <img src="\assets\img\Cyber\34.png" width="650" alt="mitb">
  <br>
  Źródło: https://cdn.ttgtmedia.com/rms/onlineimages/a_man_in_the_browser_attack-f_mobile.png
</p>

#### Przykłady ataków Man-in-the-browser:
+ Zeus to atak MitB, który kradnie dane logowania do bankowości internetowej i przeprowadza nieautoryzowane transfery środków. Był również używany do przeprowadzania oszustw związanych z pomocą techniczną.
+ OddJob to atak MitB przeznaczony do użycia na stronach bankowych. Atak jest instalowany przez przeglądarkę Firefox lub IE i aktywuje się, gdy zainfekowany użytkownik otworzy stronę bankową. Celem ataku jest token identyfikatora sesji użytkownika w czasie rzeczywistym w celu dokonania transakcji na koncie bankowym. Atak jest trudny do wykrycia, ponieważ nie jest przechowywany na dysku urządzenia.
+ SpyEye to trojan, który prosi użytkownika o podanie informacji, takich jak konta bankowe, hasła, nazwy użytkownika lub numery kart kredytowych. Atak może również działać jako keylogger.

## 2.2.2. Content Spoofing

Content Spoofing (ang. fałszowanie treści) – jest to atak wymierzony w użytkownika, możliwy dzięki luce w zabezpieczeniach aplikacji internetowej. Atak typu Content Spoofing na warstwie prezentacji odnosi się do manipulacji zawartością, która jest wyświetlana użytkownikom na stronie internetowej lub aplikacji. Atak ten polega na fałszowaniu wyglądu strony lub aplikacji w celu uzyskania poufnych informacji od użytkowników lub przekierowania ich na złośliwe strony.

### Sposoby ataku Content Spoofing: 
+ Fałszywe strony internetowe: Atakujący może stworzyć fałszywą stronę internetową, która wygląda jak oryginalna, np. logowanie do konta bankowego. Strona może wykorzystywać podobną szatę graficzną, aby zmylić użytkowników i skłonić ich do podania poufnych informacji, takich jak hasła czy dane karty kredytowej.
+ Modyfikacja zawartości: Atakujący może zmieniać zawartość wyświetlaną na stronie lub aplikacji, np. zmieniać treść formularzy, przekierować na złośliwe strony lub wstrzykiwać złośliwe skrypty. W rezultacie użytkownik może zostać oszukany, wykonując nieświadomie działania, które są korzystne dla atakującego.
+ Spoofing adresu URL: Atakujący może manipulować adresem URL wyświetlanym w przeglądarce, aby wyglądał jak zaufany serwis, podczas gdy w rzeczywistości użytkownik jest kierowany na złośliwą stronę. To może być szczególnie skuteczne w przypadku phishingu, gdzie atakujący podszywa się pod znane instytucje, takie jak banki czy serwisy społecznościowe.

## 2.2.3. MIME Sniffing

MIME Sniffing (ang. uniwersalne wąchanie rozszerzeń poczty internetowej) – to proces automatycznego rozpoznawania typu zawartości pliku na podstawie jego treści, a nie jedynie na podstawie nagłówków HTTP. Jest to funkcjonalność często wbudowana w przeglądarki internetowe.

<p align="center">
  Rys.2.2.3.1. Działanie MIME Sniffing
<br>
  <img src="\assets\img\Cyber\35.png" width="650" alt="mime">
  <br>
  Źródło: https://www.keycdn.com/img/support/mime-sniffing-md.webp
</p>

### Jak działa wykrywanie MIME?
+ Przeglądarka internetowa żąda określonego zasobu, który odpowiada bez typu zawartości lub z typem zawartości ustawionym wcześniej na serwerze źródłowym.
+ Przeglądarka internetowa „węszy” zawartość, aby przeanalizować, w jakim formacie pliku jest ten konkretny zasób.
+ Po zakończeniu analizy przeglądarka porównuje to, co znalazła, z tym, co serwer WWW podał w nagłówku Content-Type. W przypadku niezgodności przeglądarka używa typu MIME, który został powiązany z zasobem.

## 2.2.4. HTML Injection

HTML Injection (ang. wstrzyknięcie HTML) – to technika używana do wykorzystania niezweryfikowanych danych wejściowych do modyfikowania strony internetowej prezentowanej użytkownikom przez aplikację internetową. Atakujący wykorzystują fakt, że zawartość strony internetowej jest często związana z wcześniejszą interakcją z użytkownikiem. Gdy aplikacje nie sprawdzają poprawności danych użytkownika, osoba atakująca może wysłać tekst w formacie HTML w celu zmodyfikowania zawartości witryny, która jest prezentowana innym użytkownikom. Specjalnie spreparowane zapytanie może doprowadzić do umieszczenia na stronie internetowej kontrolowanych przez osobę atakującą elementów HTML, które zmieniają sposób, w jaki zawartość aplikacji jest udostępniana w sieci.

<p align="center">
  Rys.2.2.4.1. Działanie ataku HTNL Injection
<br>
  <img src="\assets\img\Cyber\36.png" width="650" alt="html">
  <br>
  Źródło: https://assets.website-files.com/5ff66329429d880392f6cba2/6455e1f13e0fb0b257e9ce71_HTML%20Injection%20Work.jpg
</p>

### Przykład HTML Injection
+ Najpierw atakujący znajduje witrynę podatną na wstrzyknięcie kodu HTML
+ Następnie osoba atakująca wysyła adres URL ze złośliwym kodem wstrzykniętym do adresu URL do użytkownika ofiary za pośrednictwem poczty elektronicznej lub innego mechanizmu.
+ Jeśli ofiara kliknie ten szkodliwy adres URL, uruchomi kod JavaScript lub VBScript z uprawnieniami użytkownika ofiary.
+ W zależności od wykonywanego kodu może ujawnić poufne informacje użytkownika, a nawet skompromitować komputer ofiary.

## 2.2.5. JavaScript Injection

JavaScript Injection (ang. wstrzyknięcie JavaScript) – atak, który polega na tym, że osoba atakująca wstrzykuje złośliwy kod bezpośrednio do kodu JavaScript po stronie klienta. Kod ten jest uruchamiany i renderowany, gdy ofiara ładuje witrynę ze złośliwym skryptem w swojej aplikacji klienckiej/ przeglądarce. Osoba atakująca może polegać na różnych technikach wprowadzania złośliwego kodu do podatnej witryny, w tym:
+ Używanie konsoli programisty przeglądarki do wstawiania kodu JavaScript lub zmiany kodu źródłowego
+ Dodanie skryptu poprzez wpisanie elementu JavaScript: SCRIPT do paska adresu klienta
+ Używanie skryptów międzywitrynowych do dodawania skryptów do pola komentarza lub formularza wejściowego

### Przykłady JavaScript Injection
+ Wstrzykiwanie zależności w JavaScript – skierowany jest na platformę DI (dependency injection), w której atakujący nakłania witrynę do pobrania niestandardowych skryptów z wybranego repozytorium. Podczas instalowania pakietów dla aplikacji JavaScript instalatorzy zazwyczaj wybierają najnowszą wersję, gdy mają do wyboru dwie wersje tego samego pliku. Załóżmy, że złośliwy użytkownik może uzyskać nazwę wewnętrznej zależności lub pliku skryptu. W takim przypadku mogą opublikować złośliwy kod aplikacji o wyższym numerze wersji w publicznym repozytorium określanym jako package.json lub inny plik kodu źródłowego. Podczas instalowania pakietów lub zależności złośliwy kod zostaje wstrzyknięty do kodu źródłowego aplikacji, gdy instalator aplikacji wybierze zaktualizowaną-zmodyfikowaną wersję.
+ Atak polegający na wstrzykiwaniu kodu JavaScript – polega na wstrzykiwaniu wykonywalnego kodu HTML przez wrażliwe pole wejściowe. Typowe znaczniki używane do osadzenia kodu HTML w aplikacjach JavaScript to: <SCRIPT>, <OBJECT>, <APPLET>, <EMBED>, <FK>, <LI>, <BR>, <DIV>, <TITLE>
+ Wstrzykiwanie kodu JavaScript – te ataki akceptują dane wprowadzane przez użytkownika i wykonują je po stronie serwera. Poniższy fragment kodu pokazuje przykład podatnej witryny:

~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Darwin Website</title>
</head><body>
    <input type="button" onclick="randomScript()">
</body>
</html>
~~~

W takim wzorcu kodu osoba atakująca może przesłać złośliwy kod do losowej funkcji randomScript() w celu wdrożenia detektora zdarzeń. Osiąga się to poprzez zbudowanie niestandardowego skryptu w konsoli zgodnej z JavaScript i JQuery w celu zmiany zdarzenia onclick. Kod będzie wyglądał podobnie do:

~~~
function randomScript(){
  alert("Test!");
}
~~~

Następnie wszyscy hakerzy muszą sprawdzić element przycisku po otwarciu strony internetowej. Daje to hakerowi dostęp do zakładki detektorów zdarzeń, która wyświetla kod uruchamiany przez funkcję randomScript(). 
+ Wstrzykiwanie kodu JavaScript do kodu SQL – polega na wykorzystywaniu błędów sprawdzania poprawności danych wejściowych w celu wstrzyknięcia złośliwych zapytań SQL do aplikacji. Modyfikuje to oryginalne zapytania do bazy danych, co umożliwia atakującemu odczytywanie poufnych treści, modyfikowanie/usuwanie wpisów w bazie danych lub zmianę zachowania serwera.


Aplikacja podatna na ataki może używać ciągów literalnych, aby umieścić wyszukiwane hasło bezpośrednio w ciągu kodu, jak pokazano:
~~~
const query = `SELECT * FROM Repository WHERE TAG = '${userQuery}' AND public = 1`;
~~~

Zgodnie z powyższą konstrukcją zapytania, ciąg zapytania SQL do wyszukiwania terminu Darwin byłby podobny do:
~~~
SELECT * FROM Repository WHERE TAG = 'darwin' AND public = 1;
~~~

Osoba atakująca może podać złośliwe wyszukiwane hasło darwin' ;–, które modyfikuje instrukcję SQL w następujący sposób:
~~~
SELECT * FROM Repository WHERE TAG = 'darwin';--' AND public = 1;
~~~

To komentuje każdą część po — znakach, skutecznie pozostawiając wykonane polecenie SQL podobne do:
~~~
SELECT * FROM Repository WHERE TAG = 'darwin';
~~~

Ponieważ usuwa to dodatkową klauzulę, która zapobiega ujawnianiu prywatnych repozytoriów w odpowiedzi serwera bazy danych, osoba atakująca może uzyskać dostęp do kodu źródłowego, plików konfiguracyjnych serwera i innych własności intelektualnych organizacji.

## 2.2.6. Web Scraping

Screen (Web) Scraping (ang. skrobanie sieci) – to proces wykorzystywania botów do wydobywania treści i danych ze strony internetowej. 

W przeciwieństwie do screen scrapingu, który kopiuje tylko piksele wyświetlane na ekranie, web scraping wyodrębnia leżący u podstaw kod HTML, a wraz z nim dane przechowywane w bazie danych. Skrobak może następnie replikować całą zawartość witryny w innym miejscu.

### Narzędzia do scrapingu i boty:

Narzędzia do skrobania stron internetowych to oprogramowanie (tj. boty) zaprogramowane do przeszukiwania baz danych i wydobywania informacji. Wykorzystywane są różne typy botów, z których wiele można w pełni dostosować do:
+ Rozpoznać unikalne struktury witryn HTML
+ Wyodrębnić i przekształć zawartość
+ Przechować zeskrobane dane
+ Wyodrębnić dane z interfejsów API

<p align="center">
  Rys.2.2.6.1. Działanie Web Scraping
<br>
  <img src="\assets\img\Cyber\37.png" width="650" alt="scraping">
  <br>
  Źródło: https://www.imperva.com/learn/wp-content/uploads/sites/13/2019/01/web-scraping-attack.jpg.webp
</p>

### Przykłady złośliwego web scraping:
+ Skrobanie cen – sprawca wykorzystuje botnet, z którego uruchamia boty typu scraper w celu sprawdzenia konkurencyjnych biznesowych baz danych. Celem jest uzyskanie dostępu do informacji o cenach, podcięcie konkurencji i zwiększenie sprzedaży.
+ Skrobanie treści – obejmuje kradzież treści na dużą skalę z danej witryny. Typowe cele obejmują katalogi produktów online i strony internetowe, które wykorzystują treści cyfrowe do napędzania biznesu. W przypadku tych przedsiębiorstw atak polegający na skrobaniu treści może być katastrofalny.


## 2.2.7. Code Injection

Wstrzykiwanie kodu (ang. Code Injection) – polega na wstrzyknięciu kodu do osadzenia złośliwego kodu w kodzie źródłowym, który aplikacja interpretuje i wykonuje. Podczas złośliwego wstrzykiwania osoby atakujące wykorzystują fakt, że systemy te konstruują część segmentu kodu przy użyciu danych zewnętrznych, bez wystarczającej weryfikacji danych wejściowych. Złośliwy kod jest zwykle tworzony w celu kontrolowania przepływu danych, co prowadzi do utraty poufności i ograniczenia dostępności aplikacji.

Atakujący identyfikują luki w walidacji danych wprowadzanych przez użytkownika, takie jak – format danych, dozwolone znaki i ilość oczekiwanych danych – i wykorzystują je jako podstawę do opracowania złośliwego kodu.

<p align="center">
  Rys.2.2.7.1. Działanie ataku Code Injection
<br>
  <img src="\assets\img\Cyber\38.png" width="650" alt="cinjection">
  <br>
  Źródło: https://images.ctfassets.net/4un77bcsnjzw/5biUz7wg0X90MDjKEwVAbm/42283a77ad24497dee3aea2f5c51632d/CodeInjection_Attack.svg
</p>

### Jak działa Code Injection

Hakerzy najpierw sondują aplikację pod kątem powierzchni ataku, które mogą akceptować niezaufane dane i wykorzystywać je podczas wykonywania kodu programu. Obejmują one bezpośrednie dane wejściowe, takie jak przesyłanie plików, pola formularzy lub inne źródła danych, takie jak pliki cookie i parametry ciągu zapytania.

Wprowadzenie kodu zazwyczaj polega na bezpośredniej konkatenacji ciągu znaków, funkcji PHP eval() lub jej odpowiednika w innym języku. Udany exploit zapewnia atakującym dostęp do interpretera aplikacji po stronie serwera. Atakujący mogą używać wywołań systemowych do uruchamiania poleceń na serwerze i penetrować dalej w celu głębszego wykorzystania.

### Rodzaje exploitów ataku

#### Wstrzykiwanie kodu po stronie klienta

Podczas wstrzykiwania po stronie klienta hakerzy wykorzystują luki w aplikacjach, w których sprawdzanie poprawności danych wejściowych odbywa się w przeglądarce przed wysłaniem danych na serwer. Takie ataki obejmują:
+ Wstrzykiwanie kodu SQL – atakujący atakują wrażliwe szczegóły konfiguracji w systemach zarządzania relacyjnymi bazami danych, aby kontrolować serwer bazy danych aplikacji internetowej za pomocą złośliwych instrukcji SQL. Instrukcje te modyfikują zapytania SQL, dając hakerom dostęp do kluczowych danych, takich jak dane logowania i informacje o konfiguracji aplikacji.
+ Wstrzykiwanie kodu Pythona – aplikacje zbudowane w Pythonie, skrypty, które akceptują wyrażenia od użytkowników i oceniają ich dane wejściowe, mogą być wykorzystywane do wstrzykiwania złośliwego kodu.
+ Wstrzykiwanie kodu HTML – wykorzystanie luk w zabezpieczeniach związanych z wstrzyknięciem kodu HTML, aby naruszyć sposób interakcji użytkowników z aplikacją internetową. Robiąc to, haker wstrzykuje złośliwy kod HTML do zaufanej witryny internetowej, wykonując niezaufane skrypty w przeglądarce użytkownika końcowego.

#### Wstrzykiwanie kodu po stronie serwera

Wstrzyknięcie kodu po stronie serwera polega na wykorzystaniu luk w aplikacjach, które sprawdzają poprawność danych wprowadzonych przez użytkownika po stronie serwera. Obejmują one:
+ Wstrzykiwanie kodu PHP –  niektóre aplikacje internetowe zbudowane w języku PHP mogą zawierać niebezpieczną funkcję, która umożliwia atakującym kontrolę nad częścią lub całością oprogramowania. Te luki umożliwiają hakerom zmianę przebiegu wykonywania kodu poprzez modyfikację części ciągu wejściowego
+ Wstrzykiwanie kodu JavaScript po stronie serwera – stosunkowo łatwo jest wstawić własny kod Javascript witryny internetowej i użyć go, znajdując lukę w zabezpieczeniach skryptów krzyżowych lub umieszczając kod w pasku adresu.


## 2.2.8. Malformed Content Attack 

Atak zniekształconej zawartości (ang. Malformed Content Attack) – rodzaj cyberataku, w których atakujący celowo tworzy lub modyfikuje zawartość, tatką jak dane lub pliki, w sposób naruszający oczekiwany format lub strukturę. 

Podstawową ideą tego ataku jest wprowadzanie nieprawidłowych lub nieoczekiwanych danych do systemu lub aplikacji, które mogą prowadzić do wykorzystania podatności w oprogramowaniu. Atakujący może wykorzystać te naruszenia w celu wykonania różnych działań, takich jak:
+ Wstrzyknięcie złośliwego kodu
+ Wywołanie błędów systemowych
+ Odwrócenie kolejności wykonywania instrukcji
+ Przechwycenie danych

## 2.2.9. Session Sidejacking

Session Sidejacking – atak, w którym atakujący uzyskuje dostęp do sesyjnego pliku cookie i nadużywa go, aby podszyć się pod użytkownika ofiary. Pozwala to złośliwemu użytkownikowi na wykonywanie różnych czynności, które w innym przypadku użytkownik mógłby wykonać po zalogowaniu się na stronie internetowej. 

### Jak odbywa się atak Sidejacking?

Zasadniczo sidejacking opiera się na identyfikacji niezaszyfrowanego - nie przez SSL – pliku cookie. Atakujący może użyć sniffera pakietów do wyszukania takiego sesyjnego pliku cookie. 

Po znalezieniu dobrego celu złośliwy użytkownik podsłuchuje ruch sieciowy. Następnie może użyć niezaszyfrowanego pliku cookie do podszywania się pod zwykłego użytkownika za pomocą swoich danych uwierzytelniających. Atakujący widzi zatem wszystkie dane przesyłane między przeglądarką ofiary a serwerem lub stroną internetową.

Dobrą wiadomością jest jednak to, że po zakończeniu sesji i wylogowaniu uprawnionego użytkownika należy wysłać dalsze żądania do serwera, a przyszłe sesje będą wymagały uwierzytelnienia nowego klienta. Oznacza to, że po zakończeniu aktywnej sesji atakujący traci nieautoryzowany dostęp.  

### Rodzaje Sidejacking 
+ Cookie hijacking – polega na kradzieży plików cookie sesji. Pliki cookie są używane do przechowywania informacji o sesji, takich jak identyfikator sesji, loginy, tokeny uwierzytelniające itp. Atakujący może przejąć te pliki cookie i użyć ich do podszywania się pod użytkownika, oszukując serwer.
+ Session hijacking – polega na przechwyceniu aktywnej sesji użytkownika. Atakujący monitoruje komunikację między użytkownikiem a serwerem, w poszukiwaniu wartości sesji, takich jak identyfikatory sesji, tokeny itp. Gdy atakujący przechwyci te dane, może użyć ich do uzyskania nieuprawnionego dostępu do konta użytkownika.
+ SSL/TLS stripping – wykorzystuje braki w zabezpieczeniach SSL/TLS, które chronią transmisję danych między użytkownikiem a serwerem. Atakujący może przechwycić komunikację między użytkownikiem a serwerem, zdejmując zaszyfrowanie SSL/TLS. W rezultacie atakujący może podejrzeć i modyfikować przesyłane dane, takie jak hasła, poufne informacje itp.
+ Man-in-the-Middle attack – polega na wprowadzeniu się pomiędzy użytkownika a serwer, tworząc fałszywe połączenie między nimi. Atakujący może monitorować i przechwytywać komunikację między nimi, kradnąc wrażliwe informacje. Może również modyfikować przesyłane dane lub przekierowywać użytkownika na fałszywe strony.


## 2.2.10. CSS Injection

Podatności na wstrzykiwanie CSS pojawiają się, gdy aplikacja importuje arkusz stylów z adresu URL podanego przez użytkownika lub osadza dane wprowadzone przez użytkownika w blokach CSS bez odpowiedniej ucieczki. Są one ściśle powiązane z lukami w zabezpieczeniach związanymi ze skryptami krzyżowymi (XSS), ale ich wykorzystanie jest często trudniejsze.

<p align="center">
  Rys.2.2.10.1. Działanie ataku CSS Injection
<br>
  <img src="\assets\img\Cyber\39.png" width="650" alt="cssinjection">
  <br>
  Źródło: https://palant.info/2021/06/28/having-fun-with-css-injection-in-a-browser-extension/css_injection.png
</p>

Możliwość wstrzyknięcia dowolnego kodu CSS do przeglądarki ofiary może umożliwić różne ataki, w tym:
+ Wykonywanie dowolnego kodu JavaScript przy użyciu funkcji expression() przeglądarki IE.
+ Używanie selektorów CSS do odczytywania części źródła HTML, które mogą zawierać poufne dane, takie jak tokeny anty-CSRF.
+ Przechwytywanie wszelkich poufnych danych w ciągu zapytania adresu URL poprzez dalsze importowanie arkusza stylów do adresu URL w domenie atakującego i monitorowanie przychodzącego nagłówka strony odsyłającej.

## 2.2.11. Cookie Manipulation

Przeglądarka traktuje pliki cookie jako węzły DOM, więc możliwe jest manipulowanie plikami cookie za pośrednictwem DOM. Najczęstszym zastosowaniem tej techniki jest usunięcie lub edycja wartości pliku cookie. Na przykład usunięcie plików cookie innych firm może pozwolić komuś na ominięcie problemów ze śledzeniem między witrynami poprzez wyczyszczenie identyfikatora modułu śledzącego z jego pamięci.

<p align="center">
  Rys.2.2.11.1. Cookie Manipulation
<br>
  <img src="\assets\img\Cyber\40.png" width="650" alt="cmanipulation">
  <br>
  Źródło: https://media.geeksforgeeks.org/wp-content/uploads/20220817124742/dombasedcookiemanipulationattack1.png
</p>


## 2.2.12. Browser Fingerprinting

Odcisk palca (ang. Browser Fingerprinting) przeglądarki to termin używany do opisania czynności polegającej na dyskretnym gromadzeniu danych o oprogramowaniu i ustawieniach urządzenia za pośrednictwem przeglądarki internetowej użytkownika, gdy jest on online. Ta kombinacja ustawień jest następnie wykorzystywana do zbudowania unikalnej tożsamości – lub „odcisku palca” – dla tej osoby. Jest to również czasami określane jako „odcisk palca urządzenia” lub po prostu „odcisk palca”.

### Jak działa odcisk palca przeglądarki internetowej?

Za każdym razem, gdy witryna internetowa jest odświeżana przeglądarka musi dostarczyć serwerowi hostingowemu pewną ilość niezbędnych informacji, aby zapewnić prawidłowe działanie witryny na indywidualnej maszynie. 

Te informacje mogą obejmować model i specyfikację urządzenia, język i układ klawiatury, lokalizację, strefę czasową, zainstalowany sprzęt, wersje oprogramowania i wiele innych.

Pojedynczo te ustawienia i konfiguracje mogą wydawać się nieszkodliwe – i tak jest. Ale po złożeniu mogą stworzyć niepowtarzalną kombinację lub „odcisk palca”.

## 2.3. Ataki na warstwie sesji

Warstwa sesji jest odpowiedzialna za synchronizację wszystkiego działania. Na przykład nie można po prostu „wyświetlić” strony internetowej. Przejęcie sesji może nastąpić na różne sposoby, w tym cross-site scripting, sidejacking, naprawę, kradzież plików cookie i próby brutalnej siły. 

## 2.3.1. Session Hijacking

Przejęcie sesji to technika wykorzystywana przez hakerów w celu uzyskania dostępu do komputera lub kont internetowych ofiary. Podczas ataku polegającego na przejęciu sesji haker przejmuje kontrolę nad sesją przeglądania użytkownika, aby uzyskać dostęp do jego danych osobowych i haseł. 

### Jak działa przejęcie sesji?

Porywacz sesji może przejąć kontrolę nad sesją użytkownika na kilka sposobów. Jedną z powszechnych metod jest użycie sniffera pakietów do przechwycenia komunikacji między użytkownikiem a serwerem, co pozwala hakerowi zobaczyć, jakie informacje są wysyłane i odbierane. Mogą następnie użyć tych informacji, aby zalogować się na konto lub uzyskać dostęp do wrażliwych danych.

Przejęcie sesji może również nastąpić poprzez wdrożenie złośliwego oprogramowania w celu zainfekowania komputera użytkownika. Daje to hakerowi bezpośredni dostęp do maszyny, umożliwiając mu przejęcie dowolnej aktywnej sesji.

### Przykłady

Session Sniffing- atakujący najpierw używa sniffera do przechwycenia ważnej sesji tokena o nazwie „Session ID”, a następnie używa ważnej sesji tokena do uzyskania nieautoryzowanego dostępu do serwera WWW.

<p align="center">
  Rys.2.3.1.1. Session Sniffing
<br>
  <img src="\assets\img\Cyber\41.png" width="650" alt="sniffing">
  <br>
  Źródło: https://owasp.org/www-community/assets/images/attacks/session-hijacking.jpg
</p>

Cross-site script attack – osoba atakująca może naruszyć token sesji, używając złośliwego kodu lub programów działających po stronie klienta. Przykład pokazuje, w jaki sposób osoba atakująca może użyć ataku XSS do kradzieży tokena sesji. Jeśli atakujący wyśle do ofiary spreparowany link ze złośliwym kodem JavaScript, gdy ofiara kliknie link, JavaScript zostanie uruchomiony i wykona instrukcje podane przez atakującego.

<p align="center">
  Rys.2.3.1.2. Cross-site script attack
<br>
  <img src="\assets\img\Cyber\42.png" width="650" alt="cssattack">
  <br>
  Źródło: https://owasp.org/www-community/assets/images/attacks/code-injection.jpg
</p>

## 2.3.2. Session Fixation

Atak utrwalania sesji to rodzaj ataku polegającego na zdalnym wykonaniu kodu, który jest wykorzystywany do wykorzystywania oprogramowania zaprojektowanego z funkcją zarządzania sesją serwera WWW. Gdy witryna internetowa korzysta z serwera HTTP, informacje o stanie sesji serwera mogą zostać skradzione, a następnie odzyskane przez osobę atakującą w celu przejęcia przeglądarki lub wykorzystania jej do dalszych ataków.

<p align="center">
  Rys.2.3.2.1. Działanie Session Fixation Attack
<br>
  <img src="\assets\img\Cyber\43.png" width="650" alt="sfixation">
  <br>
  Źródło: https://media.geeksforgeeks.org/wp-content/uploads/20220711160012/sessionfixationattack.png
</p>

### Atak utrwalania sesji:
+ Atak utrwalania sesji to atak, który ma miejsce, gdy złośliwy użytkownik konfiguruje fałszywą sesję, zanim legalni użytkownicy będą mogli się zalogować. Prowadzi to do naruszenia bezpieczeństwa całego systemu i wykorzystania go do kradzieży poufnych danych.
+ Atak utrwalania sesji jest najczęściej obserwowany w systemach bankowych, gdzie hakerzy próbują uzyskać dostęp poprzez założenie konta z minimalnymi wymaganiami startowymi. 
+ Dzięki tej metodzie omijają wszelkie środki bezpieczeństwa, takie jak CAPTCHA lub rozpoznawanie odcisków palców, które banki mogły zastosować przed kradzieżą poufnych danych. Jedną z metod stosowanych przez banki przeciwko atakom utrwalania sesji jest tokenizacja, która chroni konta, jednocześnie utrudniając hakerom wykorzystanie fałszywych danych uwierzytelniających.
+ Atak utrwalania sesji to rodzaj ataku polegającego na zdalnym wykonaniu kodu, który jest wykorzystywany do wykorzystywania oprogramowania zaprojektowanego z funkcjami zarządzania sesją serwera WWW.
+ Gdy witryna działa na serwerze HTTP, informacje o stanie sesji serwera mogą zostać skradzione, a następnie odzyskane przez atakującego w celu przejęcia przeglądarki lub wykorzystania jej do dalszych ataków.

### Procedura:
+ Atakujący tworzy złośliwą sesję HTTP z przeglądarką ofiary, przejmuje uwierzytelnianie klienta i kopiuje użytkownika. 
+ Atakujący może to zrobić, przechwytując ruch HTTP z/do przeglądarki, modyfikując lub odtwarzając istniejące prawidłowe sesje lub projektując nową szkodliwą sesję. Kradzież sesji wykorzystuje luki w zabezpieczeniach aplikacji, które nie chronią odpowiednio swoich danych. 
+ Następnie osoba atakująca uzyskuje dostęp i modyfikuje dane związane z przechwyconą sesją, takie jak pliki cookie.
+ Funkcje protokołu HTTP, takie jak metody GET i POST, umożliwiają klientom wysyłanie informacji do serwera, ale nie zawierają mechanizmu powiadamiania serwera przez klientów o odebraniu tych informacji. 
+ Aby ułatwić tę wymianę informacji, protokół HTTP obsługuje pliki cookie. Ponieważ pliki cookie są przesyłane tam iz powrotem między przeglądarką a serwerem w każdym cyklu żądania/odpowiedzi, możemy ich również używać do przejmowania sesji klientów ze stronami internetowymi.
+ Pliki cookie mogą być wykorzystywane przez osoby atakujące w celu przeprowadzania ataków polegających na przejęciu sesji, a dokładnie o to chodzi w atakach typu Session Hijacking lub Session Fixation. Techniki utrwalania sesji, takie jak cross-site scripting (XSS), cross-site request forgery (CSRF) i kradzież sesji, to aktywne zagrożenia, które są już znane w środowisku naturalnym.

## 2.2.3. Session Replay

Session Replay – jest to atak, polegający na powtórce sesji przy pomocy narzędzi takich jak Wireshark. Celem hakera jest uzyskanie dostępu do sieci, danych i zasobów w celu naprawienia wszelkich luk, które mogą zostać wykorzystane przez adwersarzy.

Ataki z powtórzeniem sesji, znane również jako ataki z powtórzeniem lub powtórzeniem, to ataki sieciowe, które złośliwie „ponawiają” lub „opóźniają” prawidłowe transmisje danych. Hakerzy mogą to zrobić, przechwytując sesję i kradnąc unikalny identyfikator sesji użytkownika (przechowywany jako plik cookie, adres URL lub pole formularza). Haker może teraz podszywać się pod autoryzowanego użytkownika i mieć pełny dostęp do wszystkiego, co autoryzowany użytkownik może robić w witrynie.

Atak powtórkowy ma miejsce, gdy cyberprzestępca przechwytuje bezpieczną komunikację sieciową, przechwytuje ją i w nieuczciwy sposób opóźnia lub przesyła, aby skłonić odbiorcę do zrobienia tego, czego chce haker. Dodatkowe ryzyko ataków polega na tym, że hakerzy nie potrzebują nawet zaawansowanych umiejętności do odszyfrowywania wiadomości po przechwyceniu ich z sieci. Atak może się powieść po prostu poprzez ponowne wysłanie wszystkiego.

<p align="center">
  Rys.2.3.3.1. Działanie Session Replay Attack
<br>
  <img src="\assets\img\Cyber\44.png" width="650" alt="sra">
  <br>
  Źródło: https://media.geeksforgeeks.org/wp-content/uploads/20220720163836/sessionreplay1.png
</p>

### Przykład:

Aplikacja internetowa przechowuje sesję w parametrze zapytania:

Aplikacja internetowa może zarządzać sesją użytkownika na podstawie wartości parametru zapytania.

~~~
http://example.com/home/show.php?SESSIONID=MOJASESJA
~~~
gdzie MYSESJA to identyfikator sesji.

Ta metoda jest podatna na atak polegający na powtórzeniu sesji, znany jako atak polegający na utrwalaniu sesji. 
+ Atakujący generuje własny identyfikator sesji.
+ Atakujący wysyła adres URL ze swoim identyfikatorem sesji do prawidłowego użytkownika aplikacji. 

~~~
Np.: http://example.com/home/show.php?SESSIONID=ATTACKER-SESSION
~~~

+ Gdy prawidłowy użytkownik kliknie łącze, sesja zostanie uruchumiona z identyfikatorem sesji ATTACKER_SESSION. 
+ Prawidłowy użytkownik łączy się z aplikacją przy użyciu swoich poświadczeń. 
+ Osoba atakująca może teraz podszyć się pod prawidłowego użytkownika, odwiedzając go. 

~~~
http://example.com/home/show.php?SESSIONID=SESJA ATAKUJĄCA
~~~

## 2.3.4. Session Prediction

Session Prediction Attack (atak przewidywany) – jest to atak przewidujący sesję, który koncentruje się na przewidywaniu wartości identyfikatora sieci, która pozwalaja atakującemu ominąć schemat uwierzytelnienia aplikacji. Analizując i rozumiejąc proces generowania identyfikatora sesji, osoba atakująca może przewidzieć prawidłową wartość identyfikatora sesji i uzyskać dostęp do aplikacji.

<p align="center">
  Rys.2.3.4.1. Działanie Session Replay Attack
<br>
  <img src="\assets\img\Cyber\45.png" width="650" alt="sp">
  <br>
  Źródło: https://media.geeksforgeeks.org/wp-content/uploads/20220715114649/SessionPrediction1.png
</p>

### Jak działa Session Prediction?
+ Najpierw należy zebrac kilka prawidłowych wartości identyfikatora sesji, które są używane do identyfikacji uwierzytelnionych użytkowników. 
+ Nastepnie należy zrozumieć struktuę identyfikatora sesji, informacje używane do jego utworzenia oraz algorytm szyfrowania lub skrótu używay przez aplikację do jego ochrony. 

### Przykład

Informacje o identyfikatorze sesji dla określonej aplikacji zwykle składają się z ciągu znaków o stałej szerokości. Losowość jest bardzo ważna, aby uniknąć jej przewidywania. Patrząc na przykład na rysunku 2.3.4.1, zmienna identyfikatora sesji jest reprezentowana przez JSESSIONID, a jej wartość to „user01”, co odpowiada nazwie użytkownika. Wypróbowując dla niego nowe wartości, takie jak „user02”, można dostać się do aplikacji bez wcześniejszego uwierzytelnienia.

<p align="center">
  Rys.2.3.4.2. Przewidywalny plik cookie
<br>
  <img src="\assets\img\Cyber\46.png" width="650" alt="sp-1">
  <br>
  Źródło: https://owasp.org/www-community/assets/images/attacks/predictable-cookie.jpg
</p>

## 2.3.5. Brute-Force Attacks on Session IDs

Ataki brute force na identyfikatory sesji są jedną z metod atakujących systemy informatyczne. Identyfikatory sesji są unikalnymi wartościami przypisanymi użytkownikom podczas korzystania z aplikacji internetowych, aby śledzić ich sesje. Brute force attack to technika polegająca na wielokrotnym próbowaniu różnych kombinacji, aż do znalezienia poprawnego identyfikatora sesji.

Atakujący, korzystając z metody brute force, próbuje automatycznie generować i testować różne wartości identyfikatorów sesji, aż do znalezienia takiego, który będzie pasował i umożliwi nieuprawniony dostęp do konta użytkownika. Jest to proces czasochłonny, ponieważ atakujący musi sprawdzić ogromną ilość kombinacji, aby znaleźć właściwy identyfikator sesji.

## 2.3.6. Cross-Site Session Transfer

Atak przeniesienia sesji między stronami (ang. Cross-Site Session Transfer Attack) jest to technika wykorzystywana przez atakujących w celu przejęcia sesji użytkownika z jednej witryny na inną. Polega to na przechwyceniu identyfikatora sesji (np. ciasteczka) podczas interakcji użytkownika z jedną stroną i wykorzystaniu go do nieuprawnionego dostępu do innej strony, na której sesja jest aktywna.

### Główne czynniki, które mogą przyczynić się do takiego ataku, to:
+ Użycie niebezpiecznych metod przesyłania identyfikatora sesji
+ Współużytkowanie identyfikatora sesji
+ Luki w mechanizmach zarządzania sesją

## 2.3.7. Session Timeout Attacks

Session Timeout Attacks (przekroczenie limitu czasu sesji) – atak, w którym użytkownik nie wykonuje żadnej akcji na stronie internetowej w czasie (określonym przez serwer WWW). Zdarzenie po stronie serwera zmienia status sesji użytkownika na „nieważna” (tzn. „nieużywana”) i nakazuje serwerowi sieciowemu zniszczenie sesji (usunięcie wszystkich zawartych w niej danych).

### Rodzaje Session Timeout Attack:
+ Deklaratywnie w deskryptorze wdrożenia sieciowego (plik “web.xml”) – stosowana do wszystkich sesji utworzonych dla aplikacji. 

~~~
<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    ns="http://java.sun.com/xml/ns/javaee" xmlns:web="http://java.sun.com/xml/ns/javaee/web-app_2_5.xsd"
    xsi:schemaLocation="http://java.sun.com/xml/ns/javaee http://java.sun.com/xml/ns/javaee/web-app_3_0.xsd"
    id="WebApp_ID" version="3.0">
    ...
    <!-- Define a session timeout to 15 minutes -->
    <session-config>
        <session-timeout>15</session-timeout>
    </session-config>
    ...
</web-app>
~~~

+ Programowo w obiekcie sesji – dotyczy tylko bieżącej sesji. 

~~~
package org.owasp.javaproject.sessiontimeout;

import java.io.IOException;

import javax.servlet.ServletException;
import javax.servlet.annotation.WebServlet;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import javax.servlet.http.HttpSession;

/**
 * Code sample showing how to access to session timeout and act on it.
 */
@SuppressWarnings("serial")
@WebServlet("/SessionTimeout")
public class SessionTimeoutCodeSample extends HttpServlet {
    /**
     * {@inheritDoc}
     *
     * @see javax.servlet.http.HttpServlet#doGet(javax.servlet.http.HttpServletRequest,
     *      javax.servlet.http.HttpServletResponse)
     */
    @SuppressWarnings("boxing")
    @Override
    protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
        // Get reference on session object
        HttpSession session = req.getSession();
        // Display session timeout value defined in "web.xml"
        // Value here is specified in seconds...
        System.out.printf("Session timeout defined at application level : %s\n", session.getMaxInactiveInterval());
        // Change session timeout for this session and display new timeout value
        // Value here is defined in seconds...
        session.setMaxInactiveInterval(60);
        System.out.printf("Session timeout defined at code level : %s\n", session.getMaxInactiveInterval());
    }
}
Session timeout defined at application level : 900
Session timeout defined at code level : 60
~~~

## 2.3.8. Insufficient Session Expiration

Insufficient Session Expiration (niewystarczające wygaśnięcie sesji) – może być wynikiem złego wdrożonego zarządzania sesją. Ta słabość może pojawić się na poziomie projektowania i implementacji i może zostać wykorzystana przez osoby atakujące w celu uzyskania nieautoryzowanego dostępu do aplikacji. 

Podczas obsługi sesji twórcy stron internetowych mogą polegać na tokenach serwera lub generować identyfikatory sesji w aplikacji. Każda sesja powinna zostać zniszczona po naciśnięciu przez użytkownika przycisku wylogowania lub po upływie określonego czasu, zwanego limitem czasu. Niestety błędy w kodowaniu i błędne konfiguracje serwera mogą mieć wpływ na proces obsługi sesji, co może skutkować nieautoryzowanym dostępem.

### Przykład podatnego kodu

Załóżmy, że mamy aplikację, która używa ciasteczek do uwierzytelniania użytkowników. Identyfikator sesji jest przekazywany w pliku cookie i jest używany przez twórców oprogramowania do uwierzytelniania odwiedzających.

Identyfikator sesji jest generowany w bezpieczny sposób za pomocą funkcji „GenerateSecureToken()”. Funkcja „ValidateSession()” przeprowadza walidację wcześniej wygenerowanej sesji.

~~~
<?php
if ( puste ( $_COOKIE [ "ID_SESJI" ] ) ) :
        $SessionID = GenerateSecureToken ( ) ;
        setcookie ( "SESSION_ID" , $SessionID , czas ( ) * 3600 ) ;
elseif ( ValidateSession ( $_COOKIE [ "SESSION_ID" ] ) ) :
        echo "Cześć" . $Logowanie użytkownika ;
inaczej :
        echo "Proszę podać dane uwierzytelniające" ;
endif ;
?>
~~~

Luka jest wprowadzana z powodu nieprawidłowego użycia funkcji PHP „setcookie()”. Deweloper zapewnił wyjątkowo długi czas życia pliku cookie „SESSION_ID”, co oznacza, że ta sesja nie wygaśnie szybko, a właściciel pliku cookie może automatycznie uwierzytelnić się w długim okresie czasu. Jeśli ten plik cookie zostanie skradziony, osoba atakująca może użyć identyfikatora sesji do uwierzytelnienia aplikacji podatnej na ataki i uzyskania do niej nieautoryzowanego dostępu z uprawnieniami zaatakowanego konta użytkownika.

## 2.3.9. Session Data Tampering

Modyfikacja danych sesji (ang. session data tampering) to technika, w której atakujący manipuluje zawartością danych sesji w celu uzyskania nieuprawnionego dostępu lub zmiany funkcjonalności aplikacji.

<p align="center">
  Rys.2.3.9.1. Działanie Session Data Tampering
<br>
  <img src="\assets\img\Cyber\47.png" width="650" alt="sdt">
  <br>
  Źródło: https://media.geeksforgeeks.org/wp-content/uploads/20220908163148/WebParameterTempering.jpg
</p>

Podczas ataku typu session data tampering, atakujący próbuje zmodyfikować dane przechowywane w sesji użytkownika, takie jak uprawnienia, identyfikatory sesji, dane użytkownika lub inne parametry, które wpływają na funkcjonowanie aplikacji. Celem ataku jest uzyskanie dostępu do informacji lub wykonanie nieautoryzowanych akcji w imieniu użytkownika.

### Atakujący może wykorzystać różne metody do manipulacji danych sesji, takie jak: 
+ Podstawienie danych – podmienianie danych przez atakującego 
+ Przechwycenie sesji – przechwytywanie identyfikatora sesji użytkownika przez atakującego
+ Ataki typu replay – przechwytywanie przez atakującego poprawnego żądania HTTP

## 2.3.10. Session Elevation

Atak podwyższenia sesji (ang. session elevation attack) to technika, w której atakujący próbuje uzyskać wyższe uprawnienia w kontekście sesji użytkownika, aby zyskać dostęp do funkcji lub danych, do których normalnie nie miałby uprawnień.

Podczas ataku podwyższenia sesji, atakujący wykorzystuje podatności lub luki w mechanizmach uwierzytelniania, autoryzacji lub zarządzania sesją, aby uzyskać dostęp do zasobów, których nie powinien mieć uprawnień. Atak taki może prowadzić do nieautoryzowanego dostępu do poufnych informacji, manipulacji danych, przejęcia kontroli nad sesją innego użytkownika lub wykonania akcji w imieniu użytkownika z wyższymi uprawnieniami.

### Przykłady ataków podwyższenia sesji
+ Atak polegający na przejęciu sesji administratora
+ Wykorzystanie podatności w mechanizmach autoryzacji
+ Przejście przez zaporę bezpieczeństwa

## 2.3.11. Session Impersonal

Atak podwyższenia sesji (session impersonation attack) to technika, w której atakujący próbuje przejąć kontrolę nad sesją innego użytkownika w celu uzyskania wyższych uprawnień lub dostępu do funkcji, do których normalnie nie ma dostępu.

Podczas ataku podwyższenia sesji, atakujący może wykorzystać podatności w mechanizmach uwierzytelniania, autoryzacji lub zarządzania sesją w celu podszywania się pod innego użytkownika. Celem ataku jest uzyskanie dostępu do informacji, wykonanie nieautoryzowanych akcji lub zmiana uprawnień użytkownika.

### Przykładowe metody ataku podwyższenia sesji
+ Przechwycenie identyfikatora sesji – atakujący przechwytuje identyfikator sesji innej osoby, na przykład poprzez podsłuchanie transmisji sieciowej lub wykorzystanie luki w zabezpieczeniach.
+ Atak typu session fixation – atakujący moze zainicjować sesję dla użytkownika, a następnie przekazać mu manipulowany identyfikator sesji. 
+ Manipulacja danymi sesji – atakujący próbuje zmienić zawartość danych przechowywanych w sesji, takich jka uprawnienia, role czy inne parametry, które wpływają na logikę aplikacji. 

## 2.3.12. Session Riding

Session Riding – jest to wysyłanie poleceń do aplikacji internetowej w imieniu docelowego użytkownika, po prostu wysylając mu wiadomość e-mail lub nakłaniając go do odwiedzenia specjalnie spreparowanej strony internetowej. 

### Jak działa Session Riding?

Przeglądarka wysyła plik cookie ustawiony przez stronę A przy każdym kolejnym żądaniu skierowanym do ośrodka A.

Jeśli przyjrzeć się temu mechanizmowi bardziej szczegółowo, należy spełnić więcej warunków: ścieżka, do której uzyskuje się dostęp, musi odpowiadać ścieżce, dla której zdefiniowano plik cookie, czas życia pliku cookie nie może wygasnąć itp. W większości przypadków możemy je zignorować poniższych rozważań, ponieważ nie są one krytycznymi elementami podstawowej zasady.

Załóżmy, że ta aplikacja używa plików cookie jako nośnika identyfikatora sesji. Załóżmy, że użytkownik pomyślnie się zalogował, więc plik cookie jest już ustawiony w jego przeglądarce. Następnie wypełnia formularz, aby złożyć ofertę:

<p align="center">
  Rys.2.3.12.1. Formularz
<br>
  <img src="\assets\img\Cyber\48.png" width="650" alt="formularz">
  <br>
  Źródło: https://crypto.stanford.edu/cs155old/cs155-spring08/papers/Session_Riding.pdf
</p>

Gdy użytkownik kliknie przycisk Prześlij, do serwera wysyłane jest żądanie (w tym przypadku żądanie GET), takie jak to poniżej:

<p align="center">
  Rys.2.3.12.2. Wysyłanie żądania
<br>
  <img src="\assets\img\Cyber\49.png" width="650" alt="zadanie">
  <br>
  Źródło: https://crypto.stanford.edu/cs155old/cs155-spring08/papers/Session_Riding.pdf
</p>

Plik cookie SESSIONID=123456789 jest automatycznie dodawany do żądania. Dzięki temu aplikacja jest w stanie rozpoznać użytkownika, potwierdzić, że wcześniej się uwierzytelnił i przeprowadzić transakcję na podstawie danych użytkownika, czyli złożyć ofertę na artykuł o nr. 1122 o wartości 100 EUR w imieniu użytkownika, który wcześniej się zalogował.

## 2.1.13. Session Revocation Bypass 

Ominięcie unieważnienia sesji (session revocation bypass) to technika, w której atakujący próbuje uzyskać dostęp do zasobów lub kontynuować aktywną sesję po unieważnieniu lub wygaśnięciu sesji użytkownika.

Unieważnienie sesji jest ważnym mechanizmem bezpieczeństwa, który pozwala zakończyć ważność sesji użytkownika, gdy użytkownik się wylogowuje lub występuje inna akcja wygaszająca sesję. Ominięcie unieważnienia sesji polega na wykorzystaniu luk w implementacji mechanizmu unieważniania sesji lub zaawansowanych technik, które pozwalają atakującemu na utrzymanie aktywnej sesji po jej unieważnieniu.

### Przykładowe metody omijania unieważnienia sesji to:
+ Utrzymanie aktywnego stanu sesji: Atakujący może manipulować danymi lub parametrami sesji, aby utrzymać jej aktywny stan po unieważnieniu. Na przykład, jeśli atakujący może kontrolować lub zmieniać identyfikator sesji, może nadal wykorzystywać tę samą sesję, nawet po wylogowaniu się użytkownika.
+ Wykorzystanie podatności w mechanizmach unieważniania sesji: Atakujący może znaleźć podatność w implementacji mechanizmu unieważniania sesji i wykorzystać ją do omijania procesu unieważnienia. Na przykład, atakujący może używać zmodyfikowanego identyfikatora sesji, który nie jest prawidłowo oznaczany jako unieważniony.
+ Przechwycenie sesji: Jeśli atakujący jest w stanie przechwycić identyfikator sesji lub uzyskać dostęp do aktywnej sesji innego użytkownika, może nadal korzystać z tej sesji nawet po unieważnieniu. Na przykład, jeśli atakujący przechwyci identyfikator sesji użytkownika, który wylogował się, może go użyć do uzyskania dostępu do konta użytkownika.

## 2.3.14. Man-in-the-Middle Attacks on Session Communication

Ataki typu Man-in-the-Middle (MitM) na komunikację sesji są technikami, w których atakujący podsłuchuje i przechwytuje komunikację między dwoma stronami, które nawiązały sesję, w celu przejęcia kontroli nad sesją lub pozyskania poufnych informacji.

Podczas ataku typu Man-in-the-Middle, atakujący umieszcza się pomiędzy dwoma komunikującymi się stronami, tworząc pozornie bezpieczne połączenie z każdą z nich. Atakujący może osiągnąć to poprzez różne metody, takie jak podsłuchy w sieci, ataki DNS spoofing, ataki ARP spoofing czy wykorzystanie bezprzewodowych punktów dostępowych.

Po umieszczeniu się pomiędzy komunikującymi się stronami, atakujący może monitorować całą komunikację między nimi, przechwytując wysyłane dane, w tym także sesje i identyfikatory sesji. Atakujący może również modyfikować przesyłane dane, wstrzykując własne pakiety lub zmieniając zawartość wysyłanych żądań.

### Przykładowe zagrożenia
+ Przechwycenie identyfikatora sesji: Atakujący może przechwycić identyfikator sesji wysyłany między klientem a serwerem, co umożliwia mu przejęcie kontroli nad sesją użytkownika.
+ Manipulacja danymi sesji: Atakujący może zmieniać przesyłane dane sesji, np. modyfikując wartości parametrów sesji, co może prowadzić do nieautoryzowanych akcji lub dostępu do chronionych zasobów.
+ Przechwycenie poufnych informacji: Atakujący może przechwytywać poufne dane przesyłane w trakcie komunikacji sesji, takie jak hasła, dane osobowe lub informacje finansowe.

## 2.4. Ataki warstwy transportowej

Atak na warstwę transportową to jedno z wielu zagrożeń, z jakimi spotykają się systemy komunikacyjne i sieci informatyczne. Warstwa transportowa jest jednym z pięciu poziomów modelu odniesienia OSI, który definiuje protokoły i mechanizmy służące do przesyłania danych między urządzeniami sieciowymi. Ataki na tę warstwę mają na celu wykorzystanie słabości w protokołach transportowych w celu zakłócenia lub przechwycenia transmisji danych.

## 2.4.1. Złamanie szyfrowania

Złamanie szyfrowania na warstwie transportowej oznacza naruszenie bezpieczeństwa protokołu komunikacyjnego na tym poziomie. Warstwa transportowa jest odpowiedzialna za zapewnienie niezawodnej i poufnej transmisji danych pomiędzy aplikacjami działającymi na różnych urządzeniach w sieci.

Najpopularniejszym protokołem transportowym jest protokół TCP (Transmission Control Protocol), który zapewnia niezawodną transmisję danych poprzez segmentację, numerowanie i potwierdzanie otrzymania pakietów. Protokół TCP nie oferuje jednak domyślnie szyfrowania, dlatego do zabezpieczenia transmisji można wykorzystać protokół SSL/TLS (Secure Sockets Layer/Transport Layer Security).

### Aby zapobiec złamaniu szyfrowania na warstwie transportowej, ważne jest:
+ Używanie silnych protokołów szyfrowania, takich jak TLS 1.2 lub TLS 1.3, i unikanie przestarzałych protokołów.
+ Regularne aktualizowanie oprogramowania i łatania zabezpieczeń w celu uniknięcia słabych punktów, które mogą być wykorzystane przez atakujących.
+ Uważne sprawdzanie i zarządzanie certyfikatami SSL/TLS oraz korzystanie z autoryzowanych dostawców certyfikatów.
+ Utrzymywanie świadomości na temat najnowszych zagrożeń i praktyk bezpieczeństwa oraz wdrażanie odpowiednich zabezpieczeń.

## 2.4.2. SYN Flood 

Atak SYN flood (atak półotwarty) to rodzaj ataku typu „odmowa usługi” (DDoS), którego celem jest uniemożliwienie dostępu do serwera legalnemu ruchowi poprzez wykorzystanie wszystkich dostępnych zasobów serwera. Wielokrotnie wysyłając pakiety początkowego żądania połączenia (SYN), osoba atakująca jest w stanie przeciążyć wszystkie dostępne porty na docelowej maszynie serwera, powodując, że docelowe urządzenie reaguje wolno lub wcale na prawidłowy ruch.

### Jak atak SYN flood działa? 

W normalnych warunkach połączenie TCP wykazuje trzy różne procesy w celu nawiązania połączenia: 
+ Najpierw klient wysyła pakiet SYN do serwera w celu zainicjowania połączenia.
+ Następnie serwer odpowiada na ten początkowy pakiet pakietem SYN/ACK w celu potwierdzenia komunikacji.
+ Na koniec klient zwraca pakiet ACK, aby potwierdzić otrzymanie pakietu z serwera. Po zakończeniu tej sekwencji wysyłania i odbierania pakietów połączenie TCP jest otwarte i może wysyłać i odbierać dane.

<p align="center">
  Rys.2.4.2.1. Działanie ataku SYN Flood
<br>
  <img src="\assets\img\Cyber\50.png" width="650" alt="synf">
  <br>
  Źródło: https://www.cloudflare.com/img/learning/ddos/syn-flood-ddos-attack/syn-flood-attack-ddos-attack-diagram-1.png
</p>

Aby wywołać atak typu „odmowa usługi”, atakujący wykorzystuje fakt, że po odebraniu początkowego pakietu SYN serwer odpowiada jednym lub kilkoma pakietami SYN/ACK i czeka na ostatni etap uzgadniania. 

### Oto jak to działa:
+ Atakujący wysyła dużą liczbę pakietów SYN do docelowego serwera, często ze sfałszowanymi adresami IP.
+ Następnie serwer odpowiada na każde żądanie połączenia i pozostawia otwarty port gotowy do odebrania odpowiedzi.
+ Podczas gdy serwer czeka na ostatni pakiet ACK, który nigdy nie dociera, atakujący kontynuuje wysyłanie kolejnych pakietów SYN. Nadejście każdego nowego pakietu SYN powoduje, że serwer tymczasowo utrzymuje połączenie z nowym otwartym portem przez określony czas, a po wykorzystaniu wszystkich dostępnych portów serwer nie może normalnie funkcjonować.

<p align="center">
  Rys.2.4.2.2. Przeprowadzanie ataku
<br>
  <img src="\assets\img\Cyber\51.png" width="650" alt="dos">
  <br>
  Źródło: https://www.cloudflare.com/img/learning/ddos/syn-flood-ddos-attack/syn-flood-attack-ddos-attack-diagram-2.png
</p>

SYN flood może wystapic na trzy sposoby: 
+ Direct attack – jest to tak SYN flood, w którym adres IP nie jest sfałszowany, nazywany jest atakiem bezpośrednim. W tym ataku atakujący w ogóle nie maskuje swojego adresu IP. W wyniku użycia przez osobę atakującą jednego urządzenia źródłowego z prawdziwym adresem IP do przeprowadzenia ataku, osoba atakująca jest bardzo narażona na wykrycie i ograniczenie zagrożeń. Aby stworzyć stan półotwarty na zaatakowanej maszynie, haker uniemożliwia swojej maszynie reagowanie na pakiety SYN-ACK serwera. Osiąga się to często za pomocą reguł zapory, które zatrzymują wychodzące pakiety inne niż pakiety SYN lub filtrując wszelkie przychodzące pakiety SYN-ACK, zanim dotrą one do komputera złośliwego użytkownika.
+ Spoofed attack – złośliwy użytkownik może również sfałszować adres IP w każdym wysyłanym pakiecie SYN, aby powstrzymać działania łagodzące i utrudnić wykrycie swojej tożsamości. Chociaż pakiety mogą być sfałszowane, potencjalnie można je prześledzić aż do ich źródła.
+ Distributed attack (DDoS) – jeśli atak jest tworzony przy użyciu botnetu, prawdopodobieństwo wyśledzenia ataku z powrotem do jego źródła jest niskie. Aby uzyskać dodatkowy poziom zaciemnienia, osoba atakująca może sprawić, że każde rozproszone urządzenie fałszuje również adresy IP, z których wysyła pakiety. Jeśli atakujący korzysta z botnetu, takiego jak botnet Mirai, generalnie nie będzie dbał o maskowanie adresu IP zainfekowanego urządzenia.

## 2.4.3. TCP/IP Hijacking

TCP/IP Hijacking – jest to atak sieciowy, w którym autoryzowany użytkownik może uzyskać dostęp do autoryzowanego połączenia sieciowego innego użytkownika lub klienta. Po przejęciu sesji TCP/IP atakujący może łatwo odczytać i zmodyfikować przesłane pakiety, a także może wysłać własne żądania do użytkownika. Do przejmowania kontroli nad TCP/IP napastnicy wykorzystują ataki DOS i fałszowanie adresów IP.

<p align="center">
  Rys.2.4.3.1. Działanie ataku TCP/IP Hijacking
<br>
  <img src="\assets\img\Cyber\52.png" width="650" alt="dos">
  <br>
  Źródło: https://media.geeksforgeeks.org/wp-content/uploads/20220718090253/Sender22.png
</p>

Proces TCP/IP Hijacking: 
+ Pierwszym głównym celem atakującego jest uzyskanie adresów IP dwóch urządzeń komunikujących się za pomocą tej samej sieci lub połączenia. W tym celu atakujący monitoruje transmisję danych w sieci do momentu uzyskania adresu IP urządzenia.
+ Po pomyślnym przechwyceniu adresu IP użytkownika hakerzy mogą łatwo zaatakować połączenie.
+ Aby uzyskać dostęp do połączenia, haker przerywa połączenie innego użytkownika poprzez atak DOS, a połączenie użytkownika czeka na ponowne połączenie.
+ Fałszując adres IP rozłączonego użytkownika, hakerzy mogą łatwo przywrócić komunikację.

## 2.4.4. UDP Flood

UDP flood – jest rodzaj ataku typu „odmowa usługi”, w którym duża liczba pakietów UDP (User Datagram Protocol) jest wysyłana do docelowego serwera w celu ograniczenia możliwości przetwarzania i reagowania na to urządzenie. Zapora chroniąca docelowy serwer może również zostać wyczerpana w wyniku zalewania UDP, co skutkuje odmową usługi dla legalnego ruchu.

### Jak atak UDP flood działa?

UDP flood działa głównie poprzez wykorzystanie kroków, które podejmuje serwer, gdy odpowiada na pakiet UDP wysłany do jednego z jego portów. W normalnych warunkach, gdy serwer odbiera pakiet UDP na określonym porcie, w odpowiedzi przechodzi przez dwa etapy:
+ Serwer najpierw sprawdza, czy są uruchomione programy, które obecnie nasłuchują żądań na określonym porcie.
+ Jeśli żaden program nie odbiera pakietów na tym porcie, serwer odpowiada pakietem ICMP (ping), aby poinformować nadawcę, że miejsce docelowe jest nieosiągalne.

<p align="center">
  Rys.2.4.4.1. Działanie UDP Flood
<br>
  <img src="\assets\img\Cyber\53.png" width="650" alt="udpf">
  <br>
  Źródło: https://www.cloudflare.com/img/learning/ddos/udp-flood-ddos-attack/amplification-ddos-attack-metaphor.png
</p>

Gdy każdy nowy pakiet UDP jest odbierany przez serwer, przechodzi przez kolejne kroki w celu przetworzenia żądania, wykorzystując w tym procesie zasoby serwera. Podczas przesyłania pakietów UDP każdy pakiet będzie zawierał adres IP urządzenia źródłowego. Podczas tego typu ataku DDoS osoba atakująca na ogół nie używa własnego prawdziwego adresu IP, ale zamiast tego sfałszuje źródłowy adres IP pakietów UDP, uniemożliwiając ujawnienie prawdziwej lokalizacji osoby atakującej i potencjalne nasycenie pakietami odpowiedzi z atakowanego serwer.
Ponieważ docelowy serwer wykorzystuje zasoby do sprawdzania, a następnie odpowiadania na każdy odebrany pakiet UDP, zasoby docelowego mogą zostać szybko wyczerpane po odebraniu dużej ilości pakietów UDP, co skutkuje odmową usługi dla normalnego ruchu.

<p align="center">
  Rys.2.4.4.2. Działanie UDP Flood
<br>
  <img src="\assets\img\Cyber\54.png" width="650" alt="udpf-1">
  <br>
  Źródło: https://www.cloudflare.com/img/learning/ddos/udp-flood-ddos-attack/udp-flood-attack-ddos-attack-diagram.png
</p>

## 2.4.5. Reflective Amplification

Atak Reflective Amplification polega na tym, że atakujący fałszuje adres IP celu i wysyła żądanie informacji, głównie przy użyciu protokołu UDP lub w niektórych przypadkach protokołu TCP. Następnie serwer odpowiada na żądanie wysyłając odpowiedź na adres IP celu. 

Ataki amplification generują dużą liczbę pakietów, które są wykorzystywane do przytłoczenia docelowej witryny internetowej bez alarmowania pośrednika. Dziej się tak, gdy podatna na ataki usługa odpowiada dużą odpowiedzią, gdy atakujący wysyła swoje żądanie, często nazywane “pakietem wyzwalającym”. Korzystając z łatwo dostępnych narzędzi, osoba atakująca jest w stanie wysłać wiele tysięcy takich żądań do wrażliwych usług, powodując w ten sposób odpowiedzi, które są znacznie większe niż pierwotne żądanie i znacznie zwiększając rozmiar i przepustowość wysyłane do celu.

<p align="center">
  Rys.2.4.5.1. Działanie ataku Reflective
<br>
  <img src="\assets\img\Cyber\55.png" width="650" alt="reflective">
  <br>
  Źródło: https://www.educative.io/answers/what-are-reflection-and-amplification-attacks
</p>

Atak wzmacniający również należy do kategorii ataków typu „odmowa usługi” (DoS): 
+ Współczynnik wzmocnienia jest utrzymywany na jak najwyższym poziomie.
+ Atakujący generuje dużą liczbę pakietów, które zalewają witrynę ofiary bez alarmowania pośrednika.
+ Atakujący wykorzystuje publicznie dostępny protokół UDP i wysyła „pakiet wyzwalający”, którego wynikiem jest obszerna odpowiedź na żądanie.
+ Równocześnie generowanych jest kilka żądań obsługiwanych przez różne podatne na ataki usługi. Atakujący może to zrobić lub użyć botnetu.
+ Zwiększa to rozmiar odpowiedzi pierwotnego żądania i pochłania ogromną przepustowość ofiary.

<p align="center">
  Rys.2.4.5.2. Działanie ataku Amplification 
<br>
  <img src="\assets\img\Cyber\56.png" width="650" alt="amplification">
  <br>
  Źródło: https://educative.io/answers/what-are-reflection-and-amplification-attacks
</p>

## 2.4.6. TCP Reset Attack

TCP Reset Attack to rodzaj ataku, w którym atakujący wysyłają do hosta sfałszowane pakiety TCP RST (Reset).  Jest to najczęstszy atak w Internecie, który powoduje wiele problemów. Ataki te są przeprowadzane głównie w celu zamknięcia stron internetowych, które z nimi nie współpracują. Atak ten można również przeprowadzić w celu przeprowadzenia rozproszonego ataku typu „odmowa usługi” (ataku DDoS).

### Jak TCP Reset Attack działa? 
+ Kiedy połączenie TCP jest ustanawiane między dwoma komputerami, komputer wysyłający wysyła pakiet TCP RST (Reset) do komputera odbierającego.
+ Przed wysłaniem pakietu TCP RST (Reset) komputer wysyłający najpierw sprawdza, czy komputer odbierający faktycznie nasłuchuje komunikacji, czy nie.
+ Jeśli komputer odbierający nie nasłuchuje komunikacji, komputer wysyłający wysyła pakiet TCP RST (Reset) do komputera odbierającego.
+ Ten pakiet TCP RST (Reset) jest zwykle wysyłany, gdy komputer odbierający nie wysyła potwierdzenia przez pewien czas.
+ Jeśli komputer odbierający faktycznie nasłuchuje komunikacji, komputer wysyłający nie wyśle pakietu TCP RST (Reset) do komputera odbierającego
+ Zamiast tego komputer wysyłający wyśle pakiet TCP RST (Reset) do komputera wysyłającego.
+ Ale w ataku resetowania protokołu TCP komputer wysyłający wysyła pakiet TCP RST (Reset) do komputera odbierającego.

<p align="center">
  Rys.2.4.6.1. Działanie ataku TCP Reset
<br>
  <img src="\assets\img\Cyber\57.png" width="650" alt="tcpreset">
  <br>
  Źródło: https://assets.website-files.com/5ff66329429d880392f6cba2/60a4fdf7a4cd57ac6da7fe11_Syn%20Spoofing%20attack.png
</p>

## 2.4.7. Port Scanning 

Port Scanning – jest to technika wykorzystywana przez hakerów do wykrywania otwartych drzwi lub słabych punktów w sieci. Kiedy hakerzy wysyłają wiadomość do portu, otrzymana odpowiedź określa czy port jest używany i czy istnieją potencjalne słabe punkty, które można wykorzystać. 

### Skanowanie portów może dostarczyć takich informacji jak: 
+ Usługi, które są uruchumione
+ Użytkownicy, którzy są anonimowe logowania
+ Czy dozwolone są anonimowe logowania
+ Które usługi sieciowe wymagaja uwierzytelnienia

### Techniki skanowania portów:
+ Skanowanie ping – jest to technika, która wysyła grupę kilku żądań ICMP do różnych serwerów w celu uzyskania odpowiedzi. Skanowanie ping może być używane przez administratora do rozwiązywania problemów, a ping może być blokowany i wyłączany przez zaporę ogniową.
+ Skanowanie vanilla – jest to technikia, która próbuje połączyć się ze wszystkimi 65 536 portami w tym samym czasie. Wysyła flagę synchronizacji (SYN) lub żądanie połączenia. Kiedy otrzymuje odpowiedź SYN-ACK lub potwierdzenie połączenia, odpowiada flagą ACK.
+ Skanowanie SYN – jest to skanowanie półotwarte, które wysyła flagę SYN do celu i czeka  na odpowiedź SYN-ACK. W przypadku odpowiedzi skaner nie odpowiada, co oznacza, że połączenie TCP nie zostało zakończone. Dlatego interakcja nie jest rejestrowana, ale nadawca dowiaduje się, czy port jest otwarty.
+ Skany XMAS i FIN – ten typ skanowania wysyła zestaw flag, które po udzieleniu odpowiedzi mogą ujawnić wgląd w zaporę ogniową i stan portów. Skanowanie FIN polega na tym, że osoba atakująca wysyła flagę FIN, często używaną do zakończenia ustanowionej sesji, do określonego portu. Reakcja systemu na to może pomóc atakującemu zrozumieć poziom aktywności i zapewnić wgląd w wykorzystanie zapory sieciowej w organizacji.
+ Skanowanie odyłaczy FTP – ta technika umożliwia nadawcy ukrycie swojej lokalizacji za pomocą serwera FTP w celu odbicia pakietu.
+ Sweep skanowanie – ta technika skanowania portów wysyła ruch do portu przez kilka komputerów w sieci, aby zidentyfikować te, które są aktywne. Nie udostępnia żadnych informacji o aktywności portu, ale informuje nadawcę, czy jakieś systemy są w użyciu.

<p align="center">
  Rys.2.4.7.1. Techniki Port Scanning
<br>
  <img src="\assets\img\Cyber\58.png" width="650" alt="portscanning">
  <br>
  Źródło: https://www.fortinet.com/resources/cyberglossary/what-is-port-scan/_jcr_content/par/c05_container_copy/par/c28_image.img.jpg/1667849404946.jpg
</p>

### Rodzaje Port Chcecker albo Scanner:
+ Ping skanowanie – polecenie ping służy do sprawdzenia, czy pakiet danych sieciowych może dotrzeć do adresu IP bez żadnych problemów
+ Half-open or SYNC scans – ten rodzaj skanowania po prostu przesyła wiadomość SYN i nie kończy połączenia z odbiorcą.
+ XMAS skanowanie – skany XMAS wysyłają pewną liczbę pakietów do portu, aby sprawdzić, czy jest on otwarty. Jeśli port jest zamknięty, skaner otrzymuje odpowiedź. Jeśli nie otrzyma odpowiedzi, oznacza to, że port jest otwarty i można go użyć do uzyskania dostępu do sieci.

## 2.4.8. Man-in-the-Middle Attacks on Transport Layer

Man-in-the-Middle (MitM) – to rodzaj cyberataku, w którym osoba atakująca przechwytuje i manipuluje komunikacją między dwiema stronami. Może to pozwolić atakującemu na podsłuchiwanie rozmowy, zmianę wymienianych wiadomości lub podszywanie się pod jedną ze stron w celu uzyskania dostępu do poufnych informacji.

Na przykład osoba atakująca może przechwycić wiadomości przesyłane między klientem a serwerem, a następnie zmienić te wiadomości w celu kradzieży poufnych informacji lub uzyskania dostępu do serwera.

Ataki MitM sa często do wykrycia, ponieważosoba atakująca zasadniczo “siedzi w środku” komunikacji między dwiema stronami i może manipulować wiadomościami bez wiedzy żadnej ze stron. 

<p align="center">
  Rys.2.4.8.1. Działanie ataku MitM 
<br>
  <img src="\assets\img\Cyber\59.png" width="650" alt="mitm">
  <br>
  Źródło: https://www.imperva.com/learn/wp-content/uploads/sites/13/2017/09/man-in-the-middle-mitm-attack.png.webp
</p>

### Jak atak Man-in-the-Middle działa?
+ Atakujący przechwytuje komunikację między klientem a serwerem. Można to zrobić za pomocą różnych środków, takich jak użycie złośliwego urządzenia sieciowego lub złamanie zabezpieczeń routera lub przełącznika sieciowego.
+ Następnie atakujący manipuluje komunikacją między klientem a serwerem. Może to obejmować zmianę wymienianych wiadomości, przekierowanie ruchu do innego miejsca docelowego lub podszywanie się pod jedną ze stron w celu uzyskania dostępu do poufnych informacji.
+ Klient i serwer nie są świadomi, że atakujący przechwytuje i manipuluje ich komunikacją. W rezultacie nadal komunikują się ze sobą w normalny sposób, a atakujący może uzyskać dostęp do poufnych informacji lub zakłócić komunikację między nimi.

### Technika MitM:
+ ARP spoofing – w tej technice atakujący wysyła fałszywe komunikaty protokołu ARP do sieci, powodując, że urządzenia w sieci aktualizują swoje pamięci podręczne ARP niepoprawnymi informacjami. Pozwala to atakującemu przechwycić ruch między dwoma urządzeniami, kierując go przez własne urządzenie.
+ DNS spoofing – w tej technice osoba atakująca manipuluje rekordami systemu nazw domen (DNS) witryny internetowej, przekierowując użytkowników do złośliwej witryny, która wygląda na legalną. Pozwala to atakującemu na kradzież poufnych informacji od niczego niepodejrzewających użytkowników, takich jak dane logowania.
+ SSL stripping – w tej technice osoba atakująca obniża poziom bezpiecznego połączenia HTTPS między klientem a serwerem do niezabezpieczonego połączenia HTTP. Pozwala to atakującemu przeglądać i modyfikować dane wymieniane między klientem a serwerem, co pozwala na kradzież poufnych informacji lub uzyskanie nieautoryzowanego dostępu do serwera.
+ Packet injection – w tej technice atakujący wstrzykuje złośliwe pakiety do sieci, zakłócając komunikację między dwoma urządzeniami i umożliwiając atakującemu uzyskanie dostępu do poufnych informacji lub zakłócenie działania sieci.

## 2.4.9. Denial of Service Attacks on Transport Layer

Ataki typu Denial of Service (DoS) na warstwie transportowej (Transport Layer) są metodą, w której przeciwnik próbuje sparaliżować lub uniemożliwić prawidłowe funkcjonowanie usług sieciowych poprzez przeciążenie warstwy transportowej protokołu komunikacyjnego.

Ataki DoS na warstwie transportowej koncentrują się na wykorzystaniu podatności w protokołach takich jak TCP (Transmission Control Protocol) i UDP (User Datagram Protocol), które są odpowiedzialne za przekazywanie danych między aplikacjami w sieci.

Przykładem ataku DoS na warstwie transportowej może być atak SYN flood. W tym przypadku, atakujący wysyła duże ilości żądań połączenia TCP do celu, ale nie finalizuje procesu nawiązywania połączenia poprzez przesłanie potwierdzenia (ACK). W rezultacie cel musi przechowywać otwarte sesje, co prowadzi do wyczerpania zasobów i uniemożliwia nawiązanie nowych, prawidłowych połączeń TCP.

Innym przykładem jest atak UDP flood, który polega na przesyłaniu ogromnej liczby pakietów UDP do celu. Ponieważ protokół UDP nie wymaga potwierdzania dostarczenia pakietów, atakujący może wysłać wiele fałszywych pakietów, co prowadzi do przeciążenia zasobów systemowych.
Ataki DoS na warstwie transportowej mają na celu uniemożliwienie użytkownikom korzystania z usług sieciowych, co może prowadzić do zakłóceń w działaniu serwisów online, a nawet prowadzić do poważnych strat finansowych dla firm lub organizacji.

## 2.4.10. Blind SQL Injection

Blind SQL Injection – to rodzaj wstrzyknięcia SQL, w którym atakujący nie otrzymuje oczywistej odpowiedzi z atakowanej bazy danych i zamiast tego rekonstruuje strukturę bazy danych krok po kroku, obserwując zachowanie serwera bazy danych i aplikacji.

### Istnieją dwa rodzaje ślepych iniekcji SQL: 
+ Oparte na wartościach logicznych (boolean-based blind):

Jako przykład załóżmy, że poniższe zapytanie ma na celu wyświetlenie szczegółów produktu z bazy.

~~~
SELECT * FROM products WHERE id = product_id
~~~

Najpierw złośliwy haker używa aplikacji w legalny sposób, aby wykryć co najmniej jeden istniejący identyfikator produktu — w tym przykładzie jest to produkt 42. Następnie może podać następujące dwie wartości dla product_id:

~~~
42 AND 1=1
42 AND 1=0
~~~

Jeśli to zapytanie jest wykonywane w aplikacji przy użyciu prostej konkatenacji łańcuchów, zapytanie staje się odpowiednio:

~~~
SELECT * FROM products WHERE id = 42 and 1=1
SELECT * FROM products WHERE id = 42 and 1=0
~~~

Jeśli aplikacja zachowuje się inaczej w każdym przypadku, jest podatna na ślepe iniekcje SQL oparte na wartościach boolowskich.

Jeśli serwerem bazy danych jest Microsoft SQL Server, osoba atakująca może teraz podać następującą wartość parametru product_id:

~~~
42 AND (SELECT TOP 1 substring(name, 1, 1)
  FROM sysobjects
  WHERE id=(SELECT TOP 1 id
    FROM (SELECT TOP 1 id
      FROM sysobjects
      ORDER BY id)
    AS subq
    ORDER BY id DESC)) = 'a'
~~~

W rezultacie podzapytanie w nawiasach po 42 AND sprawdza, czy nazwa pierwszej tabeli w bazie zaczyna się na literę a. Jeśli to prawda, aplikacja będzie zachowywać się tak samo, jak dla ładunku 42 AND 1=1. Jeśli false, aplikacja będzie zachowywać się tak samo, jak dla ładunku 42 AND 1=0.

Atakujący może iterować przez wszystkie litery, a następnie przejść do drugiej litery, trzeciej litery itd. W rezultacie atakujący może odkryć pełną nazwę pierwszej tabeli w strukturze bazy danych. Następnie mogą spróbować uzyskać więcej danych o strukturze tej tabeli i ostatecznie – wyodrębnić dane z tabeli. Chociaż ten przykład jest specyficzny dla MS SQL, podobne techniki istnieją dla innych typów baz danych.

+ Oparte na czasie (time-based blind) – atakujący obserwuje zachowanie serwera bazy danych i aplikacji po połączeniu prawidłowych zapytań z poleceniami SQL powodującymi opóźnienia.

### Przykłady time-based blind SQL Injection:
~~~
SELECT * FROM products WHERE id = product_id
~~~

Złośliwy haker może podać następującą wartość product_id:
~~~
42; WAITFOR DELAY '0:0:10'
~~~

W rezultacie zapytanie staje się:
~~~
SELECT * FROM products WHERE id = 1; WAITFOR DELAY '0:0:10'
~~~

Jeśli serwerem bazy danych jest Microsoft SQL Server, a aplikacja jest podatna na oparte na czasie ślepe iniekcje SQL, osoba atakująca zobaczy 10-sekundowe opóźnienie w aplikacji.

Teraz, gdy atakujący wie, że możliwe są ślepe iniekcje SQL oparte na czasie, może podać następujący product_id:
~~~
42; IF(EXISTS(SELECT TOP 1 *
  FROM sysobjects
  WHERE id=(SELECT TOP 1 id
    FROM (SELECT TOP 1 id 
      FROM sysobjects 
      ORDER BY id) 
    AS subq
    ORDER BY id DESC)
  AND ascii(lower(substring(name, 1, 1))) = 'a'))
  WAITFOR DELAY '0:0:10'
~~~

Jeżeli nazwa pierwszej tabeli w strukturze bazy zaczyna się na literę a, to druga część tego zapytania będzie prawdziwa, a aplikacja zareaguje z 10-sekundowym opóźnieniem. Podobnie jak w przypadku ślepych iniekcji SQL opartych na wartościach boolowskich powyżej, osoba atakująca może użyć tej metody wielokrotnie, aby odkryć nazwę pierwszej tabeli w strukturze bazy danych, a następnie spróbować uzyskać więcej danych o strukturze tej tabeli i ostatecznie wyodrębnić dane z tabela.

## 2.4.11. 

TCP/IP Sequence Number Attack – to technika używana do wykrywania złośliwych działań w sieci. Działa poprzez analizę numerów sekwencyjnych pakietów wysyłanych przez sieć i przewidywanie następnego numeru sekwencyjnego. Pomaga to wykryć wszelkie złośliwe działania, które mogą występować w sieci. Technika ta służy do wykrywania i zapobiegania atakom typu spoofing, hijacking i denial of service.

<p align="center">
  Rys.2.4.11.1. TCP/IP Sequence Number Attacks
<br>
  <img src="\assets\img\Cyber\60.png" width="650" alt="sna">
  <br>
  Źródło: https://www.tech-faq.com/wp-content/uploads/TCP-Sequence-Prediction-Attack.gif
</p>

### Jak TCP Sequence Number działa?

Przewidywanie numerów sekwencyjnych TCP polega na analizie numerów sekwencyjnych pakietów wysyłanych przez sieć i przewidywaniu kolejnego numeru sekwencyjnego. Pomaga to wykryć wszelkie złośliwe działania, które mogą występować w sieci. Technika ta polega na analizie numerów sekwencyjnych pakietów wysyłanych przez sieć i przewidywaniu następnego numeru sekwencyjnego. Pomaga to wykryć wszelkie złośliwe działania, które mogą występować w sieci.

## 2.4.12. Teardrop Attack 

Teardrop attack – to rodzaj ataku typu “odmowa usługi”. Osoba atakująca wysyła pofragmentowane pakiety do serwera docelowego, a w niektórych przypadkach, gdy występuje luka w zabezpieczeniach TCP/IP, serwer nie może ponownie złożyć pakietu, co powoduje przeciążenie.

<p align="center">
  Rys.2.4.12.1. Atak Teardrop
<br>
  <img src="\assets\img\Cyber\61.png" width="650" alt="sna">
  <br>
  Źródło: https://www.cloudns.net/blog/wp-content/uploads/2022/12/How-does-Teardrop-attack-work-1024x576.png
</p>

### Jak działa? 

Implementacje TCP/IP różnią się nieznacznie w zależności od platformy. Niektóre systemy operacyjne — zwłaszcza starsze wersje systemów Windows i Linux — zawierają błąd ponownego montażu fragmentacji TCP/IP. Ataki teardrop mają na celu wykorzystanie tej słabości. W tym ataku klent wysyła celowo pofragmentowany pakiet informacyjny do urządzenia docelowego. Ponieważ pakiety nakładają się, błąd występuje, gdy urządzenie próbuje ponownie złożyć pakiet. Atak wykorzystuje ten błąd, aby spowodować awarię krytyczną w systemie operacyjnym lub aplikacji obsługującej pakiet.

## 2.4.13. TCP/IP Fragmentation Attacks

TCP/IP Fragmentations Attack – jest to atak, w którym sprawca przejmuje kontrolę nad siecią, wykorzystując mechanizmy fragmentacji datagramów.

<p align="center">
  Rys.2.4.13.1. Atak TCP/IP Fragmentation i Reassembly
<br>
  <img src="\assets\img\Cyber\62.png" width="650" alt="fir">
  <br>
  Źródło: https://www.imperva.com/learn/wp-content/uploads/sites/13/2019/01/ip-fragmentation.jpeg.webp
</p>

### Typy ataków:
+ Ataki fragmentacji UDP i ICMP – ataki te obejmują transmisję fałszywych pakietów UDP lub ICMP, które są większe niż MTU sieci. Ponieważ pakiety te są fałszywe i nie można ich ponownie złożyć, zasoby serwera docelowego są szybko zużywane, co powoduje niedostępność serwera.
+ Ataki fragmentacji TCP – ataki te, znane również jako ataki Teardrop, są wymierzone w mechanizmy ponownego składania TCP/IP, uniemożliwiając im łączenie pofragmentowanych pakietów danych. W rezultacie pakiety danych nakładają się na siebie i szybko przytłaczają serwery ofiary, powodując ich awarię.

## 2.5. Ataki warstwy sieciowej

Ataki na warstwie sieciowej, nazywane również atakami na sieć, to próby naruszenia lub zakłócenia normalnego działania sieci komputerowej. Warstwa sieciowa odnosi się do drugiej warstwy modelu OSI (Open Systems Interconnection), a jej głównym zadaniem jest zapewnienie komunikacji między różnymi hostami w sieci.

## 2.5.1. IP Spoofing

IP Spoofing polega na tworzeniu pakietów protokołu internetowego (IP), które maja zmodyfikowany adres źródłowy w celu ukrycia tożsamości nadawcy, podszywania się pod inny system komputerowy lub obu tych elementów. Jest to technika często wykorzystywana przez złych aktorów do wywoływania ataków DDoS na docelowe urządzenia lub otaczają infrastukturę. 

<p align="center">
  Rys.2.5.1.1. IP Spoofing attack
<br>
  <img src="\assets\img\Cyber\63.png" width="650" alt="ips">
  <br>
  Źródło: https://www.cloudflare.com/img/learning/ddos/glossary/ip-spoofing/ip-spoofing.png
</p>

Fałszowanie adresów IP jest analogiczne do sytuacji, w której osoba atakująca wysyła paczkę do osoby z nieprawidłowym adresem zwrotnym. Jeśli osoba odbierająca paczkę chce powstrzymać nadawcę przed wysyłaniem paczek, zablokowanie wszystkich paczek z fałszywego adresu niewiele pomoże, ponieważ adres zwrotny można łatwo zmienić. W związku z tym, jeśli odbiorca chce odpowiedzieć na adres zwrotny, jego pakiet odpowiedzi trafi gdzie indziej niż do prawdziwego nadawcy. Możliwość fałszowania adresów pakietów jest podstawową luką wykorzystywaną przez wiele ataków DDoS.

## 2.5.2. ICMP Flood

Jest to atak, w którym osoba atakująca próbuje przeciążyć docelowe urządzenia pakietami żądań echa ICMP, powodując, że cel staje się niedostępny dla normalnego ruchu. Gdy ruch ataku pochodzi z wielu urządzeń, atak staje się atakiem DDoS lub rozproszonym atakiem “odmowa usługi”. 

### Jak działa atak ICMP Flood?
+ Osoba atakująca wysyła wiele pakietów żądania echa ICMP do docelowego serwera przy użyciu wielu urządzeń.
+ Następnie serwer docelowy wysyła pakiet odpowiedzi echa ICMP na adres IP każdego żądającego urządzenia jako odpowiedź.

<p align="center">
  Rys.2.5.2.1. Działanie ataku ICMP Flood
<br>
  <img src="\assets\img\Cyber\64.png" width="650" alt="icmpf">
  <br>
  Źródło: https://www.cloudflare.com/img/learning/ddos/ping-icmp-flood-ddos-attack/ping-icmp-flood-ddos-attack-diagram.png
</p>

## 2.5.3. Smurf Attack

Smurf Attack to rozproszony atak typu “odmowa usługi”, w którym osoba atakująca próbuje zalać atakowany serwer pakietami ICMP. Wysyłając żądania ze sfałszowanym adresem IP docelowego urządzenia do jednej lub więcej sieci komputerowych, sieci komputerowe odpowiadają następnie atakowanemu serwerowi, wzmacniając początkowy ruch ataku i potencjalnie przytłaczając cel, czyniąc go niedostępnym.

### Jak działa Smurf Attack?
+ Najpierw szkodliwe oprogramowanie Smerf buduje sfałszowany pakiet, którego adres źródłowy jest ustawiony na prawdziwy adres IP atakowanej ofiary.
+ Pakiet jest następnie wysyłany na adres rozgłoszeniowy IP routera lub zapory, który z kolei wysyła żądania do każdego adresu urządzenia hosta sieci nadawczej, zwiększając liczbę żądań o liczbę urządzeń sieciowych w sieci.
+ Każde urządzenie w sieci odbiera żądanie od nadawcy, a następnie odpowiada na sfałszowany adres celu pakietem ICMP Echo Respond.
+ Docelowa ofiara otrzymuje następnie zalew pakietów ICMP Echo Respond, potencjalnie przytłoczony i powodujący odmowę usługi dla legalnego ruchu.

### Rodzaje ataków Smurf Attack:
+ Basic Smurf Attack – występuje, gdy atakujący zalewa sieć docelową nieskończoną liczbą pakietów żądań ICMP. Pakiety zawierają adres źródłowy ustawiony na adres rozgłoszeniowy sieci, który monituje każde urządzenie w sieci, które odbiera żądanie, o udzielenie odpowiedzi. Powoduje to ogromny ruch, który ostatecznie usunie system.
+ Advanced Smurf Attack – ten atak rozpoczyna się jako atak podstawowy. Jednak żądania echa są w stanie skonfigurować źródła, aby mogły odpowiadać na dodatkowe ofiary stron trzecich. Dzięki temu atakujący mogą atakować wiele ofiar jednocześnie, co oznacza, że mogą spowolnić bardziej rozbudowane sieci i atakować większe grupy ofiar i większe sekcje sieci.
+ Smurf Attack Transmission end Effects


## 2.5.4. Ping of Death

Ping of Death to atak, w którym osoba atakująca ma na celu zakłócenie działania docelowej maszyny poprzez wysłanie pakietu większego niż maksymalny dopuszczalny rozmiar, powodując zamrożenie lub awarię komputera docelowego. 

### Jak działa ping of death?
<p align="center">
  Rys.2.5.4.1. Działanie ataku Ping of Death
<br>
  <img src="\assets\img\Cyber\65.png" width="650" alt="icmpf">
  <br>
  Źródło: https://www.cloudflare.com/img/learning/ddos/ping-of-death-ddos-attack/attack-mitigation.png
</p>

Gdy złośliwie duży pakiet jest przesyłany od osoby atakującej do celu, zostaje on podzielony na segmenty, z których każdy jest poniżej maksymalnego limitu rozmiaru. Gdy komputer docelowy próbuje ponownie połączyć elementy, suma przekracza limit rozmiaru i może wystąpić przepełnienie bufora, powodując zamrożenie, awarię lub ponowne uruchomienie komputera docelowego.

Podczas gdy echo ICMP może zostać wykorzystane do tego ataku, wszystko, co wysyła datagram IP, może zostać wykorzystane do tego exploita. Obejmuje to transmisje TCP, UDP i IPX.

## 2.5.5. Fragmentation Attack

Fragmentation Attack – jest to rodzaj ataku typu “odmowa usługi”, którego celem jest zakłócenie komunikacji poprzez fragmentację pakietów. Bombardując cel pofragmentowanymi pakietami, atakujący może przeciążyć zdolność celu do ponownego złożenia pakietów, uniemożliwiając mu skuteczną komunikację. 

### Typy Fragmentation attack: 
+ Bezpołączeniowy atak na fragment pakietu – atakujący wysyła pofragmentowane pakiety do ofiary bez uprzedniego nawiązania połączenia. System ofiary ponownie złoży pakiety, ale ponieważ są one niesprawne, dane zostaną uszkodzone.
+ Atak na fragment pakietów zorientowany na połączenie – osoba atakująca najpierw nawiązuje połączenie z ofiarą, a następnie wysyła pofragmentowane pakiety. System ofiary ponownie złoży pakiety, ale ponieważ są one niesprawne, dane zostaną uszkodzone.
+ Atak fragmentów pakietów w warstwie aplikacji – osoba atakująca wysyła do ofiary pofragmentowane pakiety, które zostały specjalnie zaprojektowane do wykorzystania luk w protokołach warstwy aplikacji. System ofiary ponownie złoży pakiety, ale ponieważ są one niesprawne, dane zostaną uszkodzone.
+ Atak fragmentów pakietów warstwy transportowej – osoba atakująca wysyła do ofiary pofragmentowane pakiety, które zostały specjalnie zaprojektowane w celu wykorzystania luk w protokołach warstwy transportowej. System ofiary ponownie złoży pakiety, ale ponieważ są one niesprawne, dane zostaną uszkodzone.

### Jak działa atak fragmentowany?
Gdy haker wysyła wiele małych pakietów danych do komputera docelowego, może przeciążyć system i spowodować jego awarię. Nazywa się to atakiem fragmentacji.

Ataki fragmentacji wykorzystują fakt, że większość systemów komputerowych ma ograniczoną ilość pamięci do przechowywania przychodzących danych. Gdy zbyt wiele danych dociera na raz, system nie może sobie poradzić i zaczyna fragmentować lub dzielić dane na mniejsze kawałki. Proces ten zużywa cenne zasoby, co może ostatecznie doprowadzić do awarii systemu.

Istnieją dwa główne typy ataków fragmentacyjnych: bezpośredni i pośredni. Ataki z bezpośrednią fragmentacją wysyłają małe pakiety danych bezpośrednio do systemu docelowego, podczas gdy ataki fragmentacji pośredniej najpierw wysyłają duże pakiety danych do systemu pośredniczącego, a następnie przekazują je do systemu docelowego.

## 2.5.6. Land Attack

Land Attack – to atak, w którym osoba atakująca ustawia informacje o źródle i miejscu docelowym segmentu TCP na takie same. Podatna na atak maszyna ulegnie awarii lub zamarznie z powodu wielokrotnego przetwarzania pakietu przez stos TCP. 

W ataku LAND tworzony jest specjalnie spreparowany pakiet TCP SYN w taki sposób, że źródłowy adres IP i port są ustawione na taki sam jak adres docelowy i port, który z kolei wskazuje otwarty port na komputerze ofiary. Podatna na ataki maszyna odebrałaby taką wiadomość i odpowiedziałaby na adres docelowy, skutecznie wysyłając pakiet do ponownego przetworzenia w nieskończonej pętli. W ten sposób procesor maszyny jest zużywany w nieskończoność, zamrażając podatną na ataki maszynę, powodując blokadę, a nawet jej awarię.

## 2.5.7. DNS Spoofing

DNS Spoofing to atak, w którym zmienione rekordy DNS są wykorzystywane do przekierowywania ruchu online do fałszywej witryny internetowej przypominającej zamierzone miejsce docelowe. 

Tam użytkownicy są proszeni o zalogowanie się na swoje konto, dając sprawcy możliwość kradzieży danych uwierzytelniających i innych rodzajów poufnych informacji. Ponadto szkodliwa strona internetowa jest często wykorzystywana do instalowania robaków lub wirusów na komputerze użytkownika, dając sprawcy długoterminowy dostęp do niej i przechowywanych danych.

### Metody przeprowadzania ataku DNS z fałszowaniem obejmują:
+ Man-in-the-Middle (MitM)
+ DNS server compromise

<p align="center">
  Rys.2.5.7.1. Działanie ataku DNS Spoofing
<br>
  <img src="\assets\img\Cyber\66.png" width="650" alt="dnss">
  <br>
  Źródło: https://www.imperva.com/learn/wp-content/uploads/sites/13/2019/01/DNS-spoofing.jpg.webp
</p>

### Przykład zatruwania pamięci podręcznej DNS

Poniższy przykład ilustruje atak polegający na zatruwaniu pamięci podręcznej DNS, w którym osoba atakująca (IP 192.168.3.300) przechwytuje kanał komunikacyjny między klientem (IP 192.168.1.100) a komputerem serwera należącym do www.estores.com witryny sieci Web (IP 192.168.2.200).

W tym scenariuszu narzędzie (np. arpspoof) jest używane do oszukania klienta, aby myślał, że adres IP serwera to 192.168.3.300. Jednocześnie serwer jest zmuszony myśleć, że IP klienta to również 192.168.3.300.

### Taki scenariusz przebiegałby następująco:
+ Osoba atakująca używa arpspoof do wydania polecenia: arpspoof 192.168.1.100 192.168.2.200. Powoduje to modyfikację adresów MAC w tabeli ARP serwera, powodując, że komputer osoby atakującej należy do klienta.
+ Atakujący po raz kolejny używa arpspoof do wydania polecenia: arpspoof 192.168.2.200 192.168.1.100, które informuje klienta, że komputer sprawcy jest serwerem.
+ Atakujący wydaje polecenie Linux: echo 1> /proc/sys/net/ipv4/ip_forward. W rezultacie pakiety IP przesyłane między klientem a serwerem są przekazywane do komputera sprawcy.
+ Plik hosta 192.168.3.300 estores.com jest tworzony na komputerze lokalnym osoby atakującej, który mapuje witrynę sieci Web www.estores.com na jej lokalny adres IP.
+ Sprawca konfiguruje serwer WWW na adresie IP komputera lokalnego i tworzy fałszywą stronę internetową, która przypomina www.estores.com.
+ Wreszcie, narzędzie (np. dnsspoof) jest używane do kierowania wszystkich żądań DNS do lokalnego pliku hosta sprawcy. W rezultacie fałszywa strona internetowa jest wyświetlana użytkownikom i tylko poprzez interakcję z witryną malware jest instalowane na ich komputerach.

## 2.5.8. DHCP Attack

DHCP Attack służy do automatycznego przypisywania adresów IP do komputerów w dowolnej sieci. Aby przeprowadzić ten atak osoba atakująca wysyła mnóstwo fałszywych wiadomości DHCP Discover ze sfałszowanymi źródłowymi adresami MAC. 

Serwer DHCP próbuje odpowiedzieć na wszystkie te fałszywe wiadomości, w wyniku czego pula adresów IP używanych przez serwer DHCP jest wyczerpana. W związku z tym legalny użytkownik nie będzie mógł uzyskać adresu IP za pośrednictwem DHCP. Powoduje to atak DoS. Ponadto osoba atakująca może skonfigurować nieautoryzowany serwer DHCP, aby przypisać adresy IP uprawnionym użytkownikom. Ten nieautoryzowany serwer może również udostępniać użytkownikom router bramy i serwer DNS. Teraz cały ruch sieciowy może być kierowany przez maszynę atakującego, a to nic innego jak atak MITM.

<p align="center">
  Rys.2.5.7.1. Działanie ataku DHCP
<br>
  <img src="\assets\img\Cyber\67.png" width="650" alt="dhcp">
  <br>
  Źródło: https://media.geeksforgeeks.org/wp-content/uploads/20220709123409/gfgDHCPstarvationattack.jpg
</p>

Adres IP serwera DHCP to 10.10.10.1/24 z maską podsieci 255.255.255.0. Dzięki temu serwer DHCP może rozdawać 254 unikatowe adresy IP. Jednak niektóre adresy IP są zarezerwowane dla routingu statycznego, więc może być mniejszy niż 254. Atakujący wysyła N pakietów DHCP Discover, gdzie N jest bardzo duże w porównaniu do 254. W związku z tym serwer DHCP nie może już rozdawać adresów IP.

## 2.5.9. VBLAN Hooping

VLAN Hopping – to metoda atakowania zasobów sieciowych sieci VLAN poprzez wysyłanie pakietów do portu, który zwykle nie jest dostępny z systemu końcowego. Głównym celem tej formy ataku jest uzyskanie dostepu do innych sieci VLAN w tej samej sieci. 

### W jaki sposób VLAN Hopping powoduje luki w zabezpieczeniach sieci? 

Luki w zabezpieczeniach sieci VLAN dotyczą ich kluczowych funkcji, w tym:
+ Umożliwienie administratorom sieci podziału jednej sieci komutowanej w celu spełnienia wymagań funkcjonalnych i bezpieczeństwa ich systemów bez konieczności prowadzenia nowych lub wprowadzania istotnych zmian w infrastrukturze sieciowej.
+ Poprawa wydajności sieci poprzez grupowanie urządzeń, które często się komunikują.
+ Zapewnienie bezpieczeństwa w większych sieciach poprzez umożliwienie większej kontroli nad tym, które urządzenia mają do siebie dostęp.

<p align="center">
  Rys.2.5.10.1. Działanie magistrali sieci VLAN z przełącznikiem warstwy 3
<br>
  <img src="\assets\img\Cyber\68.png" width="650" alt="vlans">
  <br>
  Źródło: https://cdn.ttgtmedia.com/rms/onlineImages/VLAN_samplenet.jpg
</p>

### Metody przeprowadzania ataków VLAN Hopping
+ Podwójne tagowanie – ataki podwójnego tagowania występują, gdy cyberprzestępcy dodają i modyfikują znaczniki w ramce Ethernet. Takie podejście umożliwia wysyłanie pakietów przez dowolną sieć VLAN jako natywną nieoznakowaną sieć VLAN na magistrali i wykorzystuje kilka przełączników, które przetwarzają znaczniki.
Haker przesyła dane za pośrednictwem jednego przełącznika do drugiego, wysyłając ramki z dwoma znacznikami 802.1Q: jednym dla atakującego przełącznika, a drugim dla przełącznika ofiary. To oszukuje ofiarę, która myśli, że rama była do tego przeznaczona. Następnie przełącznik celu wysyła ramkę do portu ofiary.
Może się tak zdarzyć, ponieważ większość przełączników usuwa znacznik zewnętrzny tylko przed przekazaniem ramki do wszystkich natywnych portów VLAN. Jeśli na przykład przełącznik sieciowy został skonfigurowany do automatycznego trunkingu, osoba atakująca zamienia go w przełącznik, który wygląda tak, jakby stale potrzebował połączenia trunkingowego w celu uzyskania dostępu do wszystkich sieci VLAN dozwolonych na porcie magistrali. Ponieważ hermetyzacja pakietu zwrotnego jest niemożliwa, ten exploit bezpieczeństwa jest zasadniczo atakiem jednokierunkowym. Jest to możliwe tylko wtedy, gdy haker należy do tego samego natywnego łącza VLAN.
+ Przełączanie spoofingu – fałszowanie przełącznika ma miejsce, gdy osoba atakująca wysyła pakiety protokołu DTP w celu wynegocjowania trunku z przełącznikiem. Jest to możliwe tylko w przypadku korzystania z dynamicznego automatycznego lub dynamicznego pożądanego domyślnego trybu przełączania. Po podłączeniu magistrali do komputera osoba atakująca uzyskuje dostęp do wszystkich sieci VLAN. Jest to błędna konfiguracja, ponieważ interfejsy nie powinny być konfigurowane do korzystania z trybów portu przełącznika dynamicznego.

## 2.5.10. Routing Attack

Routing Attacks, czyli ataki na trasowanie, są to próby naruszenia lub zmiany sposobu, w jaki dane są kierowane w sieci komputerowej. Ataki tego typu mają na celu zakłócenie normalnego przepływu informacji, zmianę trasowania pakietów lub przejęcie kontroli nad siecią. Przestępcy mogą wykorzystywać różne techniki i luki w zabezpieczeniach, aby osiągnąć swoje cele.

Jednym z rodzajów ataków na trasowanie jest atak Man-in-the-Middle (MitM). W tym scenariuszu, atakujący umiejscawia się pomiędzy nadawcą a odbiorcą danych, podszywając się pod obie strony komunikacji. Atakujący może przechwycić, modyfikować lub zatrzymać przesyłane pakiety, a także wprowadzać fałszywe dane do sieci. W wyniku tego ataku, dane mogą być przekierowane do niepożądanych lokalizacji lub dostarczane do nieuprawnionych osób.

Innym przykładem ataku na trasowanie jest atak typu Distributed Denial of Service (DDoS). W tym przypadku, atakujący wysyła duże ilości żądań do routerów i serwerów w sieci, przeciążając je i uniemożliwiając normalne funkcjonowanie. DDoS może spowodować przestój w dostarczaniu usług, utrudnić komunikację między urządzeniami sieciowymi lub nawet całkowicie zablokować dostęp do zasobów sieciowych.

## 2.5.11. BGP Hijacking

BGP Hijacking ma miejsce, gdy atakujący złośliwie przekierowują ruch internetowy. Atakujący osiągają to fałszywie oglaszając własność grup adresów IP, zwanych prefiksami IP, których w rzeczywistości nie posiadają, nie kontrolują ani nie kierują do nich. 
Jak można przejąc BGP?

Gdy system AS ogłasza trasę do prefiksów IP, których w rzeczywistości nie kontroluje, komunikat ten, jeśli nie zostanie przefiltrowany, może zostać rozpowszechniony i dodany do tabel routingu w routerach BGP w Internecie. Od tego momentu, dopóki ktoś nie zauważy i nie poprawi tras, ruch do tych adresów IP będzie kierowany do tego AS.

BGP zawsze preferuje najkrótszą, najbardziej szczegółową ścieżkę do żądanego adresu IP. Aby porwanie BGP zakończyło się powodzeniem, ogłoszenie trasy musi:
+ Zaproponować bardziej szczegółową trasę, ogłaszając mniejszy zakres adresów IP niż wcześniej ogłoszone inne ASy.
+ Zaoferpwać krótszą trasę do niektórych bloków adresów IP. Ponadto nie każdy może ogłaszać trasy BGP do większego Internetu. Aby doszło do porwania BGP, ogłoszenie musi zostać dokonane przez operatora systemu AS lub przez ugrupowanie cyberprzestępcze, które włamało się do systemu AS. 

<p align="center">
  Rys.2.5.11.1. Działanie ataku BGP Hijacking
<br>
  <img src="\assets\img\Cyber\69.png" width="650" alt="bgph">
  <br>
  Źródło: https://www.cloudflare.com/img/learning/security/glossary/bgp-hijacking/bgp-hijacking-technical-flow.png
</p>

## 2.5.12. IP Fragmentation Attack

IP Fragmentation Attack jest standardową formą ataku wolumetrycznej typu "odmowa usługi" (DoS). Odmowa usługi (DoS) to każdy rodzaj ataku, w którym osoby atakujące próbują uniemożliwić prawdziwym użytkownikom online dostęp do usługi. Podczas ataku fragmentacji IP mechanizmy fragmentacji datagramów są wykorzystywane do miażdżenia sieci.

### Jak działa IP Fragmentation Attack?

Fragmentacja IP ma miejsce, gdy datagramy IP są rozbite na małe pakiety. Uszkodzone pakiety są następnie wysyłane przez sieć, gdzie są rekonstruowane w oryginalny datagram w ramach regularnej komunikacji online.
Cały ten proces jest niezbędny, aby spełnić parametry wielkości, które każda sieć może wytrzymać. Ten limit wielkości jest zdefiniowany jako maksymalna jednostka transmisji (MTU).

### Typy ataków IP Fragmentaion adresów IP
+ Tiny fragment attack – każdy pakiet IP zawiera nagłówek i ładunek. Nagłówek składa się ze szczegółów, które kierują pakiet IP do zamierzonego miejsca docelowego. Z drugiej strony ładunek jest strukturą, która przenosi dane w kierunku nagłówka. Atak z małym fragmentem to mały miniaturowy atak, który występuje, gdy mały fragment pakietu ląduje na serwerze. Zwykle dzieje się tak, gdy jeden z fragmentów nie mieści się w nagłówku, ponieważ jest zbyt mały, co powoduje problemy z ponownym złożeniem, które mogą potencjalnie zamknąć serwer.
+ UDP i ICMP fragmentation attacks – ataki UDP i ICMP zalewają serwery dużymi i podejrzanymi pakietami. Proces ten drastycznie przeciąża serwer, uniemożliwiając mu wykonywanie zaplanowanych funkcji.
+ TCP fragmentation attack – atak Teardrop lub atak TCP wykorzystuje pakiety, które zostały opracowane tak, aby nie łączyć się ponownie po dostarczeniu. Bez środków bezpieczeństwa te fragmenty pakietów mogą zatrzymać system operacyjny i spowodować jego awarię, czyniąc go bezużytecznym.
