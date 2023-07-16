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
