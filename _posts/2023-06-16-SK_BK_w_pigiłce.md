---
layout: post
title: Książka
subtitle: Sieci komputerowe i bezpieczeństwo w pigułce
author: Oleh Danchivskyi
cover-img: /assets/img/Sieci/Logo.png
thumbnail-img: /assets/img/Sieci/Logo-1.png
share-img: /assets/img/Sieci/Logo.png
tags: [Sieci, Bezpieczeńswto, Komputery]
---

- [1. Architektura sieciowa](#1. Architektura sieciowa)
- [1.1. Model TCP/IP](#Model-TCP/IP)
- [1.2. model ISO/OSI](#Model-ISO/OSI)
- [2. Technologie sieciowe](#Technologie-sieciowe)
- [2.1. Technologia Ethernet](#Technologia-Ethernet)
- [2.2. Technologia WI-FI](#Technologia-WI-FI)
- [2.3. IPS](#IPS)



# 1. Architektura sieciowa

Architektura sieciowa to sposób organizacji i połączenia urządzeń sieciowych, który umożliwia wymianę danych i zasobów pomiędzy nimi. Składa się z różnych elementów, które mają określone role i funkcje, a ich współpraca umożliwia poprawne działanie sieci. Oto kilka podstawowych elementów architektury sieciowej:

<p align="center">
  Rys.1 Architektura sieci komputerowej
<br>
  <img src="\assets\img\Sieci\1.png" width="650" alt="architektura">
</p>

+ Komputery: to podstawowe urządzenia, które wykorzystują sieć do przesyłania i odbierania danych.
+ Kable i łącza: służą do połączenia urządzeń sieciowych i umożliwiają przesyłanie danych między nimi. Mogą to być kable miedziane, światłowodowe, bezprzewodowe itp.
+ Routery: służą do kierowania ruchem między sieciami i umożliwiają komunikację pomiędzy różnymi sieciami.
+ Switche: służą do połączenia urządzeń w sieci lokalnej (LAN) i umożliwiają przesyłanie danych między nimi.
+ Bramki: umożliwiają komunikację między różnymi sieciami o różnych protokołach.
+ Serwery: służą do przechowywania i udostępniania danych oraz usług w sieci, takich jak pliki, bazy danych, poczta elektroniczna, strony internetowe itp.
+ Firewalle: służą do zabezpieczenia sieci przed niepożądanym ruchem sieciowym, takim jak ataki typu DoS, próby włamań, itp.
+ Protokoły sieciowe: to zestaw reguł i standardów, które umożliwiają urządzeniom sieciowym komunikację i wymianę danych. Przykłady protokołów sieciowych to TCP/IP, HTTP, FTP, SMTP, POP3 itp.


Architektura sieciowa może być różna w zależności od potrzeb i rozmiaru sieci. W dużych sieciach, takich jak sieci korporacyjne, może być kilka warstw pośredniczących pomiędzy urządzeniami końcowymi a serwerami, takie jak warstwy dostępu, dystrybucji i rdzenia. W mniejszych sieciach, takich jak sieci domowe, architektura może być bardziej prosta i składać się tylko z kilku elementów, takich jak komputery, router, switch i kabel.


## 1.1. Model TCP/IP

Model TCP/IP to model warstwowy, który opisuje sposób, w jaki urządzenia sieciowe komunikują się ze sobą w sieciach opartych o protokół TCP/IP. Model ten składa się z 4 warstw, każda z nich odpowiada za określone zadania i protokoły. Oto opis każdej z nich:

<p align="center">
Rys. 1.1.1. Model TCP/IP
<br>
  <img src="\assets\img\Sieci\2.jpg" width="650" alt="TCP/IP">
  <br>
  Źródło: https://pasja-informatyki.pl/pliki/model-tcp-ip.jpg
</p>

+ Warstwa aplikacji: to warstwa, która umożliwia aplikacjom korzystanie z sieci (np. WWW, poczta elektroniczna, wymiana plików, połączenia terminalowe czy komunikatory). Zawiera protokoły, takie jak HTTP, SMTP, FTP, DNS, SSH, które pozwalają na przesyłanie danych między aplikacjami. Protokoły te są zwykle napisane w języku wysokiego poziomu, co umożliwia programistom łatwe korzystanie z nich.
+ Warstwa transportowa: to warstwa, która zapewnia poprawne przesyłanie danych między aplikacjami. Zawiera protokoły, takie jak TCP i UDP, które umożliwiają kontrolę przepływu danych, kontrolę błędów i segmentację danych na mniejsze pakiety.
+ Warstwa sieciowa: to warstwa, która odpowiada za kierowanie ruchem między różnymi sieciami. Zawiera protokoły, takie jak IP, ICMP, ARP, które pozwalają na przesyłanie danych między różnymi sieciami oraz na znajdowanie adresów urządzeń w sieci.
+ Warstwa dostępu do sieci: to warstwa, która umożliwia urządzeniom komunikację z fizycznymi urządzeniami sieciowymi, takimi jak karty sieciowe, switch'e i routery. Zawiera protokoły, takie jak Ethernet, Token Ring, FDDI, które określają sposób transmisji danych między urządzeniami.

Wiadomość jest wysyłana od najwyżej do najniższej warstwy, a w każdej z nich do wiadomości dodawane są kolejne nagłówki zapewniające prawidłowe dostarczanie danych – proces ten nazywany jest enkapsulacją. Dane zwrotne powracają od najniższej do najwyżej warstwy do punktu docelowego.


## 1.2. Model ISO/OSI

Model ISO/OSI (Open Systems Interconnection) to model warstwowy, który opisuje sposób, w jaki urządzenia sieciowe komunikują się ze sobą w sieciach komputerowych. Model ten składa się z 7 warstw, każda z nich odpowiada za określone zadania i protokoły. Oto opis każdej z warstw:
+ Warstwa fizyczna: to warstwa, która odpowiada za transmisję sygnału fizycznego między urządzeniami. Zawiera protokoły, takie jak Ethernet, Wi-Fi, Bluetooth, które pozwalają na przesyłanie sygnału elektrycznego lub radiowego między urządzeniami.
+ Warstwa łącza danych: to warstwa, która zapewnia poprawne przesyłanie danych między urządzeniami w tej samej sieci. Zawiera protokoły, takie jak PPP, HDLC, Ethernet, które umożliwiają kontrolę błędów, segmentację danych na mniejsze pakiety oraz kontrolę przepływu danych.
+ Warstwa sieciowa: to warstwa, która odpowiada za kierowanie ruchem między różnymi sieciami. Zawiera protokoły, takie jak IP, ICMP, ARP, które pozwalają na przesyłanie danych między różnymi sieciami oraz na znajdowanie adresów urządzeń w sieci.
+ Warstwa transportowa: to warstwa, która zapewnia poprawne przesyłanie danych między aplikacjami. Zawiera protokoły, takie jak TCP i UDP, które umożliwiają kontrolę przepływu danych, kontrolę błędów i segmentację danych na mniejsze pakiety.
+ Warstwa sesji: to warstwa, która zapewnia kontrolę nad sesją między aplikacjami. Zawiera protokoły, takie jak RPC, NetBIOS, która umożliwia aplikacjom nawiązywanie i utrzymywanie połączeń między sobą.
+ Warstwa prezentacji: to warstwa, która odpowiada za przetwarzanie i formatowanie danych w sposób zrozumiały dla aplikacji. Zawiera protokoły, takie jak MIME, SSL, które umożliwiają kompresję danych, szyfrowanie i dekodowanie formatów danych.
+ Warstwa aplikacji: to warstwa, która umożliwia aplikacjom korzystanie z sieci. Zawiera protokoły, takie jak HTTP, SMTP, FTP, DNS, SSH, które pozwalają na przesyłanie danych między aplikacjami.


| Warstwa | Wytłumaczenie |
|------------|------------|
| Warstwa Aplikacji   | Zadaniem najwyższej warstwy modelu jest zapewnienie komunikacji aplikacji z niższymi warstwami modelu. Pełni więc funkcję interfejsu pomiędzy siecią a programem.   |
| Warstwa Prezentacji   | Funkcją warstwy prezentacji jest przetwarzanie danych do odpowiedniej postaci tzw. Postaci Kanonicznej. Zajmuje się również zamianą odwrotną. Najprościej rzecz ujmując pełni funkcję tłumacza, który zmienia formaty danych oraz sposoby ich szyfrowania.  |
| Warstwa Sesji   | Zadaniem piątej warstwy modelu ISO/OSI jest synchronizacja danych sesji pomiędzy odbiorcą a nadawcą. Nadzoruje połączenie między innymi poprzez zapewnianie właściwego kierunku przepływu danych czy wznawianie transmisji po przerwaniu.   |
| Warstwa Transportu   | Dzieli ona dane na segmenty, a następnie w zależności od użytego protokołu czeka na potwierdzenie przyjęcia pakietu przez hosta docelowego, a w przypadku odnotowania, że pakiet nie dotarł, ponownie wysyła segment.   |
| Warstwa Sieci   | Rolą tej warstwy jest zmiana segmentów na pakiety, a następnie określenie najlepszej trasy dla pakietu do jego celu. Warto pamiętać, że warstwa sieci nie odpowiada za zapewnienie ciągłości transmisji.  |
| Warstwa Łącza danych   | Ta warstwa odpowiada za zmianę pakietów na ramki danych. Jednakże ma także inne zadania. W związku z tym możemy ją podzielić na dwie podwarstwy. Pierwszą z nich jest LLC, która odpowiada za sterowanie łączem danych, czyli kontroluje poprawność transmitowanych ramek. Drugą podwarstwą jest MAC, która zajmuje się przyznawaniem dostępu do medium transmisyjnego.  |
| Warstwa Fizyczna   | Zadanie warstwy fizycznej jest wręcz banalne. Zamienia ramki danych na bity, a następnie wysyła je po medium transmisyjnym. Oprócz tego odbiera nadane informacje i przekazuje je w górę modelu.  |


<p align="center">
Rys. 1.2.1. Model ISO/OSI
<br>
  <img src="\assets\img\Sieci\3.png" width="650" alt="ISO/OSI">
</p>



# 2. Technologie sieciowe

Technologie sieciowe to różnego rodzaju rozwiązania i narzędzia, które umożliwiają komunikację między urządzeniami w sieciach komputerowych. Obejmują one różne aspekty, takie jak przesyłanie danych, zarządzanie siecią, bezpieczeństwo, a także aplikacje i usługi sieciowe.

## 2.1. Technologie Ethernet

Ethernet to technologia przewodowa, która umożliwia komunikację między urządzeniami w tej samej sieci lokalnej (LAN). Technologia Ethernet jest szeroko stosowana w sieciach komputerowych ze względu na swoją prostotę i niskie koszty.

Ethernet wykorzystuje protokół CSMA/CD (Carrier Sense Multiple Access with Collision Detection), który umożliwia urządzeniom dzielenie się medium transmisyjnym. Urządzenia sieciowe, takie jak komputery, serwery i routery, mogą komunikować się ze sobą, wysyłając pakiety danych przez medium transmisyjne, takie jak kabel Ethernet.

W technologii Ethernet, pakiety danych są przesyłane w ramkach, a każda ramka składa się z nagłówka, danych i sumy kontrolnej CRC. Nagłówek ramki zawiera adresy MAC nadawcy i odbiorcy, a także informacje o typie ramki i długości danych.

Ethernet to cały zbiór rozwiązań sieciowych, które implementowane są zarówno w warstwie łącza danych, jak również w warstwie fizycznej. Pieczę nad rozwojem tej technologii sprawuje obecnie organizacja IEEE (ang. Institute of Electrical and Electronics Engineers), która w 1985 roku opublikowała jej standardy i opisała je numerem 802.2 oraz 802.3. Standard 802.2 odnosi się do funkcji związanych z podwarstwą LLC, ten drugi natomiast do podwarstwy MAC oraz do warstwy fizycznej modelu OSI.

<p align="center">
Rys. 2.1.1. Technologia Ethernet
<br>
  <img src="\assets\img\Sieci\4.jpg" width="650" alt="Ethernet">
  <br>
  Źródło: https://pasja-informatyki.pl/pliki/ieee-warstwa-lacza-danych.jpg
</p>

## 2.2. Technologia WI-FI

Technologia Wi-Fi to bezprzewodowa technologia sieciowa, która umożliwia urządzeniom komunikację między sobą bez użycia kabli. Technologia Wi-Fi wykorzystuje radiofale do przesyłania danych między urządzeniami.

Sieć Wi-Fi składa się z punktów dostępowych (AP), które pełnią rolę mostu między urządzeniami bezprzewodowymi a siecią przewodową lub internetem. Punkty dostępowe są podłączone do sieci przewodowej i emitują sygnały radiowe, które urządzenia bezprzewodowe odbierają i interpretują jako dane.

Technologia Wi-Fi opiera się na standardach opracowywanych przez organizację IEEE (Institute of Electrical and Electronics Engineers). Najbardziej popularne standardy Wi-Fi to 802.11a, 802.11b, 802.11g, 802.11n, 802.11ac i 802.11ax. Każdy standard Wi-Fi określa różne parametry, takie jak prędkość przesyłania danych, częstotliwość, zasięg i inne funkcje.

Najważniejsze zalety technologii Wi-Fi to brak konieczności stosowania kabli, elastyczność i mobilność. Urządzenia bezprzewodowe, takie jak laptopy, smartfony, tablety i inne urządzenia mobilne, mogą łączyć się z siecią bezprzewodową z dowolnego miejsca, w którym jest dostęp do sygnału Wi-Fi. Technologia Wi-Fi jest również stosowana w urządzeniach IoT (Internet of Things), takich jak inteligentne urządzenia domowe i przemysłowe.


## 2.3. IPS

Technologia IPS (Intrusion Prevention System) to narzędzie bezpieczeństwa sieciowego, które służy do wykrywania i blokowania niebezpiecznych działań na sieci. IPS jest rozwinięciem technologii IDS (Intrusion Detection System), która służy tylko do wykrywania działań nieautoryzowanych.

<p align="center">
Rys. 2.3.1. IPS
<br>
  <img src="\assets\img\Sieci\5.png" width="650" alt="IPS">
</p>

IPS monitoruje ruch sieciowy i analizuje go, szukając zachowań, które mogą wskazywać na atak lub inne niebezpieczne działanie. Gdy IPS wykryje takie zachowanie, natychmiast podejmuje akcje mające na celu zablokowanie lub zminimalizowanie szkód wynikających z ataku. IPS może na przykład zablokować ruch sieciowy pochodzący z niezaufanego źródła, lub zablokować atakującego, który próbuje przeprowadzić atak typu Denial of Service (DoS). Systemy IPS mogą także wykrywać różne rodzaje ataków, takie jak próby przejęcia sesji, ataki typu SQL injection, próby złamania hasła, próby ataków na usługi sieciowe i wiele innych.

IPS stosuje różne techniki, aby zidentyfikować niebezpieczne zachowania, takie jak sygnatury ataków, heurystyka, czy analiza zachowań. Sygnatury ataków to zbiory charakterystycznych cech ruchu sieciowego, które wskazują na określony typ ataku. Heurystyka to analiza ruchu sieciowego w celu wykrycia zachowań, które mogą wskazywać na atak, ale nie pasują do sygnatur ataków. Analiza zachowań to technika, która analizuje zachowanie użytkowników, urządzeń i aplikacji w sieci, aby wykryć podejrzane aktywności.


# 3. Metody GET i POST

+ GET 
GET służy do żądania od serwera danej strony WWW. Jego nagłówek wygląda mniej więcej tak:  GET /tomijerry.html HTTP/1.1

W żądaniu GET znajdują się jeszcze takie informacje jak: nazwa hosta (np. wp.pl), nazwa przeglądarki, z jakiej zostało wysłane żądanie, akceptowane przez przeglądarkę typy plików, preferowany język strony czy kodowanie znaków. W odpowiedzi serwera, znajdują się informacje, takie jak: czas serwera, nazwa aplikacji serwera (np. APACHE) czy czas wygaśnięcia dokumentu.

Jeśli z jakiś przyczyn serwer WWW nie może odesłać zasobu, odsyła komunikat błędu, np. 404, który informuje, że żądany zasób nie został znaleziony, lub 403 informujący o zabronionym dostępie do zasobów. Wybrane kody komunikatów i błędów widoczne są w poniższych tabelach.

+ POST
Kolejny typ wiadomości to wiadomość POST, która służy do przesyłania danych na serwer. Kiedy storna internetowa zawiera np. formularz wysyłający dane na serwer, np. formularz rejestracji, to dane które w nim umieścimy wysyłane są właśnie za pomocą wiadomości POST.

<p align="center">
Rys. 3.1. Przesyłanie formularza do serwera
<br>
  <img src="\assets\img\Sieci\6.jpg" width="650" alt="Formularz">
  <br>
  Źródło: https://pasja-informatyki.pl/pliki/metoda-post.jpg
</p>

Protokół HTTP mimo, że bardzo popularny, chyba najczęściej stosowany ze wszystkich protokołów warstwy aplikacji, nie jest bezpieczny. Metoda POST przesyła dane do serwera jawnym tekstem. Kiedy uda się przechwycić transmisję pomiędzy klientem, a serwerem, można odczytać informacje jakie chcemy przesłać na serwer.

<p align="center">
Rys. 3.2. Otrzymanie danych logowania
<br>
  <img src="\assets\img\Sieci\7.jpg" width="650" alt="Dane">
  <br>
  Źródło: https://pasja-informatyki.pl/pliki/tekst-jawny.jpg
</p>

Jest to bardzo niebezpieczne, dlatego obecnie większość stron WWW, na których istnieje możliwość przesłania na serwer jakieś informacji, czyli np. na tych stronach gdzie konieczne jest logowanie, stosowany jest już protokół HTTPS szyfrujący komunikację pomiędzy klientem a serwerem, działa on na porcie 443.

# 4. Protokoły sieciowe

Protokoły warstwowe to zestaw standardów i reguł, które umożliwiają przesyłanie informacji między urządzeniami w sieci komputerowej. Protokoły te są podzielone na warstwy, a każda z warstw odpowiada za określone zadania związane z przetwarzaniem i przesyłaniem danych.

## 4.1. TCP

Protokół TCP (Transmission Control Protocol) to jeden z dwóch głównych protokołów warstwy transportowej (obok UDP) używanych w sieciach komputerowych opartych na modelu TCP/IP. TCP jest protokołem połączeniowym, który zapewnia niezawodne i uporządkowane dostarczenie danych między aplikacjami działającymi na różnych urządzeniach w sieci.

<p align="center">
Rys. 3.2. Jak działa TCP
<br>
  <img src="\assets\img\Sieci\8.svg" width="650" alt="TCP">
  <br>
  Źródło: https://nordvpn.com/wp-content/uploads/blog-how-tcp-works-infographic-server-phone-pl-1200x628-1.svg
</p>

TCP działa w następujący sposób:
+ Nawiązanie połączenia - przed rozpoczęciem transmisji danych, aplikacje korzystające z protokołu TCP muszą najpierw nawiązać połączenie między sobą. W tym celu inicjują proces zwany "trzykrotne potwierdzenie", który służy do ustanowienia połączenia między nadawcą a odbiorcą.
+ Segmentacja - dane są dzielone na mniejsze segmenty, ponieważ większe pakiety mogą przeciążać sieć lub być utracone. Każdy segment jest numerowany i zawiera informację o sekwencji, która jest wykorzystywana do uporządkowania segmentów po otrzymaniu ich przez odbiorcę.
+ Kontrola przepływu - TCP zapewnia mechanizmy kontroli przepływu, które ograniczają ilość danych, które można przesłać w danej chwili, aby uniknąć przeciążenia sieci.
+ Mechanizmy naprawy błędów - TCP zawiera mechanizmy do wykrywania i naprawy błędów w transmisji danych. Jeśli segment nie zostanie odebrany poprawnie, odbiorca zgłasza to nadawcy, który wysyła segment ponownie.
+ Zakończenie połączenia - po przesłaniu danych, aplikacje korzystające z protokołu TCP muszą zakończyć połączenie. W tym celu inicjują proces zwanym "czterokrotnym potwierdzeniem", który służy do poprawnego zamknięcia połączenia.

TCP jest często używany w aplikacjach, które wymagają niezawodnej i uporządkowanej transmisji danych, takich jak przeglądarki internetowe, poczta elektroniczna, transfer plików czy strumieniowanie wideo. Jednakże, ze względu na swoje mechanizmy kontroli przepływu i naprawy błędów, TCP wprowadza dodatkowe opóźnienia w transmisji danych, co może wpłynąć na szybkość przesyłania danych w niektórych zastosowaniach wymagających szybkiej transmisji, takich jak gry online czy transmisja strumieniowa w czasie rzeczywistym.

Przykład działania protokołu TCP:

Krok 1: Nawiązanie połączenia:

Kiedy dwa komputery chcą przesłać do siebie dane za pomocą protokołu TCP, muszą najpierw nawiązać połączenie za pomocą trójstronnego uścisku dłoni (ang. three-way handshake).

<p align="center">
Rys. 3.2. Przykład działania TCP
<br>
  <img src="\assets\img\Sieci\9.png" width="650" alt="Przykład TCP">
</p>

Protokół TCP/IP to zbiór protokołów, które są używane do przesyłania danych w sieciach komputerowych. Protokół TCP jest jednym z protokołów wchodzących w skład protokołu TCP/IP i odpowiada za zapewnienie niezawodnej transmisji danych między aplikacjami działającymi na różnych komputerach w sieci.

TCP (Transmission Control Protocol) zapewnia połączenie punkt-punkt między dwoma hostami i umożliwia wysyłanie strumieni danych w sposób niezawodny, poprzez podział ich na pakiety i ponowną transmisję w przypadku utraty lub uszkodzenia jakiegoś pakietu. Protokół TCP odpowiada również za kontrolę przepływu i porządkowanie pakietów danych.

Natomiast protokół TCP/IP składa się z wielu protokołów, w tym m.in. z protokołu IP (Internet Protocol), który odpowiada za adresowanie i przesyłanie pakietów danych w sieci oraz protokołu TCP, który zapewnia niezawodność transmisji danych. Protokół TCP/IP jest zwykle używany do komunikacji w Internecie oraz w większości sieci komputerowych.
