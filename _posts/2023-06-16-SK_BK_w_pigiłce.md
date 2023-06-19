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
Rys. 4.1.1. Jak działa TCP
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
Rys. 4.1.2. Przykład działania TCP
<br>
  <img src="\assets\img\Sieci\9.png" width="650" alt="Przykład TCP">
</p>

Protokół TCP/IP to zbiór protokołów, które są używane do przesyłania danych w sieciach komputerowych. Protokół TCP jest jednym z protokołów wchodzących w skład protokołu TCP/IP i odpowiada za zapewnienie niezawodnej transmisji danych między aplikacjami działającymi na różnych komputerach w sieci.

TCP (Transmission Control Protocol) zapewnia połączenie punkt-punkt między dwoma hostami i umożliwia wysyłanie strumieni danych w sposób niezawodny, poprzez podział ich na pakiety i ponowną transmisję w przypadku utraty lub uszkodzenia jakiegoś pakietu. Protokół TCP odpowiada również za kontrolę przepływu i porządkowanie pakietów danych.

Natomiast protokół TCP/IP składa się z wielu protokołów, w tym m.in. z protokołu IP (Internet Protocol), który odpowiada za adresowanie i przesyłanie pakietów danych w sieci oraz protokołu TCP, który zapewnia niezawodność transmisji danych. Protokół TCP/IP jest zwykle używany do komunikacji w Internecie oraz w większości sieci komputerowych.


## 4.2. UDP

Protokół UDP jest prostym, bezpołączeniowym protokołem, którego największą zaletą jest niewielki narzut danych sterujących, dodawanych w procesie enkapsulacji. UDP w datagramie dodaje tylko 8 bajtów danych sterujących. Nagłówek datagramu UDP wygląda tak:

<p align="center">
Rys. 4.2.1. Ramka UDP
<br>
  <img src="\assets\img\Sieci\10.png" width="650" alt="UDP">
</p>

+ Port źródłowy – określa port aplikacji, z której wysłano dane.
+ Port docelowy – określa port aplikacji, do której wysłano dane.
+ Długość – 16 – bitowe pole określające długość całego datagramu UDP
+ Suma kontrolna – 16 – bitowe pole służące do sprawdzania poprawności przesłanych danych.

UDP (User Datagram Protocol) to protokół warstwy transportowej w modelu OSI, który zapewnia szybkie, niezawodne i bezpołączeniowe przesyłanie datagramów (pakietów) między aplikacjami w sieci komputerowej.

W przeciwieństwie do protokołu TCP, UDP nie zapewnia mechanizmów kontroli błędów i gwarancji dostarczenia danych. Zamiast tego, aplikacja musi sama zadbać o sprawdzenie poprawności otrzymanych danych oraz o retransmisję w przypadku ich utraty.

<p align="center">
Rys. 4.2.2. Działanie UDP
<br>
  <img src="\assets\img\Sieci\11.png" width="650" alt="Działanie UDP">
</p>

UDP jest często wykorzystywany do przesyłania informacji, które nie wymagają pełnej niezawodności, jak na przykład transmisja strumieniowa w czasie rzeczywistym (np. wideo czy dźwięku). Wysoka szybkość przesyłania danych i brak opóźnień wynikających z konieczności nawiązywania połączenia i kontroli błędów czynią UDP idealnym protokołem dla takich zastosowań.


## 4.3. IP 

IP (Internet Protocol) to protokół warstwy sieciowej w modelu OSI, który odpowiada za przesyłanie pakietów między różnymi sieciami komputerowymi w Internecie. IP jest protokołem bezpołączeniowym, co oznacza, że nie utrzymuje on żadnego stanu między wysyłającym a odbierającym.

<p align="center">
Rys. 4.2.2. Działanie IP
<br>
  <img src="\assets\img\Sieci\12.png" width="650" alt="IP">
</p>

IP dzieli dane na pakiety i przekazuje je do odbiorcy, wykorzystując do tego celu adresy IP na dane każdemu urządzeniu w sieci. Protokół IP jest niezawodny w sensie, że gwarantuje dostarczenie pakietów do celu, ale nie zapewnia gwarancji kolejności, w jakiej pakiety zostaną dostarczone.

Istnieją dwie wersje protokołu IP: IP v4 i IP v6. Wersja v4 jest bardziej popularna i wykorzystywana w większości sieci, ale jej adresy IP są ograniczone do 32-bitowych wartości, co oznacza, że maksymalna liczba urządzeń w Internecie, które mogą posiadać unikalny adres IP v4, wynosi około 4,3 miliarda. Wersja v6 rozszerza ten zakres, umożliwiając przypisanie adresów IP o długości 128 bitów i umożliwiając tym samym dużo większą liczbę unikalnych adresów.

# 5. Protokoły aplikacyjne

Protokoły aplikacyjne to protokoły wyższych warstw modelu OSI, które umożliwiają aplikacjom komunikację między sobą poprzez sieć komputerową.

## 5.1. HTTP

HTTP (Hypertext Transfer Protocol) to protokół aplikacyjny wykorzystywany do przesyłania danych między przeglądarką internetową a serwerem WWW. Protokół HTTP definiuje sposób, w jaki przeglądarka internetowa żąda informacji z serwera i otrzymuje odpowiedź.

Każde żądanie HTTP składa się z trzech części: metody, adresu URL i wersji protokołu HTTP. Najczęściej używanymi metodami są GET i POST, które służą odpowiednio do pobierania i wysyłania danych z serwera. Adres URL określa konkretną stronę lub zasób, który jest żądany, a wersja protokołu HTTP określa wersję protokołu, która jest używana do przesyłania danych.

Odpowiedź HTTP składa się z trzech części: statusu, nagłówków i treści. Status określa, czy żądanie zostało pomyślnie wykonane, czy też wystąpił jakiś błąd. Nagłówki zawierają dodatkowe informacje na temat odpowiedzi, takie jak typ treści, rozmiar pliku i czas wygaśnięcia. Treść zawiera właściwe dane przesyłane z serwera do przeglądarki, takie jak strona internetowa lub plik multimedialny.

<p align="center">
Rys. 5.1.1. Prośba o plik 
<br>
  <img src="\assets\img\Sieci\13.png" width="650" alt="HTTP">
</p>

Oczywiście tak to wygląd w telegraficznym skrócie. W rzeczywistości proces ten jest nieco bardziej złożony. Weźmy sobie przykładowy adres internetowy:

http://www.alamakota.pl/tomijerry.html

Po jego wpisaniu i zatwierdzeniu, najpierw przeglądarka sprawdza rodzaj protokołu, następnie nazwę domeny internetowej, a na końcu dopiero brana jest pod uwagę nazwa konkretnego pliku. Później nasza przeglądarka odwołuje się do serwera DNS, w celu zamiany nazwy mnemonicznej, czyli alamakota.pl na adres IP serwera, na którym ta strona jest przechowywana.

<p align="center">
Rys. 5.1.2. Pytanie do serwera DNS
<br>
  <img src="\assets\img\Sieci\14.png" width="650" alt="HTTP-1">
</p>

Znając już ten adres przeglądarka wysyła żądanie do serwera o udostępnienie pliku tomijerry.html znajdującego się w domenie alamakota.pl. Jeśli serwer dany zasób posiada w odpowiedzi przesyła stosowny komunikat wraz z zawartością żądanego pliku. Zawartość tego pliku, czyli kod HTML jest przez przeglądarkę interpretowany i wyświetlany jako strona WWW.

<p align="center">
Rys. 5.1.3. Końcowa odpowiedź 
<br>
  <img src="\assets\img\Sieci\15.png" width="650" alt="HTTP-2">
</p>


## 5.2. HTTPS

HTTPS (Hypertext Transfer Protocol Secure) to protokół bezpieczny oparty na protokole HTTP, który wykorzystuje protokół SSL/TLS (Secure Sockets Layer/Transport Layer Security) do szyfrowania danych między przeglądarką internetową a serwerem WWW.

HTTPS chroni prywatność i bezpieczeństwo przesyłanych danych, takich jak dane logowania, dane karty kredytowej, informacje osobiste itp. Szyfrowanie SSL/TLS chroni przed przechwyceniem danych przez osoby trzecie, ponieważ dane są szyfrowane w trakcie transmisji.

Protokół HTTPS działa w następujący sposób:
+ Przeglądarka internetowa łączy się z serwerem WWW i wysyła prośbę o połączenie HTTPS.
+ Serwer przesyła do przeglądarki certyfikat SSL/TLS, który zawiera klucz publiczny.
+ Przeglądarka sprawdza autentyczność certyfikatu SSL/TLS i pobiera klucz publiczny.
+ Przeglądarka i serwer wymieniają się kluczami, aby nawiązać bezpieczne połączenie.
+ Po nawiązaniu bezpiecznego połączenia przeglądarka i serwer mogą bezpiecznie przesyłać dane między sobą.

## 5.3. FTP 

FTP (File Transfer Protocol) to protokół aplikacyjny wykorzystywany do przesyłania plików między komputerami w sieci. FTP wykorzystuje klient-serwer model, w którym klient nawiązuje połączenie z serwerem FTP i przesyła lub pobiera pliki.

Komunikacja między klientem a serwerem FTP składa się z trzech części:
+ Połączenie: Klient nawiązuje połączenie z serwerem FTP i przesyła dane uwierzytelniające, takie jak login i hasło.
+ Transfer plików: Po nawiązaniu połączenia klient i serwer mogą rozpocząć przesyłanie plików. Klient może pobierać pliki z serwera lub przesyłać pliki na serwer.
+ Zamknięcie połączenia: Po przesłaniu lub pobraniu plików klient kończy połączenie z serwerem FTP.

Istnieją dwa tryby transferu plików w FTP: tryb ASCII i tryb binarny. Tryb ASCII jest używany do przesyłania plików tekstowych, takich jak pliki HTML, a tryb binarny jest używany do przesyłania plików binarnych, takich jak pliki graficzne lub pliki dźwiękowe.

FTP nie zapewnia szyfrowania danych, co oznacza, że dane przesyłane między klientem a serwerem mogą być łatwo przechwycone przez osoby trzecie. Aby zwiększyć bezpieczeństwo transferu plików, można użyć protokołu SFTP (Secure File Transfer Protocol), który wykorzystuje szyfrowanie SSL/TLS do ochrony danych.

<p align="center">
Rys. 5.3.1. Działanie FTP
<br>
  <img src="\assets\img\Sieci\16.png" width="650" alt="FTP">
</p>


## 5.4. SFTP

SFTP (Secure File Transfer Protocol) to protokół aplikacyjny wykorzystywany do bezpiecznego przesyłania plików między klientem a serwerem. SFTP jest protokołem sieciowym, który działa na warstwie transportowej, a konkretnie na protokole SSH (Secure Shell).

SFTP wykorzystuje szyfrowanie SSL/TLS, aby zapewnić bezpieczne przesyłanie danych między klientem a serwerem. W przeciwieństwie do protokołu FTP, który nie zapewnia szyfrowania danych, SFTP szyfruje całą komunikację między klientem a serwerem, w tym loginy i hasła oraz przesyłane pliki.

SFTP działa w następujący sposób:
+ Klient nawiązuje połączenie z serwerem SFTP poprzez protokół SSH.
+ Po nawiązaniu połączenia klient przesyła dane uwierzytelniające, takie jak login i hasło.
+ Po uwierzytelnieniu klient może przesyłać lub pobierać pliki z serwera SFTP.
+ Przesyłanie danych między klientem a serwerem jest szyfrowane za pomocą protokołu SSL/TLS.

SFTP jest bardziej bezpiecznym rozwiązaniem niż protokół FTP, ponieważ zapewnia szyfrowanie danych i uwierzytelnianie za pomocą protokołu SSH. SFTP jest zwykle dostępny na serwerach hostingowych i serwerach usług chmurowych, które zapewniają dostęp do plików poprzez protokół SFTP.


## 5.5. SMTP 

SMTP (Simple Mail Transfer Protocol) to protokół aplikacyjny wykorzystywany do przesyłania poczty elektronicznej w sieci internetowej. SMTP jest protokołem komunikacyjnym, który umożliwia wysyłanie i odbieranie wiadomości e-mail między różnymi serwerami poczty.

Kiedy użytkownik wysyła wiadomość e-mail, klient pocztowy wysyła ją na serwer poczty wychodzącej (SMTP), który następnie przesyła ją do serwera poczty przychodzącej (POP3 lub IMAP), gdzie odbiorca może odebrać wiadomość.

<p align="center">
Rys. 5.5.1. Działanie SMTP
<br>
  <img src="\assets\img\Sieci\17.png" width="650" alt="SMTP">
</p>

SMTP działa w następujący sposób:
+ Klient pocztowy nawiązuje połączenie z serwerem SMTP.
+ Klient przesyła dane uwierzytelniające, takie jak login i hasło.
+ Klient przesyła wiadomość e-mail na serwer SMTP, który następnie przesyła ją do serwera poczty przychodzącej.
+ Serwer poczty przychodzącej odbiera wiadomość i przechowuje ją w skrzynce pocztowej odbiorcy.
+ Odbiorca może pobrać wiadomość e-mail z serwera poczty przychodzącej za pomocą klienta pocztowego, takiego jak program pocztowy na komputerze lub aplikacja mobilna.


## 5.6. POP3

POP3 (Post Office Protocol 3) to protokół aplikacyjny wykorzystywany do odbierania poczty elektronicznej z serwera poczty przychodzącej. POP3 jest jednym z najpopularniejszych protokołów używanych do odbierania poczty elektronicznej.

Kiedy użytkownik chce pobrać wiadomości e-mail, klient pocztowy nawiązuje połączenie z serwerem POP3, pobiera wiadomości e-mail z serwera i przechowuje je na komputerze użytkownika. Pobrane wiadomości z serwera są zazwyczaj usuwane, chyba że użytkownik skonfiguruje klienta pocztowego w taki sposób, żeby wiadomości pozostały na serwerze.

<p align="center">
Rys. 5.6.1. Działanie POP3
<br>
  <img src="\assets\img\Sieci\18.png" width="650" alt="POP3">
</p>

POP3 działa w następujący sposób:
+ Klient pocztowy nawiązuje połączenie z serwerem POP3.
+ Klient przesyła dane uwierzytelniające, takie jak login i hasło.
+ Klient pobiera wiadomości e-mail z serwera POP3.
+ Pobrane wiadomości e-mail są przechowywane na komputerze użytkownika.
+ Jeśli użytkownik skonfiguruje klienta pocztowego w taki sposób, żeby wiadomości pozostały na serwerze, to pozostałe wiadomości są oznaczone jako przeczytane.

POP3 jest często używany w połączeniu z protokołem SMTP (Simple Mail Transfer Protocol), który służy do wysyłania wiadomości e-mail. POP3 jest jednym z najprostszych protokołów pocztowych, który zapewnia podstawową funkcjonalność, tzn. pobieranie i usuwanie wiadomości z serwera. W porównaniu z innymi protokołami pocztowymi, takimi jak IMAP (Internet Message Access Protocol), POP3 nie zapewnia takiej samej funkcjonalności, ale jest prostszy w obsłudze.


## 5.7. IMAP

IMAP (Internet Message Access Protocol) to protokół aplikacyjny wykorzystywany do odbierania poczty elektronicznej z serwera poczty przychodzącej. IMAP jest jednym z najbardziej zaawansowanych protokołów pocztowych i oferuje szereg funkcji, które umożliwiają użytkownikom dostęp do poczty elektronicznej z różnych urządzeń.

<p align="center">
Rys. 5.7.1. Działanie IMAP
<br>
  <img src="\assets\img\Sieci\19.png" width="650" alt="IMAP">
</p>

IMAP działa w następujący sposób:
+ Klient pocztowy nawiązuje połączenie z serwerem IMAP.
+ Klient przesyła dane uwierzytelniające, takie jak login i hasło.
+ Klient łączy się z serwerem poczty przychodzącej i pobiera informacje o wiadomościach e-mail, takie jak nagłówki, treść wiadomości i załączniki.
+ Użytkownik może przeglądać i zarządzać wiadomościami e-mail bezpośrednio na serwerze poczty przychodzącej, bez pobierania ich na swoje urządzenie.
+ Jeśli użytkownik zdecyduje się pobrać wiadomość e-mail, klient pocztowy pobiera tylko nagłówek i treść wiadomości, a załączniki pozostają na serwerze.

IMAP jest często używany w połączeniu z protokołem SMTP (Simple Mail Transfer Protocol), który służy do wysyłania wiadomości e-mail. W porównaniu z innymi protokołami pocztowymi, takimi jak POP3 (Post Office Protocol 3), IMAP oferuje bardziej zaawansowane funkcje i jest bardziej elastyczny w obsłudze, ale wymaga więcej zasobów serwera.


## 5.8. XMPP

XMPP (Extensible Messaging and Presence Protocol) to protokół komunikacyjny wykorzystywany do przesyłania wiadomości tekstowych, multimediów oraz informacji o dostępności użytkowników. XMPP jest protokołem open-source, co oznacza, że jego kod źródłowy jest dostępny publicznie i może być modyfikowany przez społeczność programistów.

XMPP jest zwykle stosowany w aplikacjach służących do komunikacji w czasie rzeczywistym, takich jak komunikatory internetowe i aplikacje do wideokonferencji. Protokół ten pozwala użytkownikom na prowadzenie rozmów w czasie rzeczywistym z innymi użytkownikami, wymianę plików, a także na tworzenie grupowych czatów.

XMPP wykorzystuje strukturę klient-serwer, w której serwer XMPP służy do połączenia między klientami. Protokół ten działa w oparciu o język XML (Extensible Markup Language), co umożliwia łatwe rozszerzanie i dostosowywanie funkcjonalności.

XMPP oferuje również funkcjonalność "presence", czyli informowanie innych użytkowników o dostępności i statusie online/offline. Dzięki temu użytkownicy mogą w prosty sposób sprawdzić, kiedy ich kontakty są dostępne i gotowe do rozmowy.

XMPP jest protokołem bardzo popularnym wśród deweloperów aplikacji do komunikacji, ze względu na jego elastyczność i możliwość rozszerzania funkcjonalności. XMPP jest również stosowany jako podstawowy protokół dla platformy komunikacyjnej Matrix, która umożliwia integrację różnych systemów komunikacyjnych.


## 5.9. LDAP

LDAP (Lightweight Directory Access Protocol) to protokół aplikacyjny, który umożliwia dostęp do katalogów informacji, takich jak katalogi użytkowników, grup, komputerów i zasobów w sieci. LDAP został zaprojektowany jako prosty i lekki protokół do pobierania informacji z katalogów.

<p align="center">
Rys. 5.9.1. Działanie LDAP
<br>
  <img src="\assets\img\Sieci\20.png" width="650" alt="LDAP">
</p>

LDAP działa w oparciu o model klient-serwer, w którym klient LDAP żąda informacji z serwera LDAP, który przechowuje katalog informacji. Protokół ten wykorzystuje protokół TCP/IP do komunikacji między klientem a serwerem.

LDAP oferuje wiele zalet, w tym:
+ Skalowalność: dzięki możliwości dodawania nowych wpisów i atrybutów, LDAP jest łatwy do skalowania w zależności od potrzeb organizacji.
+ Bezpieczeństwo: protokół LDAP oferuje wiele funkcji zabezpieczeń, takich jak szyfrowanie SSL/TLS i autentykację.
+ Efektywność: LDAP jest bardzo efektywnym protokołem, który pozwala na szybkie przeszukiwanie dużych katalogów.

LDAP jest często stosowany w firmach i organizacjach, które potrzebują centralnego katalogu użytkowników i zasobów. LDAP jest również często wykorzystywany do autentykacji użytkowników w systemach zarządzania tożsamością (IdM) oraz w aplikacjach do zarządzania tożsamością i dostępem (IAM).

<p align="center">
Rys. 5.9.2. Drzewo katalogów LDAP
<br>
  <img src="\assets\img\Sieci\21.png" width="650" alt="LDAP-1">
</p>

# 6. Protokoły zarządzania siecią

Protokoły zarządzania siecią to standardy i procedury, które umożliwiają administratorom sieci kontrolowanie i monitorowanie sieci oraz zarządzanie jej elementami. Protokoły te pozwalają na zdalne zarządzanie urządzeniami sieciowymi, jak również na zbieranie informacji o wydajności sieci oraz na monitorowanie jej stanu.

Protokoły zarządzania siecią są kluczowe dla prawidłowego funkcjonowania sieci komputerowych. Dzięki nim administratorzy są w stanie zarządzać urządzeniami sieciowymi, takimi jak routery, przełączniki, serwery i urządzenia końcowe. Protokoły te pozwalają na konfigurację urządzeń, zarządzanie nimi, monitorowanie ich pracy, a także na diagnozowanie problemów i wykrywanie awarii.

## 6.1. SNMP 

SNMP (Simple Network Management Protocol) to protokół zarządzania siecią, który jest stosowany do zdalnego monitorowania i zarządzania urządzeniami sieciowymi, takimi jak routery, przełączniki, serwery, drukarki, itp. Protokół SNMP pozwala administratorom na uzyskiwanie informacji o stanie urządzeń sieciowych, takich jak ilość przesłanych danych, zużycie pamięci, obciążenie procesora, itp. Protokół ten umożliwia również zmianę konfiguracji urządzeń, np. poprzez zmianę ustawień routera.

SNMP działa w oparciu o architekturę klient-serwer. Urządzenia sieciowe, zwane agentami, zbierają informacje o swoim stanie i przekazują je do serwera SNMP, nazywanego menedżerem. Menedżer SNMP może następnie analizować te informacje i podejmować decyzje w odniesieniu do zarządzanych urządzeń. Protokół SNMP wykorzystuje zestaw standardowych komunikatów i procedur do przekazywania informacji pomiędzy agentami i menedżerem.

Protokół SNMP jest szeroko stosowany w sieciach komputerowych, zwłaszcza w środowiskach korporacyjnych i w sieciach usługowych, gdzie istnieje potrzeba zdalnego monitorowania i zarządzania dużej liczby urządzeń. Wersja SNMPv3 zapewnia bezpieczne uwierzytelnianie i szyfrowanie, co umożliwia bezpieczne zarządzanie siecią.

<p align="center">
Rys. 6.1.1. Działanie protokołu SNMP
<br>
  <img src="\assets\img\Sieci\21.png" width="650" alt="SNMP">
</p>

Agenci rezydują na każdym urządzeniu sieciowym (routerze, punkcie dostępowym, stacji roboczej czy nawet drukarce obsługującej SNMP) i tworzą bazę danych zwaną MIB (ang. Management Information Base). W bazie przechowywane są obiekty opisujące właściwości danego urządzenia. Na żądanie zarządcy, obiekty te są udostępniane, ujawniając informacje takie, jak np. temperatura procesora, ilość wolnego miejsca na dysku, bieżące obciążenie interfejsu sieciowego czy liczba aktualnie zalogowanych użytkowników.

## 6.2. SSH

SSH (Secure Shell) to protokół komunikacyjny służący do bezpiecznego zdalnego logowania się i wykonywania poleceń na zdalnych komputerach. Protokół SSH umożliwia zdalne logowanie poprzez szyfrowanie danych przesyłanych pomiędzy klientem a serwerem, co znacznie zwiększa bezpieczeństwo przesyłanych informacji.

SSH jest stosowany do zdalnej administracji serwerów, przesyłania plików i wykonywania poleceń. Protokół SSH wykorzystuje asymetryczne szyfrowanie kluczem publicznym i prywatnym do uwierzytelniania użytkownika i serwera. Szyfrowanie danych SSH zapewnia również poufność i integralność przesyłanych danych.

Protokół SSH jest zastępcą protokołu Telnet, który był wcześniej wykorzystywany do zdalnej administracji systemów. SSH zapewnia większe bezpieczeństwo, ponieważ wszystkie dane przesyłane są szyfrowane, a proces uwierzytelniania jest bardziej bezpieczny niż w przypadku protokołu Telnet. W dzisiejszych czasach SSH jest standardem w większości systemów operacyjnych i jest szeroko stosowany do zdalnego zarządzania serwerami.

<p align="center">
Rys. 6.2.1. Działanie protokołu SSH
<br>
  <img src="\assets\img\Sieci\23.png" width="650" alt="SSH">
</p>

możliwość szyfrowania danych za pomocą nieco słabszego algorytmu DSA. Podczas instalacji serwera SSH tworzona jest para kluczy – klucz publiczny i prywatny serwera – służą one do szyfrowania i deszyfrowania komunikacji. Podczas pierwszego połączenia z serwerem, klient, zapisuje publiczny klucz serwera na swoim dysku, w pliku known_hosts.

<p align="center">
Rys. 6.2.2. Działanie protokołu SSH
<br>
  <img src="\assets\img\Sieci\24.png" width="650" alt="SSH-1">
</p>

Następnie tworzy tak zwany klucz sesji, który będzie stosowany do szyfrowania całej komunikacji. Klucz sesji zostaje zaszyfrowany kluczem publicznym otrzymanym wcześniej od serwera i jest do niego odsyłany. Od tego momentu cała komunikacja szyfrowana jest kluczem sesji.

<p align="center">
Rys. 6.2.3. Działanie protokołu SSH
<br>
  <img src="\assets\img\Sieci\25.png" width="650" alt="SSH-2">
</p>


## 6.3. RADIUS

RADIUS (Remote Authentication Dial-In User Service) to protokół autoryzacji i uwierzytelniania użytkowników zdalnego dostępu, takich jak użytkownicy dial-up, użytkownicy sieci bezprzewodowych i VPN. Protokół RADIUS działa w oparciu o architekturę klient-serwer i umożliwia centralne zarządzanie uwierzytelnianiem użytkowników.

<p align="center">
Rys. 6.2.3. Działanie protokołu RADIUS
<br>
  <img src="\assets\img\Sieci\26.png" width="650" alt="RADIUS">
</p>

Klient RADIUS jest zainstalowany na serwerze zdalnego dostępu, takim jak serwer VPN lub punkt dostępowy do sieci bezprzewodowej. Gdy użytkownik próbuje uzyskać dostęp do sieci, klient RADIUS przekierowuje żądanie uwierzytelnienia do serwera RADIUS. Serwer RADIUS przetwarza żądanie uwierzytelnienia i odpowiada na nie, przekazując informacje o poziomie uprawnień użytkownika do klienta RADIUS.

Protokół RADIUS umożliwia również śledzenie logowania użytkowników i zarządzanie ich uprawnieniami w zależności od ich roli w sieci. Użytkownicy mogą mieć różny poziom dostępu do zasobów sieciowych, a protokół RADIUS umożliwia administratorom zarządzanie tymi uprawnieniami.

RADIUS jest szeroko stosowany w sieciach korporacyjnych i usługowych, gdzie istnieje potrzeba zdalnego uwierzytelnienia użytkowników i zarządzania ich dostępem do zasobów sieciowych. Protokół ten jest niezbędny w przypadku infrastruktury VPN, gdzie użytkownicy zdalni muszą zostać uwierzytelnieni, aby uzyskać dostęp do sieci korporacyjnej.

<p align="center">
Rys. 6.2.3. Stosowanie RADIUS
<br>
  <img src="\assets\img\Sieci\27.png" width="650" alt="RADIUS-1">
</p>

# 7. Protokoły routingu

Protokoły routingu to zbiór reguł, które pozwalają na przekazywanie danych między różnymi sieciami komputerowymi. Ich zadaniem jest wyznaczanie najlepszej trasy dla pakietów danych i określanie, które sieci są osiągalne, a które nie. Protokoły te mogą działać w sieciach o różnej topologii, rozmiarze i złożoności.

Istnieją dwa rodzaje protokołów routingu: protokoły statyczne i dynamiczne. Protokoły statyczne wymagają ręcznego wprowadzenia informacji o trasach do każdego routera w sieci, co jest czasochłonne i może prowadzić do błędów. Protokoły dynamiczne automatycznie wyznaczają najlepsze trasy i są w stanie dostosować się do zmian w sieci.

<p align="center">
Rys. 7.1. Działanie protokołów routingu
<br>
  <img src="\assets\img\Sieci\28.png" width="650" alt="Routing">
</p>


## 7.1. RIP

RIP (Routing Information Protocol) to protokół routingu typu wektor odległości, który działa na warstwie sieciowej (warstwa 3 modelu OSI). RIP jest jednym z najstarszych protokołów routingu i został stworzony w celu umożliwienia automatycznego wymiany informacji o trasach między routerami w sieciach IP.

RIP działa na zasadzie przesyłania komunikatów z informacją o trasach między routerami. Każdy router z RIP musi wysyłać co określony czas swoją tabelę routingu, która zawiera informacje o trasach do innych sieci IP. Po otrzymaniu tabeli routingu od innych routerów, RIP aktualizuje swoją własną tabelę routingu i wybiera najlepszą trasę do danej sieci.

RIP stosuje metrykę hop count, czyli liczbę routerów, jakie musi przeskoczyć pakiet, aby dotrzeć do celu. Każdy router, który przekazuje pakiet, zwiększa wartość metryki hop count o 1. RIP pozwala na maksymalną liczbę 15 hopów, po przekroczeniu której sieć jest uznawana za niedostępną.

RIP jest stosowany w małych sieciach, gdzie nie ma dużego ruchu sieciowego. Jednym z głównych wad RIP jest jego powolne reagowanie na zmiany topologii sieci, co może spowodować powstanie pętli w sieci, co z kolei prowadzi do spadku wydajności sieci.

## 7.2. OSPF

OSPF (Open Shortest Path First) jest to protokół routingu typu link-state, który używa algorytmu Dijkstra do wyznaczania najkrótszych ścieżek do celu w sieci. Protokół OSPF zapewnia szybką konwergencję sieci, czyli szybkie dostosowywanie się sieci do zmian w topologii sieci. Protokół OSPF jest zwykle stosowany w dużych sieciach, ze względu na jego zdolność do obsługi wielu ścieżek i wsparcie dla klasycznych sieci hierarchicznych.

OSPF używa link-state database (LSDB), która składa się z wszystkich informacji o topologii sieci, takie jak adresy IP, metryki i status połączenia. Każdy router OSPF w sieci wysyła pakiet "Hello" na swoich interfejsach w celu nawiązania i utrzymania łączności z innymi routerami OSPF w sieci. Wszystkie połączone routery tworzą drzewo połączeń, które reprezentuje topologię sieci.

OSPF umożliwia tworzenie różnych obszarów w sieci, co pomaga zmniejszyć obciążenie sieci i zwiększyć wydajność routingu. W ramach jednego obszaru, wszystkie routery mają pełną wiedzę o topologii sieci, a w ramach różnych obszarów, informacje o topologii są wymieniane tylko między routerami brzegowymi, co zmniejsza ilość przesyłanych danych.

Protokół OSPF zapewnia również wiele funkcji bezpieczeństwa, takich jak uwierzytelnianie, uwierzytelnianie klucza publicznego (PKI) i wsparcie dla protokołu IPsec. Protokół OSPF jest uważany za jeden z najbardziej zaawansowanych protokołów routingu i jest szeroko stosowany w sieciach przedsiębiorstw i usług dostępowych do internetu.

## 7.3. BGP 

BGP (Border Gateway Protocol) to protokół routingu stosowany w sieciach ISP (Internet Service Provider) i AS (Autonomous System), który umożliwia wymianę informacji o trasach między bramami (ruterami) między różnymi AS. BGP jest protokołem opartym na wektorach odległości, w którym głównym celem jest wybór najkrótszej ścieżki między dwoma punktami.

W sieciach ISP BGP jest często wykorzystywany jako protokół do wymiany informacji o trasach między różnymi dostawcami usług internetowych. Każdy dostawca usług internetowych posiada własny AS, a BGP umożliwia wymianę informacji o trasach między różnymi AS. BGP umożliwia także określenie priorytetów dla różnych tras i wybór najlepszej trasy w zależności od określonych kryteriów.

W BGP wyróżnia się dwa typy wiadomości: UPDATE i KEEPALIVE. Wiadomości UPDATE są używane do przekazywania informacji o trasach między różnymi bramami. Wiadomości KEEPALIVE są używane do potwierdzania, że połączenie między dwoma bramami jest aktywne.

BGP umożliwia stosowanie polityk routingu, które pozwalają dostawcom usług internetowych kontrolować ruch w sieci. Dzięki temu dostawcy usług internetowych mogą kontrolować ruch między różnymi AS i zwiększyć wydajność sieci. Jednakże, ze względu na złożoność i skalowalność BGP, jego konfiguracja i utrzymanie wymaga doświadczenia i specjalistycznej wiedzy.

## 7.4. IS-IS

IS-IS (Intermediate System to Intermediate System) to protokół routingu, który używa się głównie w sieciach typu ISP i w dużych sieciach korporacyjnych. IS-IS działa na poziomie warstwy 2 i warstwy 3 modelu OSI, co oznacza, że obsługuje zarówno routowanie IP, jak i nierutowalnych protokołów warstwy 2, takich jak Ethernet.

<p align="center">
Rys. 7.4.1. IS-IS Routing
<br>
  <img src="\assets\img\Sieci\29.png" width="650" alt="IS-IS">
</p>

W protokole IS-IS każde urządzenie sieciowe, zwane systemem pośredniczącym, posiada identyfikator systemu pośredniczącego (System ID) i adres IP. W sieci IS-IS każdy system pośredniczący zna swoich bezpośrednich sąsiadów i wymienia z nimi informacje o topologii sieci, a te informacje są następnie przesyłane do pozostałych systemów pośredniczących.

IS-IS wykorzystuje algorytm SPF (Shortest Path First), aby obliczyć najkrótszą ścieżkę między dwoma systemami pośredniczącymi. Algorytm ten oblicza ścieżki do wszystkich celów w sieci i wybiera najkrótszą ścieżkę. Przy czym do wyboru najlepszej ścieżki uwzględnia się koszty połączeń między systemami pośredniczącymi.

W IS-IS istnieją dwie główne rodzaje systemów pośredniczących: systemy pośredniczące wewnętrzne (IS-IS Interior Gateway System, IS-IS-IGP) i systemy pośredniczące zewnętrzne (IS-IS-EGP). Systemy pośredniczące wewnętrzne służą do wymiany informacji routingowej w obrębie jednej domeny routingu, natomiast systemy pośredniczące zewnętrzne służą do wymiany informacji z innymi domenami routingu.

IS-IS jest stosowany w sieciach o dużych rozmiarach i ma wiele zalet, takich jak zdolność do szybkiej konwergencji, łatwość konfiguracji i skalowalność. Jednak jego wadą jest to, że jest bardziej skomplikowany w konfiguracji niż niektóre inne protokoły routingu i wymaga specjalistycznej wiedzy, aby go skonfigurować i zarządzać.

# 8. Protokoły bezpieczeństwa

Protokoły bezpieczeństwa to specjalne protokoły i standardy służące do zapewnienia bezpieczeństwa w sieciach komputerowych i systemach informatycznych. Obejmują one szereg zasad i procedur, które mają na celu ochronę poufności, integralności i dostępności informacji w sieci.

## 8.1. SSL i SSL Decryption 

SSL (Secure Sockets Layer) to protokół komunikacyjny służący do zabezpieczania transmisji danych w sieciach komputerowych. SSL został zastąpiony przez protokół TLS (Transport Layer Security), który jest jego następcą.

SSL/TLS stosuje kryptografię symetryczną i asymetryczną, aby zabezpieczyć dane przesyłane pomiędzy serwerem a klientem. Protokół ten umożliwia szyfrowanie i deszyfrowanie danych w trakcie transmisji oraz uwierzytelnienie serwera i klienta za pomocą certyfikatów cyfrowych.

SSL Decryption to proces dekodowania i odszyfrowywania danych przesyłanych przez protokół SSL/TLS w celu uzyskania dostępu do ich zawartości. Proces ten jest wykorzystywany przez niektóre narzędzia bezpieczeństwa, takie jak firewall, IDS/IPS czy rozwiązania DLP, w celu zidentyfikowania i zabezpieczenia przed niepożądanymi aktywnościami, takimi jak ataki malware, wykradanie danych itp.

SSL Decryption może być realizowany w różny sposób. Jednym z nich jest instalacja certyfikatów SSL na urządzeniach sieciowych, co umożliwia odczytanie i analizę danych przesyłanych przez protokół SSL/TLS. Innym sposobem jest wykorzystanie rozwiązania proxy SSL, które pozwala na przeprowadzenie dekodowania i analizy danych SSL/TLS na dedykowanym urządzeniu.

Warto zauważyć, że SSL Decryption może wpłynąć na prywatność użytkowników, ponieważ narzędzia te mogą dekodować i analizować również prywatne dane, takie jak hasła, numery karty kredytowej itp. W związku z tym, stosowanie rozwiązania SSL Decryption powinno być poprzedzone staranną analizą i przemyśleniem.

### Jak działa szyfrowanie SSL/TLS i dlaczego jest to ważne dla bezpieczeństwa danych?

Szyfrowanie SSL/TLS jest kluczowym elementem zapewnienia bezpieczeństwa danych w Internecie. Działa ono w następujący sposób:
+ Nawiązanie połączenia: przeglądarka internetowa (klient) inicjuje połączenie z serwerem internetowym
+ Ustanowienie parametrów połączenia: przeglądarka i serwer uzgadniają wspólny algorytm szyfrowania i klucze szyfrujące, które będą używane podczas przesyłania danych.
+ Wymiana kluczy publicznych: serwer wysyła swój klucz publiczny do przeglądarki, która go akceptuje.
+ Szyfrowanie danych: przeglądarka używa klucza publicznego serwera do zaszyfrowania klucza sesji, który jest następnie wysyłany do serwera. Serwer odszyfrowuje klucz sesji i używa go do szyfrowania danych, które są następnie przesyłane do przeglądarki.
+ Kontrola integralności danych: podczas przesyłania danych między przeglądarką a serwerem, każda wiadomość jest dodatkowo szyfrowana i kontrolowana pod kątem integralności, aby uniemożliwić ich zmodyfikowanie podczas przesyłania.

Szyfrowanie SSL/TLS jest ważne dla bezpieczeństwa danych, ponieważ uniemożliwia przechwycenie danych w trakcie przesyłania, a także ich odczytanie przez niepowołane osoby. Bez SSL/TLS, dane przesyłane między przeglądarką a serwerem są otwarte i mogą być przechwycone przez osoby trzecie, co naraża je na niebezpieczeństwo kradzieży i wykorzystania w niepożądany sposób. Dlatego też SSL/TLS jest niezbędne do zapewnienia bezpieczeństwa danych w Internecie, w szczególności w przypadku transakcji finansowych, przesyłania poufnych informacji oraz przesyłania danych osobowych.

Wśród narzędzi stosowanych do implementacji SSL Decryption są firewall'e sieciowe, NGFW (Next Generation Firewall), Proxy serwery, IDS/IPS (Intrusion Detection/Prevention System), i WAF (Web Application Firewall). Te narzędzia działają poprzez dekodowanie ruchu SSL, analizę danych i przetwarzanie ich w celu zapewnienia bezpieczeństwa.

Istnieje wiele narzędzi i technik, które mogą pomóc w monitorowaniu i zarządzaniu ruchem SSL/TLS, takich jak rozwiązania DLP (Data Loss Prevention), Narzędzia do monitorowania SSL/TLS, jak np. Wireshark, i techniki kontroli ruchu sieciowego, takie jak optymalizacja ruchu SSL/TLS i wykorzystanie mechanizmów szyfrowania z odpowiednim kluczem publicznym.


### SSL Decryption - FortiGate (Fortinet) - Serwer. Jak odbywa się odszyfrowywanie?

Aby przeprowadzić SSL Decryption, urządzenie FortiGate musi być połączone między punktem końcowym (np. komputerem) a serwerem, z którym chcemy się połączyć (np. serwerem www). W typowej konfiguracji sieciowej, FortiGate będzie działał jako brama sieciowa, kontrolując ruch między punktem końcowym a serwerem.

Jeśli chodzi o SSL Decryption, to po stronie FortiGate musi być skonfigurowane wiele elementów. Przede wszystkim musi zostać utworzona reguła firewalla, która przekieruje ruch, który chcemy odszyfrować, do odpowiedniego profilu SSL Inspection. W profilu tym określamy, jakie certyfikaty SSL/TLS są dozwolone, jakie algorytmy szyfrowania są akceptowane, a także jakie akcje podejmowane są w przypadku wykrycia nieprawidłowości.

Ważnym elementem jest również certyfikat SSL, który jest wymagany do ustanowienia połączenia między FortiGate a serwerem docelowym. W przypadku, gdy połączenie jest odszyfrowywane, FortiGate generuje własny certyfikat, który jest podpisany przez wewnętrzne centrum certyfikacji. Ten certyfikat jest następnie przesyłany do punktu końcowego, który musi go zaakceptować, aby połączenie zostało ustanowione.

Po ustanowieniu połączenia SSL/TLS między punktem końcowym a serwerem, ruch jest przekazywany do FortiGate, który przeprowadza odszyfrowanie i analizę pakietów. Jeśli pakiet jest uznany za złośliwy lub podejrzany, FortiGate może podjąć odpowiednie działania, takie jak zablokowanie połączenia, wysłanie powiadomienia o incydencie itp.

Ostatecznie, zdeszyfrowany ruch jest przekazywany do serwera docelowego, a odpowiedź serwera jest szyfrowana przez FortiGate i przesyłana z powrotem do punktu końcowego.

### Krok po kroku, jak dokładnie odbywa się ten proces:

1. Inicjacja połączenia SSL/TLS:
- Klient inicjuje połączenie SSL/TLS z serwerem, wysyłając do niego żądanie nawiązania połączenia.
- FortiGate przeprowadza analizę żądania i w razie potrzeby blokuje połączenie lub przechodzi do kolejnego etapu.
2. Przekierowanie ruchu:
- FortiGate przekierowuje ruch związany z połączeniem SSL/TLS do serwera proxy SSL.
- Serwer proxy SSL otrzymuje żądanie klienta i wysyła własne żądanie do serwera docelowego.

3. Nawiązanie połączenia między serwerem proxy SSL a serwerem docelowym:
- Serwer proxy SSL nawiązuje połączenie z serwerem docelowym i inicjuje proces handshake SSL/TLS z wykorzystaniem własnego certyfikatu SSL/TLS.
- Po ustanowieniu połączenia SSL/TLS, serwer proxy SSL odbiera certyfikat serwera docelowego i przesyła go do FortiGate.

4. Weryfikacja certyfikatu serwera docelowego:
- FortiGate pobiera certyfikat serwera docelowego i sprawdza jego ważność i poprawność.
- Jeśli certyfikat jest nieprawidłowy lub nieznany, FortiGate blokuje połączenie lub zastępuje go własnym certyfikatem.

5. Generowanie nowego klucza prywatnego:
- FortiGate generuje nowy klucz prywatny i certyfikat dla połączenia między klientem a serwerem docelowym.
- Wszystkie dane przesyłane między klientem a serwerem docelowym będą szyfrowane przy użyciu nowego klucza prywatnego.

6. Ustanowienie połączenia między klientem a serwerem docelowym:
- Serwer proxy SSL nawiązuje połączenie między klientem a serwerem docelowym przy użyciu nowego klucza prywatnego.
- FortiGate monitoruje ruch między klientem a serwerem docelowym i przeprowadza analizę treści w celu wykrycia niebezpiecznych lub niepożądanych aktywności.


## 8.2. IPSec

IPSec (Internet Protocol Security) to protokół bezpieczeństwa, który zapewnia poufność, integralność i uwierzytelnianie transmisji danych w sieciach IP. Protokół IPSec działa na warstwie sieciowej (warstwie 3) modelu OSI i może być używany do zabezpieczania różnych protokołów, takich jak IP, TCP, UDP i ICMP.

IPSec składa się z dwóch głównych protokołów: protokołu Authentication Header (AH) i protokołu Encapsulating Security Payload (ESP). Protokół AH zapewnia integralność danych, uwierzytelnianie źródła oraz ochronę przed atakami typu replay. Protokół ESP zapewnia poufność danych, integralność oraz uwierzytelnianie, a także może być stosowany do tunelowania ruchu sieciowego przez publiczną sieć.

Protokół IPSec może być stosowany w różnych konfiguracjach, takich jak tryb transportowy i tryb tunelowania. W trybie transportowym jedynie dane są szyfrowane, podczas gdy nagłówek IP jest zachowany w postaci niezaszyfrowanej. W trybie tunelowania cały ruch sieciowy jest szyfrowany i przesyłany przez tunel IPSec.

IPSec może być stosowany do różnych zastosowań, takich jak zdalny dostęp do sieci, sieci VPN, wirtualne sieci prywatne, zdalne zarządzanie siecią, a także do zabezpieczania transmisji w chmurze.

## 8.3. VPN

VPN (Virtual Private Network) to technologia umożliwiająca tworzenie prywatnych i bezpiecznych połączeń między dwoma lub więcej urządzeniami poprzez publiczną sieć, taką jak Internet. Za pomocą VPN można łączyć się z siecią prywatną (LAN) z dowolnego miejsca na świecie, jakby się znajdowało fizycznie w biurze, bez narażania danych na ryzyko przechwycenia przez osoby trzecie.

Ważną funkcją VPN jest szyfrowanie danych przesyłanych między urządzeniami. To oznacza, że wszystkie dane, które są przesyłane między urządzeniami, są zaszyfrowane i nie mogą być odczytane przez osoby trzecie. VPN zapewnia również uwierzytelnienie, czyli proces weryfikacji tożsamości użytkownika przed udostępnieniem dostępu do sieci prywatnej. Ważną funkcją VPN jest szyfrowanie danych przesyłanych między urządzeniami. To oznacza, że wszystkie dane, które są przesyłane między urządzeniami, są zaszyfrowane i nie mogą być odczytane przez osoby trzecie. VPN zapewnia również uwierzytelnienie, czyli proces weryfikacji tożsamości użytkownika przed udostępnieniem dostępu do sieci prywatnej.

Istnieją różne rodzaje VPN, w tym:
+ VPN zdalnego dostępu - umożliwia pracownikom zdalne łączenie się z siecią firmową z dowolnego miejsca na świecie.
+ VPN site-to-site - umożliwia łączenie ze sobą różnych sieci LAN znajdujących się w różnych lokalizacjach geograficznych, tworząc jedną wirtualną sieć.
+ VPN klient-serwer - umożliwia łączenie się z serwerem VPN z poziomu aplikacji na urządzeniu, takiej jak klient VPN, który umożliwia łatwe połączenie z siecią prywatną.

## 8.4. Kerberos

Kerberos to protokół uwierzytelniania sieciowego służący do zapewnienia bezpieczeństwa w sieciach komputerowych. Nazwa pochodzi od trójgłowego psa Cerbera z mitologii greckiej, który strzegł wejścia do Hadesu.

Protokół Kerberos działa na zasadzie wymiany kluczy kryptograficznych między klientem a serwerem. Dzięki temu klient może się uwierzytelnić przed serwerem i uzyskać dostęp do zasobów sieciowych.

Główne zalety protokołu Kerberos to:
+ Bezpieczeństwo: protokół Kerberos zapewnia bezpieczeństwo w sieci poprzez szyfrowanie przesyłanych danych i uwierzytelnianie klientów i serwerów.
+ Skalowalność: Kerberos może obsługiwać duże sieci z wieloma klientami i serwerami.
+ Łatwość w zarządzaniu: Kerberos umożliwia centralizowane zarządzanie uwierzytelnianiem i autoryzacją dostępu do zasobów.
Protokół Kerberos jest szeroko stosowany w systemach operacyjnych, takich jak Windows i Unix/Linux, a także w aplikacjach internetowych.


## 8.5. S/MIME

S/MIME (Secure/Multipurpose Internet Mail Extensions) to protokół bezpieczeństwa, który zapewnia poufność, integralność i uwierzytelnienie dla e-maili. Protokół S/MIME działa poprzez dodanie kryptograficznych funkcji do standardowych protokołów pocztowych, takich jak SMTP, POP i IMAP.

Główne funkcje S/MIME to:
+ szyfrowanie treści wiadomości, co oznacza, że tylko odbiorca, który zna klucz prywatny, może odszyfrować wiadomość,
+ podpisywanie wiadomości, co umożliwia odbiorcy sprawdzenie, że wiadomość nie została zmodyfikowana w trakcie przesyłki,
+ uwierzytelnianie nadawcy, co zapewnia odbiorcy, że wiadomość pochodzi od rzeczywistego nadawcy, a nie od oszusta podszywającego się pod nadawcę.

Protokół S/MIME jest stosowany głównie w firmach i instytucjach, które wymieniają poufne informacje drogą elektroniczną, takie jak umowy, dokumenty i inne informacje wrażliwe.

# 9. Protokoły dostępu do sieci

## 9.1. DHCP 

Dynamic Host Configuration Protocol (DHCP) jest protokołem używanym w sieciach komputerowych do automatycznego przydzielania adresów IP oraz innych ustawień konfiguracyjnych, takich jak maski podsieci, bramy domyślnej i serwery DNS.

Dzięki DHCP, komputery i inne urządzenia w sieci mogą automatycznie uzyskać adres IP, zamiast wymagać ręcznej konfiguracji przez administratora sieci. DHCP działa na zasadzie klient-serwer, gdzie klient wysyła zapytanie do serwera DHCP o przydzielenie mu adresu IP i innych parametrów konfiguracyjnych.

Aby komputery z systemem Windows, pobierały adresy z serwera DHCP, w konfiguracji sieci należy wybrać opcję "Uzyskaj adres IP automatycznie".

<p align="center">
Rys. 9.1.1. Działanie DHCP 
<br>
  <img src="\assets\img\Sieci\30.png" width="650" alt="DHCP">
</p>

Aby komputery z systemem Windows, pobierały adresy z serwera DHCP, w konfiguracji sieci należy wybrać opcję "Uzyskaj adres IP automatycznie".

<p align="center">
Rys. 9.1.2. Ustawienia DHCP
<br>
  <img src="\assets\img\Sieci\31.png" width="650" alt="DHCP-1">
</p>

## 9.2. DNS

DNS (Domain Name System) to protokół komunikacyjny używany w sieciach komputerowych do przetwarzania nazw domenowych na adresy IP i odwrotnie. Jest to jeden z kluczowych protokołów internetowych, który umożliwia przeglądanie stron internetowych oraz wysyłanie i odbieranie poczty elektronicznej.

DNS działa w sposób hierarchiczny, co oznacza, że istnieją serwery DNS na różnych poziomach sieci, a każdy z tych serwerów zawiera informacje o nazwach domenowych i ich odpowiadających adresach IP. Proces przetwarzania nazw domenowych na adresy IP nazywa się rozwiązywaniem nazw.

Kiedy użytkownik wpisuje adres URL do przeglądarki internetowej, przeglądarka wysyła zapytanie do serwera DNS, aby rozwiązać nazwę domenową. Serwer DNS następnie wyszukuje odpowiedni adres IP dla tej nazwy i zwraca go do przeglądarki, która następnie nawiązuje połączenie z serwerem internetowym, na którym znajduje się witryna internetowa.

DNS jest krytycznym protokołem dla działania Internetu, ponieważ umożliwia łatwe i intuicyjne korzystanie z witryn internetowych poprzez używanie nazw domenowych zamiast adresów IP.

Klient wysyła żądanie do serwera DNS, a ten sprawdza, czy w swojej bazie posiada dany rekord. Jeśli tak przekształca nazwę na adres IP i odsyła do klienta:

<p align="center">
Rys. 9.2.1. Pytanie do serwera
<br>
  <img src="\assets\img\Sieci\32.png" width="650" alt="DNS">
</p>

Jeśli nie, to kontaktuje się z innymi serwerami, aby te dany rekord wyszukały w swoich bazach:

<p align="center">
Rys. 9.2.1. Pytanie do innych serwerów
<br>
  <img src="\assets\img\Sieci\33.png" width="650" alt="DNS-1">
</p>


## 9.3. ARP 

Kiedy jako użytkownicy sieci, wysyłamy dane z jednego urządzenia do drugiego to albo znamy jego adres IP, albo nazwę domenową co pozwala nam taką transmisję wykonać. Gorzej jest już z adresami MAC, na ich podstawie, my użytkownicy sieci, nie definiujemy odbiorców danych, to dzieje się poza nami. W sieciach komputerowych, opartych na protokole IPv4, do uzyskiwania informacji o adresie MAC danego urządzenia służy protokół zwany ARP (ang. Address Resolution Protocol).

ARP to mechanizm pozwalający na odwzorowanie adresu logicznego, czyli IP na adres fizyczny, czyli MAC. Załóżmy, że komputer chcąc przesłać dane do innego urządzenia zna jego adres IP, ale nie zna adresu MAC. Aby ten adres poznać, komputer będący nadawcą danych, zanim te konkretne dane wyśle, tworzy rozgłoszeniową ramkę ARP, która rozsyłana jest do wszystkich urządzeń w tej samej sieci. W polu adresu źródłowego takiej ramki zapisywany jest adres komputera, który przygotował taką ramkę, a w polu adresu docelowego, rozgłoszeniowy adres MAC: FF-FF-FF-FF-FF-FF.

<p align="center">
Rys. 9.3.1. Tablica ARP
<br>
  <img src="\assets\img\Sieci\34.png" width="650" alt="ARP">
</p>


Każde z urządzeń, które odbierze ramkę, dekapsuluje ją do postaci pakietu i sprawdza, czy w polu docelowym adres IP jest jego adres. Jeśli w polu docelowy adres IP będzie inny adres niż jego, to zignoruje pakiet, jeśli natomiast to jego adres IP, utworzy nową ramkę, w której zapisany będzie jego adres MAC i przekaże ją do przesłania.

<p align="center">
Rys. 9.3.2. Tablica ARP
<br>
  <img src="\assets\img\Sieci\35.png" width="650" alt="ARP-1">
</p>

Teraz już komputer, który wysłał rozgłoszeniową ramkę wie jaki adres fizyczny ma urządzenie, z którym chce się skomunikować i taką komunikację może rozpocząć. Informacje o odwzorowaniu adresu IP na adres MAC zapisywane są w tablicy ARP każdego urządzenia, tak aby można je było wykorzystać w późniejszym czasie.


# 10. Konfiguracja i administracja sieci

Konfiguracja i administracja sieci to procesy związane z zaprojektowaniem, ustawieniem i zarządzaniem siecią komputerową. Wymaga to rozległej wiedzy z zakresu sieci komputerowych, włączając w to topologie sieciowe, adresowanie IP, protokoły routingu, protokoły bezpieczeństwa, zarządzanie urządzeniami sieciowymi i wiele innych.

Podczas konfiguracji sieci należy odpowiednio skonfigurować urządzenia sieciowe, takie jak przełączniki, routery, punkty dostępowe, serwery DHCP i DNS, a także zapewnić odpowiednie zabezpieczenia dla sieci. Administracja sieci to codzienne zarządzanie siecią, w tym diagnozowanie problemów, monitorowanie wydajności, aktualizowanie oprogramowania i sterowników oraz stosowanie polityk bezpieczeństwa.

Dobrze zaprojektowana i zarządzana sieć może przyczynić się do zwiększenia wydajności, bezpieczeństwa i dostępności usług sieciowych, co przekłada się na lepsze doświadczenia użytkowników końcowych.

### Symulatory programów konfiguracyjnych urządzeń sieciowych:

Symulatory programów konfiguracyjnych urządzeń sieciowych to narzędzia, które pozwalają symulować działanie różnych urządzeń sieciowych, takich jak routery, przełączniki, serwery DHCP i wiele innych. Symulatory te pozwalają na testowanie konfiguracji sieci i zrozumienie, jak różne urządzenia i protokoły sieciowe działałyby w różnych scenariuszach.

Dzięki symulatorom programów konfiguracyjnych urządzeń sieciowych można na przykład przetestować i zrozumieć, jak działa protokół routingu OSPF, jak skonfigurować sieć VLAN lub jak działa konfiguracja QoS na routerze. Symulatory te pozwalają również na eksperymentowanie z różnymi scenariuszami i konfiguracjami bez konieczności korzystania z rzeczywistych urządzeń, co pozwala na oszczędność kosztów i czasu.

Przykłady popularnych symulatorów programów konfiguracyjnych urządzeń sieciowych to GNS3, Packet Tracer, EVE-NG, NetSim i Boson NetSim. Każdy z tych symulatorów ma swoje unikalne cechy i funkcjonalności, ale każdy z nich zapewnia realistyczne środowisko testowe, w którym można eksperymentować z różnymi konfiguracjami sieciowymi i protokołami.


## 10.1. Zarządzanie IP

Zarządzanie adresami IP to proces przypisywania i kontrolowania adresów IP w sieciach komputerowych. Adres IP jest unikalnym identyfikatorem urządzenia sieciowego, który umożliwia komunikację z innymi urządzeniami w sieci. Zarządzanie adresami IP jest ważne w sieciach, ponieważ umożliwia kontrolowanie adresów IP, ich przypisywanie i usuwanie, a także umożliwia łatwe śledzenie i zarządzanie zasobami sieciowymi.

## 10.1.1. Dzelenie na podsieci

### Zadanie:

Podany jest adres ip w postaci: *192.168.1.145* oraz maska *255.255.255.128*. Na podstawie tych danych należy obliczyć:
+ adres sieci,
+ adres rozgłoszeniowy,
+ maksymalną liczbę hostów,

oraz wskazać adres pierwszego i ostatniego hosta w sieci.

Rozwiązanie: 

1. Obliczamy adres sieci

Zmieniamy adres IP oraz maskę na postać binarną

<p align="center">
Rys. 10.1.1.1. Zmiana adresów
<br>
  <img src="\assets\img\Sieci\36.png" width="650" alt="Dzielenie">
</p>

Na otrzymanych liczbach binarnych wykonujemy operację AND (czyli mnożymy liczby w kolumnach)

<p align="center">
Rys. 10.1.1.2. Operacja AND
<br>
  <img src="\assets\img\Sieci\37.png" width="650" alt="Dzielenie-1">
</p>

Otrzymaną postać binarną konwertujemy na liczbę dziesiętną

<p align="center">
Rys. 10.1.1.3. Konwertacja na liczbę dziesiętną
<br>
  <img src="\assets\img\Sieci\38.png" width="650" alt="Dzielenie-2">
</p>

2. Obliczamy adres rozgłoszeniowy

Na postaci binarnej maski wykonujemy operację logiczną NOT (jedynki zamieniamy na zera, a zera na jedynki)

<p align="center">
Rys. 10.1.1.4. Operacja NOT
<br>
  <img src="\assets\img\Sieci\39.png" width="650" alt="Dzielenie-3">
</p>

Zamieniamy otrzymaną liczbę binarną na postać dziesiętną

<p align="center">
Rys. 10.1.1.5. Zamiana na postac dziesiętna
<br>
  <img src="\assets\img\Sieci\40.png" width="650" alt="Dzielenie-4">
</p>

Otrzymaną liczbę dziesiętną dodajemy do adresu sieci

<p align="center">
Rys. 10.1.1.6. Dodanie do adresu sieci
<br>
  <img src="\assets\img\Sieci\41.png" width="650" alt="Dzielenie-5">
</p>

3. Obliczamy maksymalną liczbę hostów w sieci

Obliczając maksymalną liczbę hostów w sieci korzystamy ze wzoru

<p align="center">
Rys. 10.1.1.7. Wzór
<br>
  <img src="\assets\img\Sieci\42.png" width="650" alt="Dzielenie-6">
</p>

przypominam, że skrócony zapis maski to liczba jedynek w jej postaci binarnej


<p align="center">
Rys. 10.1.1.8. Co w naszym przypadku daje
<br>
  <img src="\assets\img\Sieci\43.png" width="650" alt="Dzielenie-7">
</p>

Na koniec wskazujemy adres pierwszego i ostatniego hosta w sieci

Jeśli adres sieci ma postać 192.168.1.128 to adres pierwszego hosta będzie miał postać *192.168.1.129*

Jeśli natomiast adres rozgłoszeniowy ma postać 192.168.1.255 to adres ostatniego hosta będzie miał postać *192.168.1.254*


Podsumowując:

+ Adres sieci: *192.168.1.128*
+ Adres rozgłoszeniowy: *192.168.1.255*
+ Liczba hostów: *126*
+ Pierwszy host: *192.168.1.129*
+ Ostatni host: *192.168.1.254*

Podział na podsieci:

<p align="center">
Rys. 10.1.1.9. Podział na podsieci
<br>
  <img src="\assets\img\Sieci\44.png" width="650" alt="Dzielenie-8">
</p>


## 10.1.2. Adresacja warstwy drugiej i trzeciej

Adresacja w warstwie drugiej oraz trzeciej sieci komputerowej to proces nadawania adresów urządzeniom, aby umożliwić im komunikację w sieci. Adresy te pozwalają na identyfikację urządzeń i określenie, jakie dane powinny być przesyłane do których urządzeń.

W warstwie drugiej, czyli warstwie łącza danych (ang. Data Link Layer), adresacja odbywa się za pomocą adresów MAC (Media Access Control). 
W warstwie trzeciej, czyli warstwie sieciowej (ang. Network Layer), adresacja odbywa się za pomocą adresów IP (Internet Protocol). 

W celu nadawania adresów w warstwie drugiej i trzeciej stosuje się różne metody, takie jak ręczne przypisywanie adresów przez administratora sieci, automatyczne przypisywanie adresów przez serwer DHCP (Dynamic Host Configuration Protocol) lub wykorzystanie protokołu ARP (Address Resolution Protocol), który umożliwia mapowanie adresów MAC na adresy IP.

## 10.2. VLAN

VLAN (Virtual Local Area Network) to technologia, która umożliwia podział sieci fizycznej na logiczne segmenty, co pozwala na lepszą organizację sieci, zwiększenie jej wydajności i bezpieczeństwa. VLANy umożliwiają grupowanie urządzeń sieciowych na podstawie różnych kryteriów, takich jak lokalizacja geograficzna, funkcja, departament, itp.

Przykładowo, w dużym przedsiębiorstwie może istnieć potrzeba podziału sieci na kilka VLANów, takich jak:
+ VLAN dla działu finansowego,
+ VLAN dla działu IT,
+ VLAN dla działu produkcji,
+ VLAN dla gości,
+ VLAN dla urządzeń bezprzewodowych.

Każdy z tych VLANów może mieć swoje własne reguły bezpieczeństwa, adresację IP, tablice routingu, itp. Jednakże, gdy mamy kilka VLANów, to w sieci fizycznej potrzebujemy kilka interfejsów VLAN. Tutaj wkracza do akcji protokół STP (Spanning Tree Protocol).

### Różnica między VLAN tagging a VLAN trunk:

VLAN tagging to proces oznaczania ramek sieciowych za pomocą specjalnego identyfikatora VLAN (tzw. tagu), który pozwala na ich przesyłanie w obrębie sieci VLAN. Dzięki temu ramek z różnych sieci VLAN można przesyłać przez ten sam fizyczny interfejs sieciowy (np. kabel Ethernet), ale nadal zachować ich odrębność i zapewnić poprawne przekierowywanie do właściwego segmentu sieci. VLAN tagging umożliwia przełącznikom sieciowym rozróżnienie ramek sieciowych i kierowanie ich do odpowiednich VLAN-ów.

VLAN trunking to natomiast mechanizm umożliwiający przesyłanie ramek oznaczonych tagami VLAN przez ten sam fizyczny interfejs sieciowy (np. kabel Ethernet) pomiędzy dwoma przełącznikami sieciowymi lub między przełącznikiem a urządzeniem sieciowym (np. routerem). Dzięki temu w jednym fizycznym interfejsie można przesyłać ruch z wielu różnych sieci VLAN.

W praktyce VLAN tagging i VLAN trunking są często stosowane razem, ponieważ umożliwiają efektywne wykorzystanie infrastruktury sieciowej przy jednoczesnym zachowaniu logiki segmentacji sieci.

### Segmentacja używana w VLAN i VLAN tagging:

Segmentacja sieci wirtualnych (VLAN) jest techniką dzielenia jednej sieci fizycznej na wiele logicznych sieci.  Segmentacja sieci VLAN jest realizowana za pomocą przełączników sieciowych.

### Broadcast, multicast i unicast:

Broadcast: to metoda transmisji, w której dane są przesyłane do wszystkich urządzeń w sieci. Broadcast jest używany, gdy potrzebujemy przesłać informację do wszystkich urządzeń w sieci. W przypadku sieci VLAN, broadcast będzie dotyczył tylko urządzeń w tej samej sieci VLAN.

Multicast: to metoda transmisji, w której dane są przesyłane do wybranej grupy urządzeń. Multicast jest używany, gdy potrzebujemy przesłać informację tylko do wybranej grupy urządzeń. W przypadku sieci VLAN, multicast będzie dotyczył tylko urządzeń w tej samej sieci VLAN.

Unicast: to metoda transmisji, w której dane są przesyłane tylko do jednego urządzenia w sieci. Unicast jest używany, gdy potrzebujemy przesłać informację tylko do jednego urządzenia. W przypadku sieci VLAN, unicast będzie dotyczył tylko urządzeń w tej samej sieci VLAN.

### Technologia VLAN z standardem 802.1Q:

Technologia VLAN z standardem 802.1Q to standard sieciowy, który pozwala na tworzenie wirtualnych sieci lokalnych (VLAN) w sieciach Ethernet. W odróżnieniu od innych metod, które wymagają oddzielnej sieci fizycznej dla każdej VLAN, 802.1Q pozwala na segmentację sieci wirtualnych na jednym fizycznym medium.

Standard 802.1Q definiuje sposób, w jaki urządzenia sieciowe, takie jak przełączniki sieciowe, dodają tagi VLAN do ramek Ethernet. Każdy tag VLAN zawiera identyfikator VLAN, który określa, do której sieci wirtualnej ramka należy. Dzięki temu ramki z różnych VLAN mogą być przesyłane przez to samo fizyczne medium, ale są traktowane jako osobne sieci wirtualne.

Dodanie tagów VLAN do ramek Ethernet nazywa się "tagowaniem VLAN" lub "VLAN tagging". Urządzenia sieciowe, takie jak przełączniki, obsługujące standard 802.1Q, mogą również łączyć wiele sieci VLAN w jednym kablu, który nazywany jest "trunkiem VLAN". Przełączniki, które obsługują VLAN trunking, umożliwiają przesyłanie ramek z wielu sieci VLAN w jednym kablu, co pozwala na lepsze wykorzystanie przepustowości sieci fizycznej.

Broadcast, multicast i unicast to trzy podstawowe rodzaje przesyłania ramek Ethernet w sieciach komputerowych. Broadcast oznacza przesyłanie ramki do wszystkich urządzeń w sieci, multicast oznacza przesyłanie ramki do wybranej grupy urządzeń, a unicast oznacza przesyłanie ramki do jednego urządzenia. W sieci VLAN, te same zasady przesyłania ramek stosuje się do ramek z tagami VLAN. Jednakże, dzięki segmentacji sieci wirtualnych, przesyłanie ramek jest ograniczone do określonych sieci VLAN, co pomaga zwiększyć bezpieczeństwo sieci i ograniczyć rozmiar transmisji sieciowej.


## 10.3. Konfiguracja routerów i przełączników

Konfiguracja routerów i przełączników to ważna część administracji sieciowej, która pozwala na zapewnienie poprawnego działania sieci i jej optymalizację. Poniżej przedstawione są podstawowe kroki konfiguracji tych urządzeń.

+ Logowanie do urządzenia - Konfiguracja routerów i przełączników rozpoczyna się od zalogowania do urządzenia przy użyciu przeglądarki internetowej lub programu konsolowego.
+ Konfiguracja interfejsów - Następnie należy skonfigurować interfejsy urządzenia, czyli określić, jakie porty są używane do komunikacji z innymi urządzeniami w sieci.
+ Adresacja IP - Po skonfigurowaniu interfejsów należy przydzielić adresy IP, które będą wykorzystywane do komunikacji między urządzeniami. Adresy te mogą być przydzielane ręcznie lub automatycznie przez protokół DHCP.
+ Konfiguracja routingu - Router umożliwia przesyłanie pakietów między różnymi sieciami. Aby to było możliwe, należy skonfigurować protokoły routingu, takie jak RIP, OSPF czy BGP.
+ Konfiguracja usług sieciowych - Router może udostępniać różne usługi sieciowe, takie jak DNS, DHCP czy VPN. Konfiguracja tych usług jest ważnym krokiem w konfiguracji urządzenia.
+ Konfiguracja zabezpieczeń - Router musi być odpowiednio zabezpieczony przed atakami z zewnątrz. Konfiguracja zabezpieczeń obejmuje takie elementy jak filtrowanie pakietów, VPN oraz zapora ogniowa.

<p align="center">
Rys. 10.3.1. Konfiguracja routerów i przełączników
<br>
  <img src="\assets\img\Sieci\45.png" width="650" alt="Konfiguracja">
</p>

Konfiguracja przełączników wygląda podobnie, ale ma kilka specyficznych kroków. Przede wszystkim należy skonfigurować VLANy, czyli wirtualne sieci, które umożliwiają izolowanie ruchu między różnymi segmentami sieci. Następnie należy skonfigurować porty przełącznika, określając, który port jest podłączony do jakiej sieci i który port jest używany jako uplink do routera. W przypadku bardziej zaawansowanych przełączników, istnieją również dodatkowe funkcje, takie jak Quality of Service (QoS), link aggregation i protokoły STP, które można skonfigurować dla lepszej wydajności sieci.

Konfiguracja routerów i przełączników jest kluczowa dla poprawnego działania sieci i zapewnienia bezpieczeństwa jej użytkowników. Wymaga ona dobrego zrozumienia architektury sieci oraz umiejętności pracy z narzędziami i protokołami konfiguracyjnymi.

## 10.4. Sieci bezpieczne 

Sieci bezpieczne to sieci komputerowe, w których zastosowano odpowiednie środki i procedury bezpieczeństwa w celu ochrony danych, urządzeń i użytkowników przed atakami i zagrożeniami z zewnątrz i wewnątrz sieci. Sieci bezpieczne opierają się na zasadach takich jak:
+ Kontrola dostępu: sieci bezpieczne wymagają autentykacji i uwierzytelnienia użytkowników oraz zastosowania zasad kontroli dostępu do zasobów sieciowych, takich jak serwery, bazy danych i inne urządzenia.
+ Szyfrowanie: dane przesyłane przez sieć powinny być szyfrowane w celu ochrony przed przechwytywaniem i odczytywaniem przez osoby trzecie
+ Firewall: sieci bezpieczne powinny być zabezpieczone za pomocą firewalla, który kontroluje ruch sieciowy i blokuje niebezpieczne połączenia.
+ Monitorowanie i logowanie: sieci bezpieczne powinny mieć systemy monitorowania i logowania, które umożliwiają wykrywanie i reagowanie na ataki i zagrożenia.
+ Aktualizacje i łatki: systemy i oprogramowanie w sieci bezpiecznej powinny być regularnie aktualizowane i łatane w celu usuwania potencjalnych luk w zabezpieczeniach.
+ Audyt bezpieczeństwa: sieci bezpieczne powinny być regularnie audytowane w celu wykrywania i usuwania luk w zabezpieczeniach oraz w celu monitorowania poziomu bezpieczeństwa sieci.
+ Polityki bezpieczeństwa: sieci bezpieczne powinny mieć ustalone polityki bezpieczeństwa, które określają procedury i zasady bezpieczeństwa oraz wymagania dla użytkowników i administratorów sieci.

## 11. Sieci LAN, WAN, MAN

<p align="center">
Rys. 11.1. Sieci LAN, WAN, MAN
<br>
  <img src="\assets\img\Sieci\46.png" width="650" alt="Sieci">
</p>

Sieć LAN (Local Area Network) to sieć lokalna, która zwykle obejmuje niewielki obszar geograficzny, tak jak budynek, biuro lub kampus. W sieci LAN komputery i inne urządzenia są połączone ze sobą przewodowo lub bezprzewodowo, umożliwiając wymianę danych między nimi. Najczęściej wykorzystywane protokoły sieciowe w sieciach LAN to Ethernet, Wi-Fi i Bluetooth. 

<p align="center">
Rys. 11.2. LAN i WAN
<br>
  <img src="\assets\img\Sieci\47.png" width="650" alt="Sieci-1">
</p>

Sieć CAN (Controller Area Network) - Ta sieć kampusowa polega na połączeniu sieci budynkowych (LAN) w większą strukturę. Z uwagi na większe niż bezpośrednie sąsiedztwo odległości pomiędzy budynkami “spina” się je z wykorzystaniem technologii bardziej odpornej na zakłócenia, np. za pomocą kabla koncentrycznego, bądź światłowodowego z wykorzystaniem transceiverów.

To co jest istotne na tym etapie – to wiedza by nie mylić sieci komputerowej CAN, z magistralą komunikacyjną CAN (Controller Area Network) używaną w technice samochodowej i zwaną potocznie CAN BUS’em.

<p align="center">
Rys. 11.3. CAN
<br>
  <img src="\assets\img\Sieci\48.png" width="650" alt="Sieci-2">
</p>

Sieć MAN (Metropolitan Area Network) to sieć o średnim zasięgu geograficznym, obejmująca miasto lub region. Sieci MAN są zwykle tworzone przez dostawców usług telekomunikacyjnych lub samorządy, aby umożliwić komunikację między różnymi punktami w mieście lub regionie. Przykładem sieci MAN może być sieć miejska, która zapewnia dostęp do Internetu i usług telekomunikacyjnych w całym mieście.

<p align="center">
Rys. 11.4. MAN
<br>
  <img src="\assets\img\Sieci\49.png" width="650" alt="Sieci-3">
</p>

Sieć WAN (Wide Area Network) to sieć o dużym zasięgu geograficznym, obejmująca miasta, kraje lub kontynenty. W sieci WAN urządzenia są połączone ze sobą za pośrednictwem różnych środków, takich jak linie telefoniczne, przewody światłowodowe, radiowe lub satelitarne. Sieci WAN są często wykorzystywane przez duże firmy, instytucje i organizacje, aby umożliwić komunikację między oddziałami lub pracownikami w różnych lokalizacjach.

<p align="center">
Rys. 11.5. WAN
<br>
  <img src="\assets\img\Sieci\50.png" width="650" alt="Sieci-4">
</p>


# 12. Analiza ruchu sieciowego

Analiza ruchu sieciowego to proces badania i oceny ruchu przesyłanego przez sieć komputerową. W ramach analizy ruchu sieciowego, dane przesyłane przez sieć są przechwytywane i przetwarzane w celu zidentyfikowania wzorców ruchu, wykrycia anomalii oraz potencjalnych zagrożeń dla bezpieczeństwa sieci.

Istnieje wiele narzędzi do analizy ruchu sieciowego, w tym programy komercyjne i otwarte oprogramowanie. Narzędzia te umożliwiają administratorom sieci monitorowanie ruchu sieciowego w czasie rzeczywistym, analizowanie danych zapisanych w logach sieciowych, wykrywanie ataków na sieć oraz identyfikowanie problemów wydajnościowych.

Analiza ruchu sieciowego może być wykorzystana w celu zrozumienia zachowania sieci, wykrywania i rozwiązywania problemów związanych z wydajnością sieci, a także wykrywania ataków i innych zagrożeń dla bezpieczeństwa sieci. W celu skutecznej analizy ruchu sieciowego, konieczne jest posiadanie odpowiedniego narzędzia oraz wiedzy i doświadczenia w zakresie analizy ruchu sieciowego.


# 13. Sieci chmurowe

Sieci chmurowe (ang. cloud computing) to model dostarczania zasobów informatycznych, takich jak serwery, aplikacje, bazy danych, przechowywanie danych i inne usługi przez internet. W tym modelu, dostawca usług chmurowych umieszcza zasoby na serwerach zdalnych i udostępnia je klientom przez internet. Zasoby te są zwykle dostępne na żądanie i są skalowalne, co oznacza, że mogą być dostosowane do potrzeb klientów.

Istnieją trzy podstawowe modele usług chmurowych:
+ IaaS (Infrastructure as a Service) - dostarczanie infrastruktury, takiej jak serwery, wirtualne maszyny, sieci i pamięć masową.
+ PaaS (Platform as a Service) - dostarczanie platformy do tworzenia i wdrażania aplikacji.
+ SaaS (Software as a Service) - dostarczanie oprogramowania jako usługi, takie jak aplikacje biurowe, CRM, ERP itp.
Korzyści wynikające z korzystania z usług chmurowych obejmują:
+ Elastyczność i skalowalność zasobów
+ Oszczędność kosztów, ponieważ klienci mogą płacić tylko za wykorzystane zasoby
+ Łatwość wdrożenia i zarządzania, ponieważ dostawca usług chmurowych odpowiada za utrzymanie infrastruktury i zasobów
+ Dostępność z dowolnego miejsca z dostępem do internetu

Jedną z najpopularniejszych platform chmurowych jest Amazon Web Services (AWS), ale istnieją też inne, takie jak Microsoft Azure, Google Cloud Platform, IBM Cloud, Oracle Cloud i wiele innych.

# 14. Wirtualizacja sieci

Virtualizacja sieci to technologia, która pozwala na stworzenie wirtualnej infrastruktury sieciowej wewnątrz istniejącej sieci fizycznej. Pozwala to na oddzielenie fizycznej infrastruktury sieciowej od jej logicznego modelu oraz na tworzenie wirtualnych sieci wewnątrz jednej fizycznej sieci.

Wirtualizacja sieci jest szczególnie przydatna w przypadku chmury obliczeniowej, gdzie wiele wirtualnych maszyn może korzystać z jednego zestawu zasobów fizycznych. Wirtualne sieci umożliwiają izolowanie i oddzielanie ruchu sieciowego między różnymi usługami i aplikacjami, co zwiększa bezpieczeństwo sieci. Ponadto pozwala na elastyczne skalowanie zasobów sieciowych w zależności od potrzeb.

Virtualizacja sieci odbywa się za pomocą oprogramowania nazywanego hypervisorem sieciowym (także zwany przełącznikiem wirtualnym). Hypervisor sieciowy tworzy wirtualne interfejsy sieciowe i umożliwia tworzenie wirtualnych sieci, które są całkowicie oddzielone od sieci fizycznej. Wirtualne sieci mogą być konfigurowane za pomocą różnych protokołów sieciowych, takich jak VLAN, VXLAN, GRE i inne.

Virtualizacja sieci pozwala na wykorzystanie zasobów sieciowych w bardziej efektywny sposób i umożliwia łatwe zarządzanie infrastrukturą sieciową. Dzięki temu przedsiębiorstwa mogą szybciej reagować na zmieniające się wymagania biznesowe i zwiększać wydajność swojej infrastruktury sieciowej.

<p align="center">
Rys. 14.1. Wirtualizacja
<br>
  <img src="\assets\img\Sieci\51.png" width="650" alt="Wirtualizacja">
</p>


## 14.1. Virtual LAN

Virtual VLAN (VLAN wirtualne) to mechanizm segmentacji sieci, który pozwala na dzielenie jednej fizycznej sieci na wiele wirtualnych sieci VLAN, które działają jak niezależne sieci. Każda sieć VLAN ma swoją własną przestrzeń adresową i może mieć swoje własne zasady konfiguracji sieci, takie jak QoS, filtrowanie adresów MAC, kontrolę przepustowości itp.

Istnieją dwa typy VLAN wirtualnych: VLAN znacznikowane i VLAN niesznacznikowane. W przypadku VLAN znacznikowanego, każdy ruch sieciowy jest oznaczany (tagowany) przez przełącznik sieciowy z numerem VLAN, który jest przypisywany do portu, na którym ruch został odebrany. W przypadku VLAN niesznacznikowanego, ruch sieciowy jest przesyłany bez znacznika VLAN, a przełącznik sieciowy musi wiedzieć, do której sieci VLAN przypisać ruch, na podstawie portu, na którym został odebrany.

VLAN wirtualne są wykorzystywane w celu poprawy wydajności i bezpieczeństwa sieci. Dzięki ich zastosowaniu, można łatwo izolować ruch sieciowy między różnymi grupami urządzeń, takimi jak urządzenia użytkowników, serwery, urządzenia IoT itp., co pomaga w utrzymaniu bezpieczeństwa sieci. Ponadto, VLAN wirtualne pozwalają na lepszą kontrolę przepustowości, zapobiegając przeciążeniom sieci i poprawiając wydajność.

## 14.2. Virtual Router

Virtual Router (VR) to wirtualny router, który jest tworzony na urządzeniu sieciowym. VR umożliwia tworzenie odseparowanych środowisk sieciowych, w których mogą działać niezależne sieci LAN lub VLAN, a także zapewnia routing między nimi.

Wirtualny router jest tworzony za pomocą oprogramowania, które symuluje działanie tradycyjnego routera. Wirtualizacja routera pozwala na elastyczne zarządzanie siecią, łatwe tworzenie nowych sieci i zmianę konfiguracji bez potrzeby instalowania dodatkowego sprzętu.

Virtual Router może być stosowany na przykład w sieciach wirtualnych (VPN) w celu umożliwienia komunikacji między sieciami w różnych lokalizacjach lub w przypadku, gdy wymagana jest izolacja niektórych sieci od pozostałych w celu zwiększenia bezpieczeństwa.

### Jak działa Virtual Router?

Virtual Router to pojęcie odnoszące się do oprogramowania, które działa na wirtualnej maszynie i umożliwia pełnienie roli routera. Dzięki temu urządzeniu możliwe jest przesyłanie pakietów między sieciami, a także zarządzanie ruchem sieciowym.

Virtual Router działa na wirtualnym systemie operacyjnym, który działa na jednym z hostów w sieci, a jego zadaniem jest połączenie różnych sieci i kierowanie ruchem między nimi. Działanie Virtual Routera opiera się na protokołach routingu, takich jak OSPF, BGP, RIP, IS-IS czy EIGRP. Router wirtualny może mieć wiele interfejsów, co umożliwia połączenie z wieloma sieciami.

Dzięki Virtual Router możliwe jest tworzenie i zarządzanie wirtualnymi sieciami, co jest bardzo przydatne w środowiskach wirtualizacyjnych, takich jak chmury prywatne. Virtual Router pozwala na elastyczne przekierowywanie ruchu między maszynami wirtualnymi i fizycznymi, co znacznie ułatwia zarządzanie siecią.

Wirtualny Router działa w sposób podobny do fizycznego routera, ale wirtualizacja umożliwia elastyczne skalowanie zasobów i dostosowanie do wymagań konkretnego środowiska sieciowego. Virtual Router może również działać jako firewall, umożliwiając filtrowanie ruchu sieciowego i ochronę przed atakami.


## 14.3. Sieci Software-Defined Networking (SDN)

Software-Defined Networking (SDN) to koncepcja sieci, w której zarządzanie i kontrola nad przepływem danych są oddzielone od fizycznej warstwy sieci. W SDN, decyzje o przekierowaniu ruchu sieciowego podejmowane są na centralnym kontrolerze, a nie na poszczególnych urządzeniach sieciowych.

W praktyce, SDN składa się z trzech głównych elementów:
+ Aplikacji sieciowych: służą do zarządzania i monitorowania ruchu sieciowego w czasie rzeczywistym, takich jak aplikacje do optymalizacji ruchu, firewall'e i balansery obciążenia.
+ Kontrolera: to centralny punkt zarządzania, który zarządza przepływem ruchu sieciowego i podejmuje decyzje o przekierowaniu ruchu sieciowego na podstawie polityk sieciowych.
+ Przełączniki: to fizyczne urządzenia sieciowe, które przekazują ruch sieciowy na podstawie decyzji podejmowanych przez kontroler. Przełączniki muszą obsługiwać protokoły SDN, takie jak OpenFlow, aby umożliwić komunikację z kontrolerem.


<p align="center">
Rys. 14.3.1. Architektura SDN
<br>
  <img src="\assets\img\Sieci\52.png" width="650" alt="SDN">
</p>

Sieć overlay (nakładowa), to właśnie tutaj realizowane są wszystkie “inteligentne” funkcje takie jak różnego rodzaju polityki czy segmentacja. Mimo że protokoły komunikacyjne w tej warstwie mogą być różne w zależności od producenta danego rozwiązania, to do enkapsulacji wykorzystywany jest zazwyczaj protokół VXLAN.

Jeśli chodzi o sieć underlay (podkładowa), tutaj sprawa jest dużo prostsza. W zakresie komunikacji ma to być po prostu routowalna sieć IP zapewniająca maksymalną prostotę, wydajność i niezawodność.

To właśnie dla tego, w niektórych rozwiązaniach na ścieżce sieci SDN mogą występować urządzenia starszych generacji, w przeciwieństwie do urządzeń, na których realizowane najważniejsze funkcje sieci nakładkowej i komunikacja z kontrolerami. W zależności od rozwiązania stopień przeniesienia logiki do centralnego kontrolera jest różny. Czasem jest to zdecydowana większość a czasem, część z niej zostawiona jest urządzeniom, którymi kontroler steruje.

Bez względu na to, w przypadku sieci definiowanych programowo śmiało możemy mówić o rozdziale między część Control Plane, która przeniesiona jest na kontroler, i część Data Plane, a więc prostego przesyłu pakietów, który niejako pozostał urządzeniom sieciowym. Kwestia proporcji w jakich część Control Plane została wyniesiona poza urządzenia końcowe, zależy już od konkretnego rozwiązania.

# 15. NGFW - Security Functions

NGFW (Next-Generation Firewall) to rodzaj zapory sieciowej, która umożliwia bardziej zaawansowaną kontrolę i zabezpieczenie ruchu sieciowego niż tradycyjne zapory. NGFW łączy w sobie funkcje tradycyjnych zapór sieciowych z dodatkowymi funkcjami, takimi jak IPS (Intrusion Prevention System), VPN (Virtual Private Network), filtracja treści, wykrywanie anomalii i zagrożeń, a także integrację z systemami SIEM (Security Information and Event Management).

NGFW oferuje wiele funkcji związanych z bezpieczeństwem sieciowym, w tym:
+ Blokowanie niepożądanych aplikacji - NGFW może blokować dostęp do aplikacji, które nie są zgodne z polityką bezpieczeństwa organizacji, takich jak media społecznościowe, gry, poczta elektroniczna itp.
+ Kontrola dostępu - NGFW może umożliwiać lub blokować dostęp do zasobów sieciowych, w zależności od poziomu uprawnień użytkownika i rodzaju urządzenia.
+ Wykrywanie i blokowanie zagrożeń - NGFW może wykrywać i blokować niebezpieczne zachowania, takie jak ataki malware, phishing, ransomware itp.
+ Filtrowanie treści - NGFW może umożliwiać blokowanie dostępu do nieodpowiednich treści, takich jak pornografia, wulgaryzmy itp.
+ Ochrona przed atakami DDoS - NGFW może chronić sieć przed atakami DDoS, wykrywając i blokując nadmierne ruchy sieciowe, które mogą prowadzić do przeciążenia serwerów.
+ Kontrola danych - NGFW może umożliwiać filtrowanie i kontrolę przesyłanych danych, takich jak numer karty kredytowej, dane personalne itp.

NGFW oferuje także wiele innych funkcji związanych z bezpieczeństwem sieciowym, takich jak monitorowanie i analiza ruchu sieciowego, raportowanie zdarzeń związanych z bezpieczeństwem, integracja z systemami SIEM, a także automatyczne aktualizacje oprogramowania w celu zapewnienia najnowszych funkcji zabezpieczeń.

NGFW może obsługiwać różne protokoły i usługi, takie jak protokoły sieciowe (np. TCP/IP, UDP), protokoły tunelujące (np. IPSec, GRE), protokoły routingu (np. OSPF, BGP), protokoły aplikacyjne (np. HTTP, FTP), a także usługi bezpieczeństwa (np. VPN, filtracja URL).

W celu monitorowania i zarządzania NGFW można stosować różne narzędzia i technologie, takie jak systemy monitorowania zdarzeń (SIEM), systemy zarządzania politykami bezpieczeństwa (NAC), narzędzia do audytowania i raportowania (np. NetFlow Analyzer), a także oprogramowanie do wirtualizacji sieci (np. VMware NSX). Dodatkowo, w niektórych przypadkach producenci NGFW oferują własne narzędzia zarządzania i monitorowania.

### Na jakiej podstawie blokowane są ruchy w funkcji "blokowanie aplikacji" w NGFW?

W funkcji blokowania aplikacji w NGFW blokowanie niedozwolonych aplikacji odbywa się na podstawie zdefiniowanych zasad polityki bezpieczeństwa. Polityka bezpieczeństwa określa, jakie aplikacje są dozwolone i niedozwolone, a także jakie reguły i filtry mają być stosowane do każdej aplikacji. Blokowanie aplikacji może odbywać się na podstawie różnych parametrów, takich jak porty, protokoły, adresy IP, sygnatury aplikacji i wiele innych. NGFW może wykorzystywać różne techniki, takie jak inspekcja pakietów i analiza zachowań, aby wykryć i zablokować niedozwolone aplikacje.


# 16. Spanning Tree

Spanning Tree Protocol (STP) to protokół sieciowy, który umożliwia uniknięcie pętli w topologiach sieciowych z topologią drzewa (np. w sieciach LAN). Pętle w sieci mogą prowadzić do poważnych problemów, takich jak nadmierny ruch sieciowy i utrata wydajności sieci. STP rozwiązuje ten problem, wybierając jedną drogę do przesyłania ruchu w drzewie topologii sieciowej, co zapobiega tworzeniu pętli.

STP działa poprzez wybieranie korzenia drzewa sieciowego, który służy jako punkt centralny dla całej sieci. Wszystkie pozostałe urządzenia sieciowe wybierają najkrótszą ścieżkę do korzenia, co tworzy drzewo topologii sieciowej. STP regularnie monitoruje ruch w sieci i automatycznie wybiera nową najkrótszą ścieżkę, jeśli oryginalna ścieżka zostanie przerwana.

STP ma kilka zalet:
+ Zapobiega pętlom - STP wybiera jedną ścieżkę do przesyłania ruchu w topologii drzewa, co zapobiega tworzeniu pętli.
+ Zwiększa niezawodność sieci - STP automatycznie wybiera nową najkrótszą ścieżkę, jeśli oryginalna ścieżka zostanie przerwana, co zapewnia niezawodność sieci.
+ Poprawia wydajność sieci - STP wybiera najlepszą ścieżkę do przesyłania ruchu, co zwiększa wydajność sieci i zmniejsza opóźnienia.
+ Łatwość konfiguracji - STP jest łatwy do skonfigurowania i działa automatycznie, co zmniejsza potrzebę ręcznej konfiguracji urządzeń sieciowych.

Wady STP to:
+ Wolna konwergencja - STP może prowadzić do wolnej konwergencji sieci, co może prowadzić do opóźnień w przesyłaniu ruchu.
+ Złożoność sieci - STP może prowadzić do złożonej topologii sieciowej, co może utrudniać zarządzanie siecią.
+ Brak wykorzystania pełnego potencjału sieci - STP wybiera jedną drogę do przesyłania ruchu, co oznacza, że inne ścieżki są nieużywane i nie wykorzystują pełnego potencjału sieci.

Pętla w topologii sieciowej to sytuacja, w której ruch sieciowy krąży w kółko między urządzeniami sieciowymi, zamiast dotrzeć do swojego celu. Pętle mogą powstać w sieciach, które mają więcej niż jedną ścieżkę między dwoma punktami w sieci. Może to wystąpić, gdy na przykład w sieciach LAN mamy połączenie z punktu A do punktu B, a także z punktu A do punktu C, a z punktu C do punktu B. W takim przypadku, jeśli ruch sieciowy zostanie przesłany z punktu A do punktu B przez połączenie A-C-B, a jednocześnie zostanie przesłany z punktu A do punktu B przez połączenie A-B, to ruch sieciowy będzie krążył między punktami A, B i C, tworząc pętlę.

Pętle mogą prowadzić do poważnych problemów, takich jak zwiększenie ruchu sieciowego, utrata wydajności sieci, a nawet awarie sieci. Wiele urządzeń sieciowych, takich jak switche, posiada funkcje bezpieczeństwa, które pomagają zapobiegać pętlom, na przykład protokół STP, o którym pisałem wcześniej.

### Jakie są typowe problemy związane z działaniem Spanning Tree?

Odpowiedź: Typowymi problemami związanymi z działaniem Spanning Tree są: spowolnienie sieci, utrata pakietów, problemy z konfiguracją i utrzymaniem. Nieprawidłowa konfiguracja algorytmu Spanning Tree może prowadzić do nieoptymalnej ścieżki między urządzeniami w sieci.

### Jakie narzędzia i technologie są stosowane w celu monitorowania i zarządzania Spanning Tree?

Odpowiedź: Narzędzia i technologie stosowane w celu monitorowania i zarządzania Spanning Tree to między innymi: narzędzia do analizy pakietów, SNMP (Simple Network Management Protocol), CLI (Command Line Interface), GUI (Graphical User Interface), syslog, alerty i raporty.

### Według jakiej zasady wybiera się drogą w Spanning Tree (tzn. jak jest kilka ruchów w VLAN to na jakiej zasadzie odrzucane są inne ruchy, oprócz najlepszego)?

W protokole Spanning Tree (STP) wybieranie drogi odbywa się na podstawie priorytetów mostów i ich adresów MAC. Każdy most STP posiada swój priorytet, który jest domyślnie ustawiony na 32 768. Most o niższym priorytecie jest uważany za lepszego i jest używany jako most korzeniowy, czyli główny most w sieci. Każdy port mostu posiada swój własny priorytet, który jest wyliczany na podstawie priorytetu mostu i adresu MAC podłączonego urządzenia. Porty z niższym priorytetem są uważane za lepsze i są wybierane jako główna ścieżka do przesyłania ruchu. Gdy STP wykryje pętlę w sieci, blokuje jeden z portów na mostach, aby zapobiec przepływowi ruchu i zapobiec pętli.

# 17. Network Security

Bezpieczeństwo sieci (Network Security) to proces zapewnienia ochrony sieci przed różnymi zagrożeniami, takimi jak ataki z zewnątrz lub wewnętrzne incydenty bezpieczeństwa. Bezpieczeństwo sieci jest kluczowe dla zapewnienia poufności, integralności i dostępności informacji przechowywanych w sieciach.

Podstawowymi zagrożeniami dla sieci są ataki z zewnątrz, takie jak ataki DDoS, phishing czy ransomware. Wewnętrzne zagrożenia obejmują takie kwestie jak nieuprawniony dostęp do sieci lub danych, błędy ludzkie czy zagrożenia wynikające z nieaktualnych lub niewystarczających zabezpieczeń.

## 17.1. Wireless Security (802.11i)

Wireless Security (802.11i) to standard bezpieczeństwa sieci bezprzewodowych, który określa protokoły i metody zabezpieczania transmisji danych w sieciach WLAN. 802.11i został wprowadzony w celu zastąpienia niezbyt skutecznych mechanizmów zabezpieczeń w starszych standardach bezprzewodowych.

W 802.11i zastosowano protokół bezpieczeństwa WPA2 (Wi-Fi Protected Access II), który zapewnia silne szyfrowanie i uwierzytelnianie użytkowników. WPA2 wykorzystuje zaawansowany algorytm szyfrowania AES (Advanced Encryption Standard), który zapewnia bezpieczną komunikację między punktem dostępu a urządzeniami końcowymi.

WPA2 zapewnia dwa tryby uwierzytelniania: PSK (Pre-Shared Key) i EAP (Extensible Authentication Protocol). PSK to tryb, w którym używany jest wspólny klucz uwierzytelniający (hasło) między punktem dostępu a urządzeniami końcowymi. W trybie EAP używany jest serwer uwierzytelniania, który weryfikuje tożsamość użytkownika, przed udzieleniem dostępu do sieci.

W 802.11i wprowadzono również mechanizm szyfrowania danych zwany Temporal Key Integrity Protocol (TKIP), który generuje unikalne klucze szyfrujące dla każdej transmisji danych. Dzięki temu, nawet jeśli ktoś przechwyciłby klucz szyfrujący, nie mógłby go wykorzystać do deszyfrowania innych transmisji.

W 802.11i zaimplementowano także mechanizm autoryzacji dostępu, zwany RADIUS (Remote Authentication Dial-In User Service), który umożliwia uwierzytelnianie użytkowników przy użyciu serwera autoryzacji. Serwer RADIUS może kontrolować dostęp użytkowników do różnych części sieci oraz nakładać ograniczenia dotyczące przepustowości i innych parametrów połączenia.


## 17.2. Malware

Malware to skrót, który pochodzi od słowa malicious software. Oznacza złośliwe oprogramowanie, które zostało stworzone z myślą o uszkodzeniu sprzętu lub kradzieży danych. Ten termin jest jednak bardzo szeroki i obejmuje zarówno fragmenty kodu, jak i programy szkodzące systemowi. W zależności od typu złośliwe oprogramowanie może dążyć do uszkodzenia podstawowych funkcjonalności systemu, skasowania danych, otworzeniu, tzw. tylnych drzwi do kolejnych ataków, blokady komputera lub atakowania reklamami. Złośliwe oprogramowanie może pojawić się na różnego typu sprzęcie, tj. komputerze stacjonarnym, laptopie, tablecie, telefonie czy każdym innym urządzeniu, które posiada dostęp do internetu. 

Aby chronić system przed złośliwym oprogramowaniem, ważne jest stosowanie odpowiedniego oprogramowania antywirusowego i zapory sieciowej, a także regularne aktualizacje systemu i oprogramowania. W przypadku infekcji malware, należy jak najszybciej podjąć kroki do usunięcia złośliwego oprogramowania i przywrócenia bezpieczeństwa systemu.

<p align="center">
Rys. 17.2.1. Typy Malware
<br>
  <img src="\assets\img\Sieci\53.png" width="650" alt="Malware ">
</p>

Najważniejsze rodzaje malware to:
+ wirusy, robaki, konie trojańskie – programy albo fragmenty kodu, które pasożytują na programach wykorzystywanych przez sprzęt i zajmują jego zasoby; wirusy dołączają się do innych programów i modyfikują je tak, żeby się powielać;
+ ransomware – oprogramowanie szantażujące; umożliwia dostęp do prywatnych dokumentów poprzez szyfrowanie plików lub blokuje ekran albo start systemu operacyjnego; aby odblokować te funkcjonalności, należy zapłacić okup – jego żądanie wyświetla się na komputerze;  
+ spyware – to kolejne oprogramowanie szpiegujące; jego działanie opiera się na zbieraniu informacji o aktywności użytkownika, np. odwiedzanych w Internecie stronach; 
+ adware – odpowiada za natrętnie wyświetlane reklamy, których użytkownik sobie nie życzy;
+ browser hijackers – wprowadzają zmiany w konfiguracji przeglądarek (np. dodają paski narzędzi czy zmieniają stronę startową);
+ keyloggery – działanie tego oprogramowania polega na odczytywaniu, następnie zapisywaniu naciskanych przez użytkownika klawiszy; dzięki temu cyberprzestępcy mogą wykradać hasła, np. do bankowości internetowej, kont na mediach społecznościowych itp.;
+ rootkit – ukryta aplikacja, która pozwala administrować całym systemem, np. w celu kradzieży danych; uznaje się, że rootkit jest jedną z najgroźniejszych form szkodliwego oprogramowania, trudna do wykrycia;
+ rogue anti-spyware – to malware, które udają programy chroniące przed oprogramowaniem szpiegującym; podaje informacje mające przestraszyć użytkownika i skłonić go do zakupu drogiego programu, który rzekomo chroni przed zagrożeniami; 
+ cryptojacking – jest to nazwa dla nieautoryzowanego dostępu do komputera, które ma na celu wykorzystanie potencjału sprzętu do kopania kryptowaluty.


## 17.3. Password Attack

Password Attack to atak polegający na próbie złamania hasła do systemu lub konta użytkownika. Atak ten może zostać przeprowadzony w różny sposób, w zależności od celu i dostępnych narzędzi.

Jednym z najpopularniejszych rodzajów ataków na hasła jest atak siłowy (brute-force attack). Polega on na przetestowaniu wszystkich możliwych kombinacji znaków, aż zostanie znalezione poprawne hasło. Innym rodzajem ataku jest atak słownikowy (dictionary attack), w którym atakujący korzysta z listy popularnych haseł lub wykorzystuje informacje z wcześniejszych wycieków haseł, aby znaleźć odpowiednie hasło.

Innym sposobem ataku na hasła może być wykorzystanie tzw. social engineeringu. Polega to na wykorzystaniu informacji o użytkowniku (np. z mediów społecznościowych) lub jego bliskich, aby uzyskać dostęp do informacji potrzebnych do złamania hasła.

Istnieją również bardziej zaawansowane techniki ataków na hasła, takie jak ataki z wykorzystaniem tzw. botnetów lub wykorzystanie luki w systemie, która pozwala na łatwiejsze zdobycie hasła.

Aby chronić swoje hasła przed atakami, ważne jest stosowanie silnych i unikalnych haseł, regularna zmiana haseł oraz wykorzystanie technologii takich jak dwuskładnikowe uwierzytelnianie czy hasła jednorazowe (OTP). W przypadku organizacji ważne jest również stosowanie polityk bezpieczeństwa haseł oraz szkolenie pracowników w zakresie bezpiecznego przechowywania i korzystania z haseł.

<p align="center">
Rys. 17.3.1. Password Attack
<br>
  <img src="\assets\img\Sieci\54.png" width="650" alt="Ransomware">
</p>


## 17.3.1. Brute-Force ataki na hasła

Ten typ ataku na hasło wykorzystuje metody prób i błędów w celu odgadnięcia informacji uwierzytelniających użytkownika. Zły aktor używa zautomatyzowanych skryptów, aby przejść przez jak najwięcej permutacji, aby poprawnie odgadnąć hasło użytkownika. Chociaż jest to stosunkowo stara metoda, która wymaga dużo cierpliwości i czasu, atak brutalnej siły jest nadal standardem w przypadku prób włamania na konto, ponieważ są one zautomatyzowane i proste. Istnieje kilka rodzajów ataków siłowych:
+ Proste ataki siłowe —  haker wykorzystuje logikę i dane o użytkowniku, aby odgadnąć najbardziej prawdopodobne hasło. Ta technika jest używana w przypadku prostych haseł, takich jak te zawierające kombinację imienia i nazwiska zwierzaka, roku i urodzenia.
+ Upychanie poświadczeń —  obejmuje to użycie wcześniej ujawnionych kombinacji logowania, które zostały złośliwie uzyskane na podatnych stronach internetowych. W takich atakach hakerzy zazwyczaj wykorzystują fakt, że podmioty mają tendencję do ponownego wykorzystywania kombinacji nazwy użytkownika i hasła w wielu usługach.
+ Hybrydowe ataki typu brute force —  osoba atakująca łączy proste odgadywanie słabych haseł ze zautomatyzowanym oprogramowaniem, które wypełnia dane uwierzytelniające w celu wykrycia złożonych haseł. W większości systemów produkcyjnych podmioty używają niewielkich odmian haseł w różnych witrynach internetowych. Atakujący polegają również na wzorcach danych użytkowników w różnych usługach, aby poprawić dokładność narzędzi do upychania danych uwierzytelniających.
+ Odwrotne ataki brute force –  w tym ataku haker zaczyna od znanego hasła, a następnie szuka pasujących do niego nazw użytkowników. Ponieważ cyberprzestępcy często mają dostęp do wielu baz danych uwierzytelniających, które wyciekły, łatwo jest zidentyfikować wspólne hasła w obrębie określonej grupy użytkowników.


## 17.4. Ransomware

Ransomware to złośliwe oprogramowanie, które szyfruje pliki na komputerze ofiary i żąda od niej okupu w zamian za odszyfrowanie danych. W większości przypadków, gdy ransomware zainfekuje komputer, szyfruje on pliki na dysku twardym, a następnie wyświetla monit, w którym żąda okupu w zamian za odszyfrowanie plików.

Ransomware może dostać się na komputer za pomocą złośliwych załączników e-mail, niezaufanych witryn internetowych, exploitów wykorzystujących luki w oprogramowaniu lub poprzez wykorzystanie luk w zabezpieczeniach sieci.

Po zainfekowaniu komputera ransomware zaczyna działać i szyfruje pliki, takie jak dokumenty, filmy, zdjęcia itp. Następnie wyświetla monit, w którym żąda okupu, zwykle w postaci kryptowaluty, takiej jak Bitcoin, w zamian za odszyfrowanie plików. Często monit zawiera także ostrzeżenie, że w przypadku braku zapłaty klucz do odszyfrowania plików zostanie trwale usunięty.

W przypadku ataku ransomware ważne jest, aby nie płacić okupu, ponieważ nie ma to gwarancji, że pliki zostaną odszyfrowane. Zamiast tego należy wykonać kopię zapasową plików i oczyścić komputer z złośliwego oprogramowania. W celu zminimalizowania ryzyka ataku ransomware, zaleca się również stosowanie oprogramowania antywirusowego i regularne aktualizowanie systemu oraz oprogramowania.


<p align="center">
Rys. 17.4.1. Password Attack
<br>
  <img src="\assets\img\Sieci\55.png" width="650" alt="Password">
</p>


## 17.5. Firewall 

Firewall, czyli zapora sieciowa, to rodzaj programu lub urządzenia, które ma za zadanie chronić sieć komputerową przed nieautoryzowanym dostępem oraz atakami z sieci. Firewall może blokować niepożądany ruch sieciowy, pozwalać na dostęp jedynie do określonych portów oraz ograniczać dostęp do sieci wewnętrznej z zewnątrz.

Istnieją dwa główne typy firewalli:
+ Firewall programowy - działa jako program na komputerze lub urządzeniu sieciowym. Oprogramowanie firewalla analizuje każdy pakiet przesyłany przez sieć, decydując, czy należy go zablokować czy przekierować. W firewallach programowych można ustawić różne reguły blokowania lub umożliwienia dostępu, a także konfigurować szczegółowe ustawienia.
+ Firewall sprzętowy - jest to fizyczne urządzenie, które działa jako brama między siecią wewnętrzną a zewnętrzną. Firewall sprzętowy może działać jako osobne urządzenie lub być zintegrowany z routerem lub innym urządzeniem sieciowym. Firewalle sprzętowe są zazwyczaj wyposażone w zaawansowane funkcje, takie jak ochrona przed atakami DDoS, filtracja adresów URL i wykrywanie intruzów.

*Stanowy firewall* to rodzaj zapory sieciowej, który analizuje połączenia sieciowe w kontekście stanu połączenia. Oznacza to, że firewall śledzi stan każdego połączenia sieciowego i decyduje, czy dane połączenie powinno być zezwolone, zablokowane lub przekierowane na podstawie informacji o stanie połączenia.

Przykładowo, gdy klient wysyła żądanie połączenia z serwerem, firewall tworzy wpis w tabeli stanu połączenia, który zawiera informacje o adresach źródłowych i docelowych, numerach portów, stanie połączenia i innych parametrach. Wtedy, kiedy odpowiedź na żądanie połączenia zostanie odebrana, firewall porównuje parametry połączenia w odpowiedzi z informacjami o stanie połączenia w tabeli. Jeśli informacje są zgodne, firewall przepuszcza ruch sieciowy zgodnie z regułami ustawionymi przez administratora.

*Firewall proxy* służy jako brama z jednej sieci do drugiej dla konkretnej aplikacji. Serwery proxy mogą zapewnić dodatkową funkcjonalność, jak na przykład buforowanie treści i zabezpieczanie poprzez uniemożliwianie nawiązywania bezpośrednich połączeń z siecią zewnętrzną.

Zapory sieciowe (firewalle) na różnych warstwach modelu ISO/OSI:
+ Warstwa 2 - firewall na warstwie 2 to tzw. firewall typu filtr MAC. Działa on na poziomie adresów MAC, blokując lub przepuszczając pakiety na podstawie ich adresów źródłowych i docelowych. Takie firewalle są stosowane przede wszystkim do zabezpieczania sieci bezprzewodowych.
+ Warstwa 3 - firewall na warstwie 3 to zapora typu filtr IP. Działa ona na poziomie adresów IP, decydując o przepuszczeniu lub zablokowaniu pakietów na podstawie adresu źródłowego i docelowego oraz numerów portów. Firewalle warstwy 3 mogą działać w trybie routera, gdzie blokują niepożądany ruch między różnymi sieciami.
+ Warstwa 4 - firewall na warstwie 4 to firewall typu filtr pakietów. Działa na poziomie numerów portów, decydując o przepuszczeniu lub zablokowaniu ruchu na podstawie portów źródłowych i docelowych. Ten typ firewalla jest najczęściej stosowany do zabezpieczenia serwerów, aplikacji oraz usług sieciowych.
+ Warstwa 5, 6 i 7 - na tych warstwach mogą działać firewalle typu proxy, które pełnią rolę pośrednika w połączeniach między aplikacjami. Działają one na poziomie protokołów wyższych warstw ISO/OSI, analizując zawartość ruchu sieciowego. Zapory tego typu pozwalają na bardziej szczegółowe kontrolowanie ruchu sieciowego i filtrowanie treści, co zapewnia większe bezpieczeństwo.


## 17.6. Ataki DoS

Ataki DoS (Denial of Service) polegają na przepełnieniu łącza sieciowego lub zasobów systemowych serwera przez atakującego, co skutkuje tymczasowym lub trwałym wyłączeniem usługi dla użytkowników.

Atak DoS może być przeprowadzany na różne sposoby, na przykład poprzez generowanie dużych ilości zapytań do serwera, a także poprzez infekowanie komputerów i urządzeń sieciowych botami, które wysyłają zapytania do serwera w celu zwiększenia obciążenia.

Ataki DoS mogą skutkować znacznymi stratami finansowymi dla firm i organizacji, które są atakowane, ze względu na czasowe wyłączenie usługi i koszty związane z odtwarzaniem uszkodzonych zasobów.

Aby chronić się przed atakami DoS, firmy i organizacje mogą stosować różne rozwiązania, takie jak firewalle, filtry pakietów, rozwiązania antyspamowe oraz technologie load balancingu, które pozwalają na równomierne rozłożenie obciążenia pomiędzy kilka serwerów.


## 17.7. DDoS

DDoS (Distributed Denial of Service) to rodzaj ataku, w którym sieć komputerowa jest zalewana ogromną ilością żądań, zwykle pochodzących z wielu różnych źródeł, w celu spowolnienia lub całkowitego wyłączenia usługi dla prawidłowych użytkowników.

Ataki DDoS są zwykle przeprowadzane za pomocą botnetów, które składają się z wielu zainfekowanych komputerów połączonych w jedną sieć. Atakujący mogą kontrolować te komputery zdalnie i używać ich do wysyłania nieustannych strumieni żądań do celu ataku.

Cele ataków DDoS mogą obejmować serwery internetowe, strony internetowe, aplikacje internetowe, a nawet całe sieci komputerowe. Ataki DDoS mogą powodować znaczne straty finansowe i reputacyjne, ponieważ spowalniają lub uniemożliwiają normalne funkcjonowanie usług online.
Obrona przed atakami DDoS może obejmować wykorzystanie specjalistycznych narzędzi i usług do wykrywania i blokowania ruchu złośliwego, a także projektowanie infrastruktury sieciowej z myślą o minimalizacji skutków ataku.

*Różnica między DoS a DDoS:*

Atak DoS (Denial of Service) to atak, w którym atakujący próbuje sparaliżować dostępność systemu lub usługi, przeciążając je ruchem sieciowym lub wykorzystując inne sposoby, takie jak ataki z użyciem złośliwego oprogramowania. Atak DoS może być przeprowadzony przez jednego atakującego i jest zazwyczaj ograniczony do jednego źródła.

Z drugiej strony, atak DDoS (Distributed Denial of Service) wykorzystuje wiele źródeł, często rozproszonych po całym świecie, aby przeciążyć cel ataku ruchem sieciowym. Atakujący wykorzystuje botnety lub komputery zombie do przeprowadzenia ataku, co utrudnia zlokalizowanie źródła ataku. Atak DDoS jest zazwyczaj bardziej skuteczny niż atak DoS i może być trudniejszy do powstrzymania.


## 17.8. Phishing

Phishing to atak polegający na wyłudzeniu poufnych informacji, takich jak hasła, numery kart kredytowych czy inne dane osobowe, poprzez podszywanie się pod zaufane źródło, np. bank, sklep internetowy czy serwis społecznościowy.

Typowo, atak phishingowy wykorzystuje fałszywe e-maile, SMS-y lub wiadomości na platformach społecznościowych, które wyglądają jak autentyczne, ale w rzeczywistości są prowadzone przez oszustów, którzy próbują przekonać odbiorcę do udostępnienia swoich poufnych danych lub kliknięcia w linki prowadzące do złośliwych stron internetowych.

Ataki phishingowe zwykle są stosowane w celu kradzieży tożsamości lub innych danych, które można wykorzystać do celów finansowych lub przestępczych. Można je zminimalizować, stosując ostrożność podczas przeglądania internetu, nieudostępnianie poufnych danych w odpowiedzi na nieznane lub podejrzane wiadomości e-mail, oraz korzystanie z narzędzi do blokowania i filtrowania wiadomości phishingowych.

W atakach typu phishing hakerzy często wykorzystują wiele metod, aby nakłonić użytkownika do kliknięcia złośliwego łącza, w tym:
+ Zatruwanie pamięci podręcznej DNS —  atakujący wykorzystują luki w serwerze DNS aplikacji, aby przekierować żądania użytkowników do złośliwej witryny o podobnie wyglądającej nazwie domeny.
+ Przechwytywanie adresów URL/typosquatting —  osoba atakująca tworzy autentycznie wyglądający adres URL z subtelnymi różnicami w stosunku do witryny, pod którą chce się podszyć. Następnie atak polega na tym, że użytkownicy popełniają błędy w pisaniu, więc lądują na złośliwej stronie. 
+ Tabnabbing –  osoba atakująca przepisuje nienadzorowane karty przeglądarki złośliwymi witrynami, które wyglądają jak legalne strony internetowe.
+ Przekierowywanie interfejsu użytkownika/nakładka iFrame —  za pomocą przezroczystych warstw atakujący umieszcza łącze do złośliwej strony nad legalnym, klikalnym przyciskiem. 
+ Clone phishing –  w tym ataku atakujący wysyła kopię legalnej wiadomości e-mail, w której łącza w oryginalnej wiadomości e-mail są zastępowane adresami URL prowadzącymi do złośliwych witryn.


## 17.9. Bezpieczeństwo w sieciach IoT

Bezpieczeństwo w sieciach IoT (Internet of Things) to kwestia kluczowa, ponieważ coraz więcej urządzeń jest połączonych z internetem i sieciami. Sieci IoT składają się z urządzeń takich jak inteligentne telewizory, smartfony, samochody, systemy alarmowe, kamery itp., które zbierają, przetwarzają i wysyłają dane do sieci. Jednakże wiele z tych urządzeń nie ma wbudowanych mechanizmów bezpieczeństwa, co czyni je podatnymi na ataki i naruszenia prywatności.

<p align="center">
Rys. 17.9.1. Bezpieczeństwo w sieciach IoT
<br>
  <img src="\assets\img\Sieci\56.png" width="650" alt="IoT">
</p>

Poniżej przedstawiono kilka kluczowych aspektów bezpieczeństwa w sieciach IoT:
+ Aktualizacje oprogramowania: ważne jest, aby urządzenia w sieci IoT były zawsze zaktualizowane do najnowszej wersji oprogramowania. Aktualizacje zawierają łatki bezpieczeństwa, które poprawiają lukę w zabezpieczeniach i chronią przed atakami.
+ Wprowadzenie certyfikatów SSL/TLS: to standardowe narzędzie zabezpieczające dane przesyłane między urządzeniami IoT i serwerami. Certyfikaty SSL/TLS zapewniają szyfrowanie danych, dzięki czemu trudniej jest uzyskać nieautoryzowany dostęp do sieci.
+ Ochrona przed atakami DDoS: ataki DDoS (Distributed Denial of Service) to próba przeciążenia sieci IoT poprzez atakowanie wielu urządzeń jednocześnie. Aby zabezpieczyć sieć przed tym rodzajem ataku, można zastosować rozwiązania takie jak filtrowanie adresów IP i wdrożenie rozwiązania zapobiegającego atakom.
+ Uwierzytelnianie i autoryzacja użytkowników: w sieciach IoT ważne jest, aby każdy użytkownik miał unikalne dane uwierzytelniające i uprawnienia dostępu do danych i urządzeń. W przypadku nieautoryzowanego dostępu do urządzeń lub danych, możliwe jest naruszenie prywatności i bezpieczeństwa użytkowników.
+ Monitorowanie i analiza ruchu sieciowego: istotne jest, aby sieć IoT była monitorowana w celu wykrycia nieprawidłowości i ataków. Dzięki analizie ruchu sieciowego można zidentyfikować podejrzane aktywności i podjąć odpowiednie kroki w celu ochrony sieci.


# 18. Standardy bezpieczeństwa

Istnieje wiele standardów i ram bezpieczeństwa, które zostały opracowane, aby pomóc w ochronie systemów i sieci przed różnymi zagrożeniami i atakami.

## 18.1. ISO 27001

ISO 27001 to międzynarodowy standard dla systemów zarządzania bezpieczeństwem informacji (Information Security Management Systems, ISMS). Jest to kompleksowy framework zawierający wymagania dotyczące procesu zarządzania bezpieczeństwem informacji w organizacji.

Standard ISO 27001 składa się z czterech głównych sekcji: wprowadzenie i obszar zastosowania, normatywne odwołania, terminy i definicje oraz wymagania dla systemów zarządzania bezpieczeństwem informacji.

Wymagania te obejmują:
+ Określenie zakresu i celów systemu zarządzania bezpieczeństwem informacji.
+ Ustalenie polityki bezpieczeństwa informacji i kierunków działań w tym zakresie.
+ Wykonywanie oceny ryzyka i ustalanie odpowiednich środków zapobiegawczych.
+ Zapewnienie stałej poprawy systemu zarządzania bezpieczeństwem informacji.
+ Wdrażanie i utrzymywanie odpowiednich środków technicznych i organizacyjnych w celu ochrony informacji.
+ Wykonywanie audytów wewnętrznych i zapewnienie, że system zarządzania bezpieczeństwem informacji jest skuteczny.

ISO 27001 jest jednym z najczęściej stosowanych standardów w dziedzinie bezpieczeństwa informacji. Wdrażając go, organizacje mogą skutecznie chronić swoje informacje, minimalizując ryzyko związane z cyberatakiem lub wyciekiem poufnych danych.

<p align="center">
Rys. 18.1.1. ISO 27001 
<br>
  <img src="\assets\img\Sieci\57.png" width="650" alt="ISO">
</p>

Zasady działania ISO 27001 opierają się na Plan, Do, Check, Act (PDCA) - Planuj, Wykonuj, Sprawdzaj, Działaj. W ramach tej metodologii, organizacja działa w następujący sposób:
+ Planowanie: Organizacja musi opracować i wdrożyć politykę bezpieczeństwa informacji, która określa cele i cele bezpieczeństwa informacji, a także identyfikuje ryzyka i planuje działania zapobiegające.
+ Wykonanie: Organizacja musi wdrożyć planowane działania zapobiegające, w tym technologie i procedury, które zapewnią bezpieczeństwo jej zasobów informacyjnych. W ramach tego procesu organizacja powinna też wyznaczyć role i odpowiedzialności w zakresie bezpieczeństwa informacji.
+ Sprawdzanie: Organizacja musi regularnie monitorować swoje środowisko informacyjne w celu identyfikacji ryzyka i zagrożeń. W przypadku wykrycia zagrożeń, organizacja powinna podjąć odpowiednie kroki w celu ich wyeliminowania.
+ Działanie: Organizacja musi stale doskonalić swoje systemy bezpieczeństwa informacji, biorąc pod uwagę wyniki monitoringu i przeglądu. W tym celu organizacja powinna regularnie przeprowadzać przeglądy swoich systemów i wprowadzać ulepszenia w celu zwiększenia bezpieczeństwa swoich zasobów informacyjnych.


## 18.2. PCI DSS

Standard PCI DSS(Payment Card Industry Data Security Standard) to zestaw wymagań bezpieczeństwa informacji, który został opracowany przez Radę PCI Security Standards w celu ochrony danych kart płatniczych przed kradzieżą i nadużyciem.

Standard PCI składa się z 12 wymagań bezpieczeństwa informacji, które są podzielone na 6 kategorii:
+ Ochrona sieci: Wymagania te obejmują m.in. instalację i konfigurację zapor ogniowych, zapewnienie bezpieczeństwa sieci bezprzewodowych i utrzymanie zabezpieczeń przeciwko atakom sieciowym.
+ Ochrona danych kart płatniczych: Wymagania te dotyczą przechowywania, przetwarzania i przesyłania danych kart płatniczych. Obejmują one m.in. zapewnienie bezpiecznego przechowywania danych kart płatniczych, ograniczenie dostępu do tych danych tylko do niezbędnych pracowników i zabezpieczenie przesyłania danych za pomocą protokołu SSL.
+ Zarządzanie zabezpieczeniami: Wymagania te obejmują m.in. utrzymywanie polityki bezpieczeństwa informacji, regularne przeprowadzanie przeglądów zabezpieczeń i szkolenie pracowników w zakresie bezpieczeństwa informacji.
+ Wdrażanie i zarządzanie zabezpieczeniami systemów: Wymagania te dotyczą m.in. zapewnienia bezpieczeństwa systemów operacyjnych, aplikacji i urządzeń sieciowych oraz regularnego aktualizowania oprogramowania i systemów.
+ Monitorowanie i testowanie sieci: Wymagania te obejmują m.in. monitorowanie sieci w celu wykrycia nieprawidłowości i podejrzanych aktywności oraz regularne testowanie systemów w celu wykrycia luk w zabezpieczeniach.
+ Zarządzanie ryzykiem: Wymagania te obejmują m.in. identyfikację i ocenę ryzyka związanego z przetwarzaniem danych kart płatniczych oraz opracowanie planów awaryjnych w przypadku wystąpienia incydentu związanego z bezpieczeństwem informacji.

Przestrzeganie standardu PCI jest obowiązkowe dla firm, które przetwarzają, przechowują lub przesyłają dane kart płatniczych. Standard ten jest wymagany przez organizacje płatnicze, takie jak Visa, MasterCard, American Express i Discover, i ma na celu ochronę danych kart płatniczych przed kradzieżą i nadużyciem.


## 18.3. HIPAA

Ustawa Health Insurance Portability and Accountability Act (HIPAA) to profil zabezpieczeń skupiający się na ochronie danych EPHI. 

Reguła zabezpieczeń HIPAA skupia się w szczególności na ochronie informacji EPHI i tylko niektóre agencje mają podlegać regule zabezpieczeń HIPAA w oparciu o ich funkcję i korzystanie z informacji EPHI.

Reguła zabezpieczeń HIPAA skupia się na ochronie poufności, integralności i dostępności informacji EPHI zgodnie z definicją w regule zabezpieczeń.


## 18.4. GDRP

GDPR to rozporządzenie ogólne o ochronie danych osobowych, które weszło w życie w Europie 25 maja 2018 roku. Oto kilka standardów bezpieczeństwa GDPR:
+ Zasada minimalizacji danych - gromadzenie danych osobowych powinno być ograniczone do minimum potrzebnego do realizacji celów, dla których dane te są przetwarzane.
+ Pseudonimizacja - dane osobowe powinny być przetwarzane w sposób, który uniemożliwi ich identyfikację bez użycia dodatkowych informacji.
+ Ciągłość przetwarzania danych - dane osobowe powinny być przetwarzane w sposób, który zapewnia ich ciągłość, dostępność i integralność.
+ Zasada poufności - dane osobowe powinny być przetwarzane w sposób, który zapewnia ich poufność i ochronę przed nieuprawnionym dostępem.
+ Zasada przejrzystości - osoby, których dane dotyczą, powinny być poinformowane o przetwarzaniu ich danych i mieć możliwość wyrażenia lub nie wyrażenia na to zgody.
+ Zasada odpowiedzialności - podmioty przetwarzające dane osobowe powinny być odpowiedzialne za przestrzeganie zasad bezpieczeństwa danych osobowych.
+ Zasada prawo do zapomnienia - osoby, których dane dotyczą, powinny mieć prawo do usunięcia swoich danych osobowych, jeśli nie są one już potrzebne do celów, dla których zostały zebrane.
+ Zasada ochrony danych od dzieciństwa - dane osobowe dzieci powinny być przetwarzane w sposób szczególnie chroniący ich prywatność i bezpieczeństwo.
+ Zasada meldowania naruszeń ochrony danych osobowych - podmioty przetwarzające dane osobowe powinny zgłaszać wszystkie naruszenia ochrony danych osobowych odpowiednim organom.
+ Zasada przetwarzania danych osobowych tylko w celach, dla których zostały zebrane - dane osobowe powinny być przetwarzane tylko w celach, dla których zostały zebrane i nie powinny być przetwarzane dalej w sposób niezgodny z tymi celami.


## 18.5. OWASP

OWASP to organizacja non-profit, której celem jest poprawa bezpieczeństwa aplikacji internetowych. W ramach swojej działalności OWASP tworzy listy najczęstszych zagrożeń dla aplikacji internetowych oraz proponuje najlepsze praktyki dla tworzenia bezpiecznego oprogramowania. Jedną z najważniejszych inicjatyw OWASP jest lista OWASP Top 10, która zawiera dziesięć najczęstszych zagrożeń dla aplikacji internetowych. Poniżej przedstawiam standardowe zagrożenia uwzględnione na liście OWASP Top 10:
+ Iniekcje (Injection) - obejmują ataki, które polegają na wprowadzeniu niebezpiecznego kodu do aplikacji poprzez nieodpowiednie walidowanie lub brak sanityzacji danych.
+ Złamanie uwierzytelnienia i autoryzacji (Broken Authentication and Session Management) - obejmuje ataki na proces uwierzytelniania i autoryzacji użytkowników, takie jak haseł słabe lub wyciekające dane uwierzytelniające.
+ Wrażliwe dane (Sensitive Data Exposure) - obejmuje ataki, w których wrażliwe dane, takie jak hasła czy dane karty kredytowej, są przechowywane lub przesyłane w sposób niebezpieczny.
+ Nieprawidłowa konfiguracja serwera (XML External Entities (XXE)) - obejmuje ataki, w których nieprawidłowa konfiguracja serwera umożliwia atakującemu odczytanie wrażliwych informacji.
+ Złamanie funkcji kontroli dostępu (Broken Access Control) - obejmuje ataki, w których atakujący uzyskuje dostęp do zasobów, do których nie powinien mieć dostępu.
+ Złośliwe oprogramowanie (Security Misconfiguration) - obejmuje ataki, w których oprogramowanie jest źle skonfigurowane lub posiada niewłaściwe ustawienia, co umożliwia atakującemu dostęp do systemu.
+ Niepoprawna walidacja danych wejściowych (Cross-Site Scripting (XSS)) - obejmuje ataki, w których atakujący wprowadza kod JavaScript do aplikacji, który wykorzystuje błędy w walidacji danych wejściowych.
+ Niepoprawna konfiguracja zabezpieczeń (Insecure Deserialization) - obejmuje ataki, w których atakujący wprowadza specjalnie spreparowane dane, które wykorzystują błędy w procesie deserializacji.
+ Użycie komponentów z podatnościami (Using Components with Known Vulnerabilities) - obejmuje ataki, w których aplikacje wykorzystują komponenty, które posiadają znane podatności.
+ Niedostateczne rejestrowanie i monitorowanie (Insufficient Logging and Monitoring) - obejmuje ataki, w których brak odpowiednie

## 18.6. NIST Cybersecurity Framework

NIST Cybersecurity Framework to ramy opracowane przez National Institute of Standards and Technology (NIST) w celu zapewnienia ochrony infrastruktury krytycznej oraz innych organizacji przed zagrożeniami związanymi z bezpieczeństwem cybernetycznym. Framework składa się z pięciu podstawowych kategorii: Identyfikacja, Ochrona, Wykrycie, Reagowanie i Przywracanie.

+ Identyfikacja: w tej kategorii chodzi o określenie podatności i zagrożeń dla systemów i sieci, w tym ocenę ryzyka i zarządzanie tożsamością.
+ Ochrona: ta kategoria dotyczy działań mających na celu ochronę przed atakami, w tym wykrycie nieautoryzowanego dostępu, zarządzanie hasłami i szyfrowanie.
+ Wykrycie: w tej kategorii chodzi o monitorowanie systemów i sieci w celu szybkiego wykrycia incydentów i ataków oraz analizę logów i innych danych, które mogą pomóc w wykryciu zagrożeń.
+ Reagowanie: ta kategoria dotyczy szybkiej reakcji na incydenty i ataki, w tym reagowania na incydenty, przeprowadzania śledztw i przywracania systemów do stanu sprzed ataku.
+ Przywracanie: ta kategoria dotyczy działań mających na celu przywrócenie systemów i sieci do normalnego stanu po incydentach, w tym procesu weryfikacji i testowania systemów.

Framework NIST Cybersecurity jest elastyczny i może być dostosowany do potrzeb różnych organizacji. Poza tym, framework zawiera różne narzędzia, takie jak przykładowe polityki i procedury, które organizacje mogą wykorzystać do wdrożenia zasad bezpieczeństwa cybernetycznego. Framework NIST Cybersecurity może być również stosowany przez rządy i inne instytucje, które chcą zapewnić bezpieczeństwo swoich sieci i systemów informatycznych.

<p align="center">
Rys. 18.6.1. NIST Cyber Security Framework
<br>
  <img src="\assets\img\Sieci\58.png" width="650" alt="NIST">
</p>

# 19. Analiza podatności

Analiza podatności to proces oceny systemów informatycznych w celu zidentyfikowania potencjalnych słabości, które mogą być wykorzystane przez atakujących do przeprowadzenia ataku na system. Jest to ważna część procesu zapewniania bezpieczeństwa systemów informatycznych.

Podczas analizy podatności specjaliści od bezpieczeństwa informacyjnego stosują różne narzędzia i techniki, takie jak skanery podatności, narzędzia do testowania penetracyjnego, analizę kodu źródłowego, inspekcję w poszukiwaniu niezabezpieczonych konfiguracji, a także przeglądanie dokumentacji technicznej i innych informacji o systemie.

Celem analizy podatności jest zidentyfikowanie słabości w systemie, takich jak luki w zabezpieczeniach, niezaktualizowane oprogramowanie lub konfiguracje, które nie są odpowiednio zabezpieczone. Następnie specjaliści od bezpieczeństwa informacyjnego mogą opracować strategie i środki zaradcze, aby zminimalizować ryzyko wykorzystania tych podatności przez atakujących.

Analiza podatności jest istotna nie tylko dla systemów informatycznych, ale również dla innych rodzajów systemów, takich jak infrastruktura krytyczna, systemy kontrolne przemysłowe, urządzenia medyczne, itp. Wszystkie te systemy są podatne na ataki, które mogą prowadzić do zagrożenia dla zdrowia i życia ludzi oraz dla bezpieczeństwa narodowego. Dlatego ważne jest, aby regularnie przeprowadzać analizę podatności i dostosowywać środki bezpieczeństwa w celu minimalizowania ryzyka ataków.

Przeprowadzenie analizy podatności to złożony proces, który wymaga zaangażowania odpowiednich narzędzi i technik, a także doświadczenia w dziedzinie bezpieczeństwa informacyjnego. Poniżej przedstawiam krok po kroku, jak przeprowadzić analizę podatności:
+ Przygotowanie planu i celów analizy: W pierwszej kolejności należy zdefiniować cele i zakres analizy, aby określić, które systemy i aplikacje będą poddane testom, a także jakie rodzaje ataków i scenariuszy należy przetestować. Przygotowanie planu pomaga w skutecznym przeprowadzeniu analizy podatności i zapewnieniu, że wszystkie ważne elementy zostaną przeanalizowane.
+ Skanowanie podatności: Skanowanie podatności to proces automatycznego przeszukiwania systemów i aplikacji w celu wykrycia potencjalnych podatności. Skanowanie może być przeprowadzone za pomocą specjalistycznego oprogramowania, takiego jak Nessus, OpenVAS, QualysGuard i wiele innych. Skanowanie podatności pozwala na szybkie wykrycie potencjalnych zagrożeń, ale nie jest w stanie zidentyfikować wszystkich podatności.
+ Testowanie penetracyjne: Testowanie penetracyjne to proces manualnego przeprowadzania ataków na systemy i aplikacje, aby zidentyfikować słabości, które nie zostały wykryte podczas skanowania podatności. Testowanie penetracyjne może obejmować różne techniki, takie jak testowanie haseł, ataki typu SQL injection, ataki typu cross-site scripting (XSS) i wiele innych. Testowanie penetracyjne może być przeprowadzone ręcznie lub za pomocą specjalistycznego oprogramowania, takiego jak Metasploit, Core Impact lub Burp Suite.
+ Analiza kodu źródłowego: Analiza kodu źródłowego to proces oceny kodu aplikacji, aby zidentyfikować potencjalne luki w zabezpieczeniach. Analiza kodu źródłowego może pomóc w wykryciu podatności, które nie zostały wykryte podczas skanowania podatności lub testowania penetracyjnego. Do analizy kodu źródłowego można wykorzystać specjalistyczne narzędzia, takie jak Checkmarx, Fortify i wiele innych.
+ Inspekcja w poszukiwaniu niezabezpieczonych konfiguracji: Inspekcja w poszukiwaniu niezabezpieczonych konfiguracji to proces oceny ustawień i konfiguracji systemów i aplikacji, aby zidentyfikować potencjalne słabości. Inspekcja może obejmować takie rzeczy jak nieprawidłowo skonfigurowane serwery DNS, nieaktualne oprogramowanie, słabe hasła i wiele innych. Inspekcja może być przeprowadzana ręcznie lub za pomocą


# 20. Systemy operacyjne

System operacyjny (ang. Operating System, OS) to podstawowe oprogramowanie, które zarządza działaniem komputera lub urządzenia elektronicznego. OS zapewnia interakcję między użytkownikiem lub aplikacją a sprzętem, a także zarządza zasobami systemu, takimi jak procesory, pamięć, dyski twarde i inne urządzenia wejścia/wyjścia.

Systemy operacyjne są kluczowe dla działania komputerów i innych urządzeń elektronicznych. Bez systemu operacyjnego urządzenie elektroniczne byłoby niemożliwe do uruchomienia lub działania.

Rodzaje systemów operacyjnych:
+ Systemy operacyjne desktopowe: przeznaczone dla komputerów osobistych i oferujące interfejs użytkownika w postaci pulpitu. Do systemów operacyjnych desktopowych należą np. Windows, macOS, Linux, Chrome OS.
+ Systemy operacyjne serwerowe: zaprojektowane do obsługi aplikacji i usług sieciowych, takich jak serwery WWW, bazy danych itp. Systemy operacyjne serwerowe zapewniają wydajność, niezawodność i skalowalność. Do systemów operacyjnych serwerowych należą np. Windows Server, Linux, Unix.
+ Systemy operacyjne mobilne: przeznaczone dla urządzeń przenośnych, takich jak smartfony i tablety. Systemy operacyjne mobilne oferują interfejs użytkownika oparty na dotyku i są zoptymalizowane pod kątem energooszczędności. Do systemów operacyjnych mobilnych należą np. Android, iOS, Windows Mobile.
+ Systemy operacyjne wbudowane: zaprojektowane do urządzeń elektronicznych, takich jak routery, telewizory, kasy fiskalne, automaty do gier itp. Systemy operacyjne wbudowane są zazwyczaj zoptymalizowane pod kątem małej mocy obliczeniowej i ograniczonej pamięci. Do systemów operacyjnych wbudowanych należą np. FreeRTOS, ThreadX, VxWorks.

Systemy operacyjne są zazwyczaj zoptymalizowane pod kątem określonych zastosowań, co oznacza, że wybór systemu operacyjnego powinien być dostosowany do potrzeb użytkownika. Każdy system operacyjny ma swoje wady i zalety, a wybór odpowiedniego systemu zależy od indywidualnych potrzeb i wymagań użytkownika.


## 20.1. Windows

System operacyjny Windows to rodzina systemów operacyjnych opracowanych przez firmę Microsoft. Jest to jeden z najpopularniejszych systemów operacyjnych na świecie, który działa na większości komputerów osobistych i wielu innych urządzeniach, takich jak tablety, smartfony, konsolki do gier i wiele innych.

System operacyjny Windows to rodzina systemów operacyjnych opracowanych przez firmę Microsoft. Jest to jeden z najpopularniejszych systemów operacyjnych na świecie, który działa na większości komputerów osobistych i wielu innych urządzeniach, takich jak tablety, smartfony, konsolki do gier i wiele innych.

Windows działa na podstawie jądra systemu operacyjnego, które zapewnia podstawowe usługi dla programów, które działają w systemie. Jądro Windows zapewnia między innymi obsługę sprzętu, obsługę pamięci, zarządzanie procesami, zarządzanie plikami i katalogami oraz obsługę sieci.

Interfejs użytkownika w Windowsie opiera się na tzw. "oknach", czyli osobnych obszarach ekranu, w których wyświetlane są programy i pliki. Użytkownik może korzystać z myszy lub klawiatury, aby poruszać się między oknami, wybierać opcje z menu i wprowadzać dane.

System operacyjny Windows działa na poziomie sprzętu i programowym, a jego działanie można podzielić na kilka kluczowych obszarów:
+ Zarządzanie sprzętem: Windows działa na poziomie sprzętowym poprzez jądro systemu operacyjnego, które odpowiada za obsługę urządzeń, takich jak procesory, pamięć RAM, dyski twarde, karty graficzne, klawiatury, myszy i wiele innych. Jądro systemu operacyjnego zapewnia interfejs między sprzętem a oprogramowaniem, umożliwiając aplikacjom korzystanie z różnych urządzeń.
+ Zarządzanie procesami: Windows zarządza procesami na poziomie programowym, czyli aplikacji, które działają na komputerze. Procesy to programy, które są uruchomione na komputerze i wykonywane przez procesor. Windows zarządza procesami poprzez menedżer zadań, który umożliwia użytkownikom monitorowanie i kontrolowanie procesów.
+ Zarządzanie pamięcią: Windows zarządza pamięcią na poziomie programowym, co oznacza, że system operacyjny kontroluje, która aplikacja może korzystać z pamięci i jak wiele pamięci może wykorzystać. Windows wykorzystuje algorytmy do zarządzania pamięcią, które umożliwiają przydzielanie i zwalnianie pamięci w zależności od potrzeb aplikacji.
+ Zarządzanie plikami i katalogami: Windows zarządza plikami i katalogami na poziomie programowym poprzez eksplorator plików, który umożliwia użytkownikom przeglądanie plików i katalogów na komputerze oraz wykonywanie operacji na plikach, takich jak kopiowanie, przenoszenie i usuwanie.
+ Interfejs użytkownika: Windows udostępnia interfejs użytkownika, który umożliwia użytkownikom interakcję z systemem operacyjnym. Interfejs użytkownika Windows składa się z wielu elementów, takich jak pasek zadań, menu startowe, ikony, okna i wiele innych. Windows obsługuje różne tryby interakcji z użytkownikiem, takie jak tryb tekstowy i graficzny, co umożliwia korzystanie z systemu na różnych urządzeniach.

Podsumowując, Windows działa na poziomie sprzętowym i programowym, umożliwiając aplikacjom korzystanie z różnych urządzeń i dostarczając interfejs użytkownika, który umożliwia interakcję z systemem. System operacyjny Windows jest ciągle rozwijany i ulepszany przez Microsoft, co umożliwia użytkownikom korzystanie z nowych funkcji i usprawnień.


## 20.2. Linux

System operacyjny Linux to rodzaj oprogramowania open-source, który został stworzony w 1991 roku przez Linusa Torvaldsa. Linux jest jednym z najpopularniejszych systemów operacyjnych, a jego popularność wynika z wielu czynników, w tym z faktu, że jest bezpłatny i dostępny na różne platformy sprzętowe.

Linux składa się z kilku podsystemów, które zapewniają różne funkcjonalności. Oto kilka z tych podsystemów i funkcjonalności:
+ Jądro systemu: To podstawowy komponent systemu, który odpowiada za zarządzanie zasobami sprzętowymi, takimi jak procesory, pamięć, dyski twarde, karty sieciowe i inne. Jądro Linux jest modułowe, co oznacza, że można łatwo dodawać lub usuwać moduły, aby dostosować system do potrzeb użytkownika.
+ System plików: Linux wykorzystuje system plików do przechowywania i organizowania danych na dysku twardym. Linux obsługuje wiele różnych systemów plików, takich jak Ext4, Btrfs, XFS, FAT i NTFS. Systemy plików umożliwiają użytkownikom organizowanie i przetwarzanie danych w sposób efektywny i bezpieczny.
+ Środowisko graficzne: Linux oferuje kilka różnych środowisk graficznych, takich jak GNOME, KDE, XFCE i wiele innych. Środowiska graficzne umożliwiają użytkownikom interakcję z systemem za pomocą ikon, okien, menu i innych graficznych elementów interfejsu użytkownika.
+ Narzędzia wiersza poleceń: Linux oferuje wiele narzędzi wiersza poleceń, które umożliwiają użytkownikom wykonywanie różnych operacji, takich jak przeglądanie plików, kopiowanie, usuwanie, instalowanie oprogramowania i wiele innych. Narzędzia wiersza poleceń są szczególnie przydatne dla programistów i administratorów systemów, którzy często muszą pracować z tekstem i skryptami.
+ Programy użytkowe: Linux oferuje wiele programów użytkowych, takich jak przeglądarki internetowe, edytory tekstowe, odtwarzacze multimedialne, klienty poczty elektronicznej, narzędzia do edycji obrazów i wiele innych. Programy użytkowe umożliwiają użytkownikom wykorzystanie różnych funkcjonalności systemu i służą do wykonywania codziennych zadań.

Linux ma wiele zalet, takich jak bezpłatność, otwartość kodu źródłowego, stabilność, bezpieczeństwo i dużą elastyczność. System ten jest szczególnie popularny wśród programistów, administratorów systemów oraz w środowiskach naukowych i badawczych, gdzie wykorzystuje się wiele narzędzi open-source i potrzebna jest duża kontrola nad systemem. Linux jest również powszechnie stosowany w serwerach internetowych, usługach chmurowych i innych systemach, które wymagają dużych zasobów sprzętowych i elastyczności.

Linux jest również bardzo elastyczny i dostosowany do różnych potrzeb użytkowników. Użytkownicy mogą dostosować system do swoich potrzeb poprzez wybór odpowiedniego systemu plików, środowiska graficznego, narzędzi wiersza poleceń i innych komponentów systemu.

Jednym z najważniejszych aspektów Linuxa jest jego model dystrybucji. Linux jest dostępny w postaci tzw. dystrybucji, czyli zestawu oprogramowania, który obejmuje jądro systemu, system plików, narzędzia wiersza poleceń, programy użytkowe i wiele innych komponentów. Istnieje wiele różnych dystrybucji Linuxa, takich jak Ubuntu, Fedora, Debian, Arch Linux i wiele innych. Każda dystrybucja Linuxa ma swoje własne cechy i cechy charakterystyczne, co umożliwia użytkownikom wybór najlepszego rozwiązania dla swoich potrzeb.

Ogólnie rzecz biorąc, Linux jest systemem operacyjnym o otwartym kodzie źródłowym, który oferuje użytkownikom wiele funkcjonalności, elastyczność i kontrolę nad systemem. Linux jest szczególnie popularny wśród programistów, administratorów systemów, naukowców i badaczy, a także wśród użytkowników, którzy szukają stabilnego i bezpiecznego systemu, który może być dostosowany do ich potrzeb.


## 20.3. MacOS

System operacyjny MacOS to system operacyjny firmy Apple, który jest używany w komputerach Macintosh (Mac) i notebookach MacBook. MacOS został pierwotnie wydany w 1984 roku jako pierwszy system operacyjny z interfejsem graficznym użytkownika (GUI) i był rozwijany na przestrzeni lat, wraz z wprowadzeniem nowych wersji i aktualizacji.

Jednym z najważniejszych elementów MacOS jest interfejs użytkownika, który jest znacznie różni się od interfejsów innych systemów operacyjnych. System MacOS używa nakładki graficznej o nazwie Aqua, która oferuje wiele efektów graficznych, przejść i animacji. Interfejs Aqua jest zintegrowany z pulpitem i umożliwia łatwe zarządzanie plikami i folderami.

MacOS jest oparty na jądrze systemu Unix, co oznacza, że jest wysoce skalowalny, stabilny i bezpieczny. System MacOS ma wiele wbudowanych narzędzi do zarządzania plikami, przeglądania internetu, pracy z dokumentami i innymi czynnościami, które zwykle wymagają instalacji oprogramowania w innych systemach operacyjnych.

W MacOS istnieją również wbudowane narzędzia do tworzenia i edycji multimediów, takie jak iMovie do edycji wideo i GarageBand do edycji dźwięku. Wszystkie te narzędzia są łatwe w użyciu i oferują wysoką jakość wytwarzanych treści.

System MacOS jest również znany z bezpieczeństwa i prywatności. W porównaniu z innymi systemami operacyjnymi, MacOS ma mniej problemów z wirusami i innymi zagrożeniami bezpieczeństwa. Istnieje również wiele wbudowanych narzędzi, takich jak zapora sieciowa i szyfrowanie plików, które pomagają użytkownikom chronić swoje dane.

Podsumowując, MacOS to zaawansowany system operacyjny, który oferuje użytkownikom wiele funkcjonalności i narzędzi, które ułatwiają codzienną pracę i korzystanie z multimediów. System MacOS jest również znany z bezpieczeństwa i stabilności, co czyni go popularnym wyborem wśród profesjonalistów, kreatywnych i wymagających użytkowników.


# 21. Usługi sieciowe

Usługi sieciowe to aplikacje, które są uruchamiane na serwerach i udostępniają zasoby lub funkcjonalność dla klientów, którzy łączą się z tymi serwerami za pośrednictwem sieci komputerowej. Usługi sieciowe pozwalają użytkownikom na wykonywanie różnych zadań, takich jak udostępnianie plików, drukowanie, udostępnianie połączenia internetowego, przesyłanie poczty elektronicznej, a także wykonanie zaawansowanych operacji, takich jak analiza danych czy obliczenia naukowe.

Usługi sieciowe są zwykle dostępne przez sieć lokalną lub przez Internet. Serwery udostępniające usługi sieciowe są zwykle konfigurowane w taki sposób, aby kontrolować dostęp do zasobów sieciowych i udostępniać je tylko uprawnionym użytkownikom lub klientom. Aby korzystać z usług sieciowych, klient musi zwykle zainstalować odpowiednie oprogramowanie klienta, które pozwoli mu na połączenie się z serwerem i uzyskanie dostępu do usług.

Przykładami popularnych usług sieciowych są:
+ Serwer plików, który pozwala użytkownikom na udostępnianie i pobieranie plików w sieci lokalnej lub przez Internet.
+ Serwer drukowania, który umożliwia użytkownikom drukowanie dokumentów z różnych komputerów w sieci.
+ Serwer poczty elektronicznej, który umożliwia użytkownikom przesyłanie i odbieranie wiadomości e-mail.
+ Serwer bazy danych, który umożliwia dostęp do przechowywanych danych i informacji.
+ Serwer WWW, który umożliwia udostępnianie stron internetowych i aplikacji internetowych.

Usługi sieciowe są kluczowe dla wielu organizacji i firm, ponieważ pozwalają na udostępnianie i koordynowanie pracy wielu użytkowników na różnych komputerach. Dzięki usługom sieciowym pracownicy mogą łatwiej udostępniać i korzystać z zasobów i informacji w firmie, co prowadzi do większej efektywności i wydajności pracy.

## 21.1. Metabase

Metabase to darmowe oprogramowanie typu open-source do tworzenia interaktywnych i łatwych w użyciu raportów biznesowych i analiz danych. Jest to narzędzie, które umożliwia użytkownikom łatwe połączenie i analizowanie danych z różnych źródeł, takich jak bazy danych, pliki CSV czy API.

Metabase umożliwia tworzenie wizualizacji danych za pomocą wbudowanych narzędzi, takich jak wykresy, tabele i mapy. Narzędzie to oferuje prosty interfejs graficzny, który umożliwia łatwe tworzenie pytań do bazy danych oraz tworzenie interaktywnych raportów i paneli. Dzięki temu użytkownicy mogą szybko i łatwo przeglądać, analizować i prezentować swoje dane.

Metabase jest zintegrowane z wieloma popularnymi bazami danych, takimi jak MySQL, PostgreSQL, Microsoft SQL Server czy Oracle, co umożliwia łatwe połączenie i analizowanie danych z różnych źródeł. Narzędzie to oferuje również wiele wbudowanych funkcji i opcji, takich jak zapytania SQL, grupowanie danych, filtrowanie i sortowanie, dzięki czemu użytkownicy mogą dostosować i zoptymalizować swoje raporty i analizy.

Metabase jest narzędziem, które jest stosunkowo łatwe w użyciu i nie wymaga dużej wiedzy technicznej. Jest to idealne rozwiązanie dla małych i średnich przedsiębiorstw, które potrzebują prostego narzędzia do analizowania i prezentowania swoich danych biznesowych. Ponadto, ze względu na swój otwarty kod źródłowy, Metabase oferuje wiele opcji dostosowywania i rozszerzania, co czyni go idealnym narzędziem dla programistów i osób zainteresowanych rozwojem oprogramowania.

### Jak działa Metabase?

Metabase działa jako warstwa pośrednicząca pomiędzy użytkownikami a bazą danych. Narzędzie to umożliwia użytkownikom łatwe połączenie i analizowanie danych z różnych źródeł, takich jak bazy danych, pliki CSV czy API.

Po zainstalowaniu i skonfigurowaniu Metabase, użytkownicy mogą łączyć się z różnymi źródłami danych i tworzyć pytania SQL za pomocą wbudowanego interfejsu graficznego lub edytora zapytań SQL. Metabase pozwala na łączenie się z wieloma popularnymi bazami danych, takimi jak MySQL, PostgreSQL, Microsoft SQL Server czy Oracle, a także z plikami CSV, Excel i API.

Głównym zadaniem Metabase jest analiza i prezentacja danych w sposób łatwy do zrozumienia i interaktywny. Narzędzie to oferuje wiele wbudowanych funkcji i opcji, takich jak zapytania SQL, grupowanie danych, filtrowanie i sortowanie, a także wiele różnych wizualizacji danych, takich jak wykresy, tabele i mapy.

Metabase wykorzystuje wiele różnych technologii, takich jak Clojure, Java, JavaScript, React i D3.js. Narzędzie to działa na serwerze, ale interfejs jest dostępny przez przeglądarkę internetową, co umożliwia użytkownikom dostęp do Metabase z dowolnego miejsca i urządzenia.

Metabase jest narzędziem, które jest stosunkowo łatwe w użyciu i nie wymaga dużej wiedzy technicznej. Narzędzie to oferuje również wiele opcji dostosowywania i rozszerzania, co czyni je idealnym narzędziem dla programistów i osób zainteresowanych rozwojem oprogramowania.

### Jak skonfigurować?

~~~
Instalacja Javy:
apt update
apt install default-jdk
java -version

Instalacja Postgresa:
apt install postgresql

mcedit /etc/postgresql/13/main/postgresql.conf
W nim ustawiamy:
datestyle = 'European, German'
#intervalstyle = 'postgres'
timezone = 'Poland'

systemctl start postgresql
systemctl start postgresql
su - postgres
createuser -d -P -e -W dbuser
createdb -e -E UTF-8 -O dbuser testdb
createuser -d -P -e -W metuser
createdb -e -E UTF-8 -O metuser metdb
psql -h localhost -U dbuser -W testdb

Instalacja testowej bazy danych:
wget ...
scp ./northwind.sql stud@192.168.1.X:
psql -h localhost -U dbuser -W testdb<./northwind.sql

Instalacja Metabase:
mkdir /opt/metabase
wget "http://pei.prz.edu.pl/sint/duze_pliki/metabase.jar" /opt/metabase/metabase.jar
cd /opt/metabase
java -jar metabase.jar
groupadd -r metabase
useradd -r -s /bin/false -g metabase metabase
chown -R metabase:metabase /opt/metabase
touch /var/log/metabase.log
chown root:adm /var/log/metabase.log
touch /etc/default/metabase
chmod 640 /etc/default/metabase
touch /etc/systemd/system/metabase.service
mcedit /etc/systemd/system/metabase.service

Do pliku wkleić zawartość i zapisać:
[Unit]
Description=Metabase server
After=syslog.target
After=network.target
   
[Service]
WorkingDirectory=/opt/metabase
ExecStart=/usr/bin/java -jar /opt/metabase/metabase.jar
EnvironmentFile=/etc/default/metabase
User=metabase
Type=simple
StandardOutput=syslog
StandardError=syslog
SyslogIdentifier=metabase
SuccessExitStatus=143
TimeoutStopSec=120
Restart=always

[Install]
WantedBy=multi-user.target

Środowsko metabase:
mcedit /etc/default/metabase

Umieszczemy w nim:
MB_PASSWORD_COMPLEXITY=normal
MB_PASSWORD_LENGTH=5
MB_JETTY_HOST=0.0.0.0
MB_JETTY_PORT=3000
MB_DB_TYPE=postgres
MB_DB_DBNAME=metdb
MB_DB_PORT=5432
MB_DB_USER=metuser
MB_DB_PASS=osource
MB_DB_HOST=localhost
MB_EMOJI_IN_LOGS=true


systemctl daemon-reload
systemctl start metabase
systemctl status metabase
systemctl enable metabase.service

Konfiguracja nginx - alternatywa:
apt remove apache2
apt install nginx
systemctl status nginx
mcedit /etc/nginx/sites-available/default

Umieszczamy w pliku:
# sample nginx.conf
  location / {
    proxy_pass http://127.0.0.1:3000;
  }

systemctl restart nginx

Konfiguracja Apache - alternatywa:
a2enmod proxy
a2enmod proxy_http
a2enmod proxy_balancer
a2enmod lbmethod_byrequests
Dodajemy dyrektywę location:
<Location "/">
  ProxyPass "http://127.0.0.1:3000/"
</Location>

systemctl restart apache2
~~~


## 21.2. Perl

Perl jest językiem programowania, który umożliwia programistom tworzenie usług sieciowych. Usługi sieciowe napisane w Perl mogą być uruchamiane na serwerach WWW i umożliwiają klientom dostęp do różnych funkcji i danych za pośrednictwem sieci.

Przykładowe usługi sieciowe napisane w Perl to systemy CMS (Content Management System) lub blogowe, narzędzia do analizy danych lub generowania raportów, a także narzędzia do automatyzacji procesów biznesowych.

Przy tworzeniu usługi sieciowej w Perl ważne jest zapewnienie bezpieczeństwa, niezawodności oraz wydajności. W tym celu programiści muszą stosować dobre praktyki programistyczne i dbać o odpowiednie zarządzanie pamięcią, obsługę błędów oraz optymalizację kodu.

Wiele narzędzi dostępnych w Perl ułatwia tworzenie usług sieciowych, takich jak moduły Net::Server, CGI::Application, Catalyst czy Dancer. Te narzędzia umożliwiają programistom szybkie tworzenie usług sieciowych, a także zapewniają narzędzia do testowania, debugowania i monitorowania aplikacji.

Usługi sieciowe napisane w Perl zazwyczaj korzystają z protokołów sieciowych takich jak HTTP, FTP, SMTP czy POP3. Programiści mogą wykorzystać biblioteki dostępne w Perl, takie jak LWP (Library for WWW in Perl), Net::FTP czy Net::SMTP, aby obsługiwać te protokoły.
W sumie, Perl jest jednym z popularnych języków programowania wykorzystywanych do tworzenia usług sieciowych. Z jego bogatej oferty modułów i narzędzi, programiści mogą szybko i łatwo tworzyć różnego rodzaju aplikacje sieciowe i usługi.

## 21.3. Hadoop

Hadoop to darmowy, otwartoźródłowy system do przetwarzania danych rozproszonych. Jest on zaprojektowany do obsługi ogromnych zbiorów danych, które mogą być przechowywane i przetwarzane na wielu maszynach w klastrze. Hadoop jest wykorzystywany w wielu dziedzinach, w tym w analizie danych, eksploracji danych i uczeniu maszynowym.

Hadoop składa się z dwóch głównych komponentów: Hadoop Distributed File System (HDFS) i MapReduce.

HDFS jest systemem plików zaprojektowanym do przechowywania dużych zbiorów danych. Dane są dzielone na mniejsze części i replikowane na różnych węzłach klastra w celu zapewnienia niezawodności i skalowalności. HDFS udostępnia narzędzia do zarządzania plikami, takie jak dodawanie, usuwanie, przenoszenie i zmienianie nazwy plików.

<p align="center">
Rys. 21.3.1. Hadoop
<br>
  <img src="\assets\img\Sieci\59.png" width="650" alt="Hadoop">
</p>

MapReduce to model programowania do przetwarzania danych rozproszonych. Programy MapReduce są pisane w języku Java lub innym języku programowania, który może być skompilowany do kodu bytecode Javy. Program MapReduce składa się z dwóch funkcji: map i reduce. Funkcja map pobiera dane z HDFS i przetwarza je w sposób niezależny od innych części danych. Wynik funkcji map jest następnie przekazywany do funkcji reduce, która przetwarza dane wejściowe i zwraca wynik.

Hadoop obsługuje wiele narzędzi i bibliotek, które ułatwiają programistom pracę z dużymi zbiorami danych. Na przykład, Hadoop Streaming umożliwia programowanie w językach innych niż Java, takich jak Python czy Ruby. Hadoop Hive umożliwia zapytania SQL na danych przechowywanych w HDFS. Hadoop Pig jest językiem skryptowym do przetwarzania danych, który jest łatwy w użyciu dla osób, które nie są programistami.

Hadoop oferuje również narzędzia do monitorowania i zarządzania klastrami, takie jak Hadoop YARN i Apache Ambari. Te narzędzia umożliwiają administratorom systemów zarządzanie zasobami klastra i zapewnienie niezawodności i skalowalności.

Podsumowując, Hadoop to system do przetwarzania danych rozproszonych, który składa się z HDFS do przechowywania danych i MapReduce do przetwarzania danych. Hadoop oferuje wiele narzędzi i bibliotek do pracy z dużymi zbiorami danych oraz narzędzia do zarządzania klastrami. Jest to popularne narzędzie w dziedzinie analizy danych i uczenia maszynowego, ze względu na swoją zdolność do obsługi ogromnych zbiorów danych i łatwej skalowalności.

## 21.4. Kafka

Apache Kafka to open-source'owy system przetwarzania strumieniowego, który umożliwia przetwarzanie i przesyłanie dużych ilości danych w czasie rzeczywistym. Kafka jest wykorzystywana w wielu dziedzinach, w tym w analizie danych, przetwarzaniu w czasie rzeczywistym, przetwarzaniu logów i systemach monitorujących.

Kafka opiera się na architekturze publikuj-subskrybuj, w której nadawca publikuje wiadomości na temacie, a odbiorcy subskrybują dany temat w celu odbierania wiadomości. Kafka składa się z trzech głównych komponentów: producentów, brokerów i konsumentów.

Producent jest odpowiedzialny za wysyłanie wiadomości do Kafki. Kafkowy producent może publikować wiadomości w wielu tematach, a każda wiadomość jest automatycznie przypisana do partycji tematu. Producent może być skonfigurowany w celu zapewnienia spójności danych i niezawodności, takiej jak potwierdzenia zapisu danych.

Broker to serwer Kafka, który przechowuje partycje tematów i umożliwia konsumentom subskrypcję wiadomości z tematu. Każdy broker jest skonfigurowany jako członek klastra Kafka, co umożliwia łatwe skalowanie i równoważenie obciążenia.

Konsument odbiera wiadomości z tematu. Kafkowy konsument może subskrybować jeden lub wiele tematów i przetwarzać dane w czasie rzeczywistym. Konsument może być skonfigurowany w celu przetwarzania danych z określonych partycji, aby umożliwić równoległe przetwarzanie danych.
Kafka oferuje wiele zalet, takich jak wysoka wydajność i skalowalność, niezawodność i spójność danych oraz łatwość obsługi. Kafka umożliwia również łatwe integrowanie z innymi narzędziami, takimi jak Hadoop, Spark i Flink. Ponadto Kafka oferuje wiele narzędzi i bibliotek, takich jak Kafka Connect i Kafka Streams, które ułatwiają pracę z danymi strumieniowymi.

Podsumowując, Apache Kafka to system przetwarzania strumieniowego, który umożliwia przetwarzanie i przesyłanie dużych ilości danych w czasie rzeczywistym. Kafka opiera się na architekturze publikuj-subskrybuj i składa się z trzech głównych komponentów: producentów, brokerów i konsumentów. Kafka oferuje wiele zalet, takich jak wysoka wydajność i skalowalność, niezawodność i spójność danych oraz łatwość obsługi.

<p align="center">
Rys. 21.4.1. Kafka
<br>
  <img src="\assets\img\Sieci\60.png" width="650" alt="Kafka">
</p>


## 21.5.1. ActiveMQ

Apache ActiveMQ to oprogramowanie do przesyłania wiadomości oparte na standardzie JMS (Java Message Service). Jest to oprogramowanie open-source napisane w języku Java, które umożliwia tworzenie i zarządzanie kolejkami wiadomości.

Główną ideą ActiveMQ jest przesyłanie wiadomości pomiędzy różnymi aplikacjami lub systemami, które są w stanie obsługiwać JMS. Dzięki temu, aplikacje mogą działać oddzielnie, a jednocześnie wymieniać między sobą dane, bez konieczności bezpośredniego połączenia.

ActiveMQ składa się z kilku głównych komponentów, takich jak broker, producenci, konsumenci i klienci. Broker to serwer, który obsługuje połączenia między producentami a konsumentami. Producent jest odpowiedzialny za wysyłanie wiadomości, a konsument za ich odbieranie. Klienci to aplikacje, które korzystają z usług ActiveMQ.

ActiveMQ obsługuje różne rodzaje wiadomości, takie jak jednokierunkowe (np. powiadomienia), dwukierunkowe (np. żądania i odpowiedzi) i wiele innych. Wiadomości są przechowywane w kolejkach, które umożliwiają ich dostarczenie w kolejności, w jakiej zostały odebrane.

ActiveMQ oferuje również wiele funkcjonalności, takich jak klastrowanie, replikacja i partycjonowanie, co pozwala na zwiększenie wydajności i niezawodności systemu. Dodatkowo, ActiveMQ umożliwia integrację z różnymi systemami i aplikacjami, co czyni go jednym z popularniejszych rozwiązań do przesyłania wiadomości.

<p align="center">
Rys. 21.5.1. ActiveMQ
<br>
  <img src="\assets\img\Sieci\61.png" width="650" alt="ActiveMQ">
</p>


## 21.6. Camel 

Apache Camel to open-source'owy framework dla platformy Java, który umożliwia integrację systemów opartych na różnych technologiach. Jego głównym zadaniem jest ułatwienie komunikacji pomiędzy różnymi aplikacjami, usługami oraz systemami poprzez przetwarzanie i przekazywanie danych w formacie wiadomości.

<p align="center">
Rys. 21.6.1. Camel 
<br>
  <img src="\assets\img\Sieci\62.png" width="650" alt="Camel">
</p>

Apache Camel posiada wiele wbudowanych komponentów, które umożliwiają integrację z różnymi protokołami, bazami danych, systemami plików, narzędziami ETL (Extract, Transform, Load) i wieloma innymi. Oprócz wbudowanych komponentów, Camel umożliwia także tworzenie własnych rozszerzeń i integracji.

Camel korzysta z różnych wzorców integracyjnych, takich jak: routery, transformery, filtrowanie, agregacja, oczekiwanie na odpowiedź, obsługa błędów, transakcje i wiele innych. Użytkownicy Camel mogą definiować szablony (tzw. route) integracji, które pozwalają na łatwe definiowanie, konfigurację i zarządzanie procesami przetwarzania wiadomości.

W Camel ważną koncepcją jest tzw. Exchange - obiekt reprezentujący przetwarzanie wiadomości w systemie. Exchange składa się z nagłówka, ciała oraz informacji dotyczących transakcji i kontekstu przetwarzania. Dzięki temu Camel pozwala na prostą i efektywną manipulację danymi.

<p align="center">
Rys. 21.6.3. Camel 
<br>
  <img src="\assets\img\Sieci\63.png" width="650" alt="Camel-1">
</p>

Jednym z najważniejszych cech Camel jest jego elastyczność. Framework jest niezależny od konkretnej platformy, dzięki czemu pozwala na integrację różnych systemów i aplikacji bez konieczności zmiany istniejącej infrastruktury. Oprócz tego Camel oferuje wiele narzędzi umożliwiających monitorowanie, debugowanie oraz zarządzanie procesami integracyjnymi.


## 21.7. Apache Kylin

Apache Kylin to otwarty framework analityczny zaprojektowany do pracy z dużymi zbiorami danych. Jest to rozwiązanie do przetwarzania hurtowni danych w czasie rzeczywistym i umożliwia generowanie raportów z ogromnych zestawów danych w bardzo krótkim czasie.

Kylin pozwala na integrację z różnymi źródłami danych, w tym z systemami relacyjnymi, NoSQL, Hadoop i innych. Framework wykorzystuje technologię OLAP (Online Analytical Processing) oraz Cubing, czyli proces tworzenia kostek OLAP, które są wykorzystywane do generowania raportów i analizy danych.

Kylin składa się z kilku modułów, które umożliwiają integrację, przetwarzanie i analizę danych. Główne moduły to:
+ Moduł budowania kostek (Cube Build): Moduł ten umożliwia tworzenie kostek OLAP z danych źródłowych. Kylin obsługuje wiele formatów danych, w tym Apache Hadoop HDFS, Apache HBase, Apache Parquet i inne. Kostki mogą być budowane z różnych źródeł danych, a następnie agregowane i przetwarzane w czasie rzeczywistym, aby zapewnić szybką i efektywną analizę danych.
+ Moduł zapytań (Query): Moduł ten umożliwia generowanie raportów i analizowanie danych z wykorzystaniem języka SQL. Kylin oferuje wiele funkcjonalności takich jak filtrowanie, grupowanie, sortowanie, agregacja, a także obsługuje wiele funkcji analitycznych. Dodatkowo, Kylin oferuje interfejs REST API, który umożliwia integrację z innymi aplikacjami.
+ Moduł administracyjny (Admin): Moduł ten pozwala na zarządzanie i konfigurację Kylin. Oferuje wiele narzędzi, takich jak interfejs webowy, wiersz poleceń, czy narzędzia do monitorowania i debugowania.

Kylin został zaprojektowany z myślą o skalowalności, wydajności i elastyczności. Framework działa w środowisku Hadoop, co pozwala na wykorzystanie mocy obliczeniowej wielu maszyn. Kylin oferuje także wiele narzędzi do monitorowania i zarządzania systemem, dzięki czemu jest łatwy w użyciu i administracji.

<p align="center">
Rys. 21.7.1. Apache Kylin
<br>
  <img src="\assets\img\Sieci\64.png" width="650" alt="Apache Kylin">
</p>


## 21.8. OpenVPN
OpenVPN to otwarte oprogramowanie służące do tworzenia prywatnych sieci wirtualnych (Virtual Private Networks - VPN) poprzez protokół SSL/TLS. OpenVPN jest używany do łączenia urządzeń z siecią VPN w celu bezpiecznego przesyłania danych między nimi.

Podstawowym celem OpenVPN jest umożliwienie bezpiecznego połączenia dwóch lub więcej urządzeń znajdujących się w różnych sieciach, tak aby były one widoczne dla siebie tak, jakby były połączone w jedną sieć lokalną. OpenVPN wykorzystuje silne algorytmy szyfrowania i autoryzacji, takie jak AES, Blowfish, RSA i SHA, aby zapewnić bezpieczeństwo i poufność danych przesyłanych w sieci VPN.

OpenVPN działa w oparciu o architekturę klient-serwer. Serwer OpenVPN obsługuje wiele klientów, a każdy klient połączony jest z serwerem za pomocą tunelu VPN. OpenVPN może działać na wielu systemach operacyjnych, w tym na Windows, Linux, macOS, iOS i Android.

Konfiguracja OpenVPN jest bardzo elastyczna, co pozwala na dostosowanie ustawień sieci VPN do indywidualnych potrzeb użytkownika. OpenVPN oferuje wiele opcji konfiguracyjnych, takich jak konfiguracja protokołu, konfiguracja algorytmów szyfrowania i autoryzacji, oraz konfiguracja adresów IP i tuneli VPN.

OpenVPN zapewnia także wiele funkcjonalności, takich jak obsługa wielu połączeń VPN, równoważenie obciążenia, rozszerzalność i skalowalność. Dzięki temu OpenVPN może być stosowany zarówno w małych, jak i dużych sieciach VPN.

W celu ułatwienia korzystania z OpenVPN, dostępne są różne narzędzia graficzne i interfejsy użytkownika, takie jak OpenVPN GUI, OpenVPN Connect i inne. Ponadto, OpenVPN jest łatwy w instalacji i konfiguracji, dzięki czemu może być używany przez użytkowników z różnym poziomem zaawansowania technicznego.

<p align="center">
Rys. 21.8.1. OpenVPN
<br>
  <img src="\assets\img\Sieci\65.png" width="650" alt="OpenVPN">
</p>


## 21.9. Tomcat

Tomcat to serwer aplikacji napisany w języku Java, który umożliwia uruchamianie aplikacji webowych opartych na technologii Java Servlet i JavaServer Pages (JSP). Jest to oprogramowanie typu open-source, rozwijane przez Apache Software Foundation. Tomcat może być uruchamiany na różnych systemach operacyjnych, takich jak Windows, Linux i macOS.

Tomcat działa jako kontener servletów, który zarządza i obsługuje żądania HTTP wysyłane do aplikacji webowej. Żądania HTTP są przesyłane do Tomcat za pośrednictwem serwera internetowego (np. Apache HTTP Server) lub bezpośrednio do Tomcat. Tomcat przetwarza te żądania, uruchamia odpowiednie servlety i wyświetla odpowiedź na stronie internetowej.

Aplikacje webowe w Tomcacie są zwykle pakowane w pliki WAR (Web Application Archive), które zawierają pliki klas servletów, pliki JSP, biblioteki i inne zasoby. Po zainstalowaniu pliku WAR na serwerze Tomcat, aplikacja jest gotowa do uruchomienia.

Tomcat składa się z kilku modułów, które są odpowiedzialne za różne funkcje, takie jak przetwarzanie żądań HTTP, obsługę sesji, logowanie i bezpieczeństwo. Tomcat umożliwia również konfigurację wielu parametrów, takich jak porty nasłuchu, rozmiar puli wątków, poziom logowania i wiele innych.

Tomcat jest często wykorzystywany jako serwer aplikacji dla aplikacji webowych napisanych w języku Java. Dzięki swojej prostocie i elastyczności, Tomcat jest popularnym wyborem dla wielu projektów.


## 21.10. BigBlueButton

BigBlueButton to oprogramowanie typu open-source, służące do organizowania internetowych spotkań i konferencji online. Głównym celem BigBlueButton jest umożliwienie użytkownikom prowadzenia interaktywnych sesji edukacyjnych, prezentacji i warsztatów w czasie rzeczywistym.

BigBlueButton składa się z kilku modułów, które są odpowiedzialne za różne funkcje. Na przykład moduł prezentacji umożliwia prowadzącemu wyświetlanie slajdów, materiałów edukacyjnych i wideo. Moduł czatu pozwala na prowadzenie interakcji między uczestnikami spotkania, podczas gdy moduł kamery internetowej umożliwia uczestnikom udział w spotkaniu wideo. BigBlueButton umożliwia również udostępnianie plików i ekranu, a także zapisywanie nagrania całego spotkania.

BigBlueButton jest oparty na technologii WebRTC, co oznacza, że użytkownicy mogą korzystać z oprogramowania bez konieczności instalowania dodatkowych programów czy wtyczek. Dzięki temu BigBlueButton jest łatwy w użyciu i dostępny dla użytkowników z różnych platform i urządzeń.

BigBlueButton umożliwia także integrację z innymi systemami i narzędziami, takimi jak Moodle, Canvas, WordPress czy Slack. Istnieje również wiele wtyczek i rozszerzeń dostępnych dla BigBlueButton, które umożliwiają dostosowanie oprogramowania do indywidualnych potrzeb użytkowników.

Ze względu na swoją prostotę i elastyczność, BigBlueButton stał się popularnym narzędziem dla edukacji na odległość, szkoleń online i innych spotkań wirtualnych.


## 21.11. WebRTC

WebRTC (Web Real-Time Communication) to otwarty standard webowy, który umożliwia komunikację w czasie rzeczywistym między przeglądarkami internetowymi, bez konieczności instalowania dodatkowych wtyczek lub programów. WebRTC jest dostępny dla użytkowników różnych platform i urządzeń, w tym na komputerach, tabletach i smartfonach.

WebRTC pozwala na przesyłanie strumieni audio i wideo oraz przesyłanie danych w czasie rzeczywistym między przeglądarkami. Standard ten opiera się na technologii peer-to-peer (P2P), co oznacza, że dane są przesyłane bezpośrednio między urządzeniami użytkowników, bez pośrednictwa serwerów. Dzięki temu WebRTC umożliwia szybką i efektywną komunikację.

WebRTC wykorzystuje wiele technologii, w tym kodeki audio i wideo, protokoły transportowe, protokoły szyfrowania i zarządzanie sesją. WebRTC jest również zintegrowany z innymi standardami webowymi, takimi jak HTML5 i JavaScript, co umożliwia deweloperom tworzenie zaawansowanych aplikacji internetowych z interaktywnymi funkcjami komunikacyjnymi.

WebRTC jest często wykorzystywany w aplikacjach takich jak wideo-konferencje, czaty wideo, gry wieloosobowe oraz aplikacje do zdalnej pomocy technicznej. Standard ten jest również wykorzystywany w innych zastosowaniach, takich jak streamowanie muzyki i filmów oraz wideo na żywo na platformach społecznościowych.

<p align="center">
Rys. 21.11.1. Działanie WebRTC
<br>
  <img src="\assets\img\Sieci\66.png" width="650" alt="WebRTC">
</p>


# 22. Kryptografia

Kryptografia to nauka zajmująca się bezpiecznym przesyłaniem informacji, a także chronieniem danych przed nieuprawnionym dostępem i modyfikacją. Jest to kluczowy element dzisiejszych systemów informatycznych i sieci komputerowych.

Istnieją różne metody kryptografii, ale można je podzielić na dwie główne kategorie: symetryczne i asymetryczne.

W *kryptografii symetrycznej* używa się jednego klucza, który jest używany zarówno do szyfrowania, jak i deszyfrowania danych. Jest to prostszy i szybszy sposób szyfrowania danych, ale wymaga bezpiecznego sposobu przekazywania klucza do odbiorcy.

<p align="center">
Rys. 22.1. Kryptografia
<br>
  <img src="\assets\img\Sieci\67.png" width="650" alt="Kryptografia">
</p>

Przykładem algorytmu kryptograficznego wykorzystującego kryptografię symetryczną jest AES (Advanced Encryption Standard), który jest powszechnie stosowany w zabezpieczaniu danych w systemach informatycznych.

Istnieją trzy podstawowe etapy procesu szyfrowania i deszyfrowania danych w kryptografii symetrycznej:
+ Generowanie klucza - klucz symetryczny musi być wygenerowany przed rozpoczęciem procesu szyfrowania i deszyfrowania danych. Ten sam klucz musi być znany zarówno przez nadawcę, jak i odbiorcę.
+ Szyfrowanie - dane są szyfrowane za pomocą klucza symetrycznego. Algorytm szyfrowania przekształca oryginalną wiadomość w zaszyfrowaną wersję, która jest niemożliwa do odczytania bez posiadania klucza.
+ Deszyfrowanie - odbiorca używa tego samego klucza symetrycznego, aby odszyfrować zaszyfrowaną wiadomość na oryginalną wersję.

Kryptografia symetryczna jest stosunkowo prosta i szybka w użyciu, ale wymaga bezpiecznego sposobu przekazywania klucza między nadawcą a odbiorcą. Bezpieczeństwo algorytmu zależy w dużej mierze od bezpieczeństwa klucza. Jeśli klucz zostanie przechwycony przez nieuprawnioną osobę, będzie ona w stanie odczytać zaszyfrowane dane. Dlatego klucz symetryczny powinien być przechowywany w bezpiecznym miejscu i przesyłany w sposób bezpieczny.

W kryptografii asymetrycznej używa się dwóch kluczy: publicznego i prywatnego. Klucz publiczny jest dostępny dla każdego, a klucz prywatny jest tajny i znany tylko właścicielowi. Dane są szyfrowane kluczem publicznym i mogą być odszyfrowane tylko za pomocą klucza prywatnego. Jest to bardziej bezpieczny sposób szyfrowania danych, ale jest też wolniejszy i bardziej złożony.

Klucz publiczny udostępniany jest każdej osobie która chce zaszyfrować wiadomość. Deszyfrowanie wiadomości możliwe jest wyłącznie z wykorzystaniem klucza prywatnego, który powinien być pilnie strzeżony.

Obliczenie klucza prywatnego na podstawie klucza publicznego powinno być matematycznie trudne. W przeciwnym razie opublikowany klucz publiczny pozwalałby na łatwe uzyskanie klucza prywatnego, a co za tym idzie deszyfrowanie wiadomości.

<p align="center">
Rys. 22.2. Kryptografia
<br>
  <img src="\assets\img\Sieci\68.png" width="650" alt="Kryptografia-1">
</p>

Inne metody kryptografii to m.in. haszowanie, które pozwala na szybkie i łatwe sprawdzanie, czy dana wiadomość została zmodyfikowana, ale nie pozwala na jej odszyfrowanie. 

<p align="center">
Rys. 22.3. Jak działa algorytm haszujący
<br>
  <img src="\assets\img\Sieci\69.png" width="650" alt="Kryptografia-2">
</p>

Kryptografia haszowania, nazywana również kryptografią jednokierunkową, to proces przetwarzania danych w taki sposób, że trudno jest odwrócić proces i odzyskać oryginalne dane. W tym procesie, z oryginalnego tekstu (nazywanego tekstem jawnym) generowany jest skrót wiadomości (hash), który jest reprezentowany przez ciąg znaków o stałej długości. Skrót ten jest zwykle znacznie krótszy niż oryginalna wiadomość.

Skrót wiadomości jest generowany przez algorytm haszowania, który przetwarza dane wejściowe i generuje wartość wyjściową o stałej długości. Algorytmy haszowania są projektowane w taki sposób, aby generować różne skróty dla różnych wiadomości, ale także aby był to proces jednokierunkowy, czyli niemożliwy do odwrócenia.

Jednym z najbardziej popularnych algorytmów haszowania jest SHA (Secure Hash Algorithm), który jest stosowany w wielu zastosowaniach, takich jak weryfikacja integralności plików, uwierzytelnianie haseł, identyfikacja oprogramowania antywirusowego i wiele innych.

Skrót wiadomości może być używany do weryfikacji integralności wiadomości. W celu sprawdzenia, czy wiadomość nie została zmodyfikowana w trakcie transmisji, nadawca może obliczyć skrót wiadomości przed jej wysłaniem i porównać go z skrótem wiadomości, który jest obliczany przez odbiorcę po jej otrzymaniu. Jeśli skróty się nie zgadzają, wiadomość została zmodyfikowana w trakcie transmisji.

Jednym z ograniczeń kryptografii haszowania jest to, że skrót wiadomości nie może być odszyfrowany na oryginalną wiadomość. Z tego powodu kryptografia haszowania jest stosowana głównie do weryfikacji integralności wiadomości, a nie do bezpiecznego przesyłania poufnych informacji.

Istnieją także protokoły kryptograficzne, takie jak SSL/TLS, które pozwalają na bezpieczną komunikację między serwerami i klientami w sieciach komputerowych.

Kryptografia jest stosowana w wielu dziedzinach, takich jak finanse, medycyna, bezpieczeństwo państwowe, handel elektroniczny i wiele innych. Bez kryptografii wiele dzisiejszych systemów informatycznych byłoby narażonych na ataki hakerów i włamywaczy.


# 23. Metodologie i frameworki

Metodologie i frameworki to narzędzia, które pomagają w zarządzaniu projektami informatycznymi oraz w wdrażaniu i utrzymywaniu systemów informatycznych. Są to zbiory najlepszych praktyk, procesów, procedur i narzędzi, które mają na celu usprawnienie procesów projektowych, zmniejszenie ryzyka oraz zwiększenie efektywności i jakości projektów.

Wszystkie te narzędzia mają na celu usprawnienie procesów projektowych oraz zwiększenie efektywności i jakości projektów. Wybór odpowiedniej metodyki lub frameworka zależy od charakteru projektu, branży oraz wymagań biznesowych.


## 23.1. Cykl życia rozwoju zabezpieczeń SDL (Security Development Lifecycle SDL)

Cykl życia rozwoju zabezpieczeń (Security Development Lifecycle - SDL) to proces projektowania i wdrażania oprogramowania, który uwzględnia aspekty bezpieczeństwa już na etapie tworzenia aplikacji. Zapewnia to zwiększenie odporności aplikacji na ataki i minimalizację ryzyka wystąpienia luk w zabezpieczeniach.

<p align="center">
Rys. 23.1.1. Cykl życia rozwoju zabezpieczeń SDL
<br>
  <img src="\assets\img\Sieci\70.png" width="650" alt="SDL">
</p>

Cykl życia rozwoju zabezpieczeń SDL składa się z kilku etapów:
+ Planowanie - w tym etapie definiowane są cele i wymagania dotyczące bezpieczeństwa, a także przeprowadzane są analizy zagrożeń oraz identyfikowane są obszary wymagające szczególnej ochrony.
+ Projektowanie - na tym etapie projektowane są mechanizmy zabezpieczeń, w tym procesy uwierzytelniania, autoryzacji i szyfrowania.
+ Implementacja - w tym etapie tworzony jest kod programu, który uwzględnia wcześniej zdefiniowane wymagania bezpieczeństwa.
+ Testowanie - na tym etapie przeprowadzane są różnego rodzaju testy, które mają na celu wykrycie błędów w implementacji zabezpieczeń.
+ Wdrożenie - po przeprowadzeniu testów aplikacja jest gotowa do wdrożenia.
+ Monitorowanie - po wdrożeniu aplikacji przeprowadzane są regularne audyty bezpieczeństwa, które mają na celu wykrycie ewentualnych luk w zabezpieczeniach.

W ramach cyklu życia rozwoju zabezpieczeń SDL stosuje się różne narzędzia i metody, takie jak:
+ kody źródłowe kontrolne, które pozwalają na wykrycie błędów w kodzie przed jego wdrożeniem;
+ testy penetracyjne, które polegają na próbie zdobycia nieautoryzowanego dostępu do systemu;
+ testy bezpieczeństwa aplikacji, które pozwalają na sprawdzenie zgodności z wymaganiami bezpieczeństwa.

Cykl życia rozwoju zabezpieczeń SDL stanowi ważny element w budowaniu bezpiecznych aplikacji i systemów informatycznych. Pozwala na minimalizację ryzyka wystąpienia luk w zabezpieczeniach i zwiększenie odporności na ataki.


## 23.2. OWASP Top Ten

OWASP Top Ten to lista dziesięciu najważniejszych zagrożeń bezpieczeństwa aplikacji internetowych, opracowana przez organizację Open Web Application Security Project (OWASP). Lista ta stanowi podstawowy punkt odniesienia dla firm i organizacji, które zajmują się wdrażaniem aplikacji internetowych i chcą zabezpieczyć swoje systemy przed atakami.

<p align="center">
Rys. 23.2.1 OWASP Top Ten 
<br>
  <img src="\assets\img\Sieci\71.png" width="650" alt="OWASP">
</p>


Poniżej przedstawione są poszczególne zagrożenia uwzględnione na liście OWASP Top Ten:
+ Wstrzyknięcia SQL (SQL Injection) – ataki polegające na wprowadzeniu nieodpowiednich danych do formularzy internetowych lub zapytań SQL, co pozwala na przejęcie kontroli nad aplikacją i uzyskanie dostępu do wrażliwych informacji.
+ Niepoprawna autoryzacja i uwierzytelnianie (Broken Authentication and Session Management) – zagrożenie polegające na słabej ochronie systemów autoryzacji i uwierzytelniania, co pozwala na przejęcie kontroli nad kontami użytkowników.
+ Cross-Site Scripting (XSS) – ataki polegające na wprowadzeniu kodu JavaScript do aplikacji internetowej, co pozwala na przechwycenie danych użytkownika lub przejęcie kontroli nad aplikacją.
+ Narażenie na niebezpieczeństwo poufności (Sensitive Data Exposure) – zagrożenie polegające na niedostatecznej ochronie wrażliwych danych użytkowników, takich jak hasła, numery kart kredytowych czy informacje personalne.
+ Niepoprawne ustawienia bezpieczeństwa (Security Misconfiguration) – zagrożenie polegające na błędnej konfiguracji aplikacji internetowej, co pozwala na łatwe ataki hackerów.
+ Używanie komponentów z podatnościami (Using Components with Known Vulnerabilities) – zagrożenie polegające na używaniu komponentów, które są znane z podatności na ataki hackerów.
+ Nieprawidłowe przetwarzanie danych wejściowych (Insufficient Input Validation) – zagrożenie polegające na niewłaściwym przetwarzaniu danych wejściowych, co pozwala na wprowadzenie do systemu niebezpiecznych danych.
+ Nieuprawnione operacje na kontach (Broken Access Control) – zagrożenie polegające na braku kontroli dostępu do danych użytkowników i możliwości wykonania nieuprawnionych operacji na ich kontach.
+ Brak monitorowania i reagowania na ataki (Insufficient Logging and Monitoring) – zagrożenie polegające na niedostatecznym monitorowaniu systemu, co pozwala na łatwe ataki hackerów.
+ Nieodpowiednia ochrona przed atakami z wykorzystaniem sieci (Insecure Network Architecture) – nieprawidłowa konfiguracja zabezpieczeń aplikacji oznacza błędne ustawienia aplikacji, które pozwalają na łatwiejsze jej zhakowanie lub umożliwiają atakującemu na dostęp do poufnych informacji. Przykładami nieprawidłowej konfiguracji mogą być np. pozostawienie domyślnych haseł, niedostateczna weryfikacja uprawnień użytkowników, brak szyfrowania transmisji danych czy niewłaściwe skonfigurowanie pamięci podręcznej. 


## 23.3. Ramy bezpieczeństwa cybernetycznego NIST

NIST (National Institute of Standards and Technology) to agencja rządu USA, która zajmuje się m.in. standardami technologicznymi i kwestiami związanymi z bezpieczeństwem. NIST udostępnia wiele ram bezpieczeństwa cybernetycznego, które mogą pomóc organizacjom w zabezpieczeniu swoich systemów informatycznych.

<p align="center">
Rys. 23.3.1. Ramy bezpieczeństwa cybernetycznego NIST
<br>
  <img src="\assets\img\Sieci\72.png" width="650" alt="NIST">
</p>

Najważniejsze ramy bezpieczeństwa cybernetycznego NIST to:
+ Cybersecurity Framework (CSF) - jest to ramowy dokument opracowany przez NIST, który pomaga organizacjom w tworzeniu i wdrażaniu programów bezpieczeństwa cybernetycznego. Składa się z pięciu elementów: identyfikacji, ochrony, wykrywania, reagowania i naprawy.
+ NIST SP 800-53 - jest to standard bezpieczeństwa informacji, który zawiera listę kontroli bezpieczeństwa, które powinny być wdrożone w systemach informatycznych. Standard ten określa wymagania dla systemów federalnych w Stanach Zjednoczonych.
+ NIST SP 800-171 - to standard bezpieczeństwa informacji, który określa wymagania dla firm prywatnych, które dostarczają produkty lub usługi dla rządu USA. Wymagania te dotyczą m.in. zarządzania dostępem, szyfrowania, weryfikacji tożsamości i monitorowania systemów informatycznych.
+ NIST Cybersecurity Framework for Improving Critical Infrastructure Cybersecurity (Cybersecurity Framework 2.0) - jest to uaktualniona wersja Cybersecurity Framework, która została wydana w 2018 roku. Zawiera ona nowe zalecenia, które mają pomóc organizacjom w lepszym zabezpieczaniu swoich systemów informatycznych.
+ Privacy Framework - to ramowy dokument NIST, który pomaga organizacjom w zarządzaniu ryzykiem związanym z prywatnością danych. Framework ten składa się z trzech elementów: zarządzania, ochrony i przetwarzania danych osobowych.

Wszystkie te ramy bezpieczeństwa cybernetycznego NIST mają na celu pomóc organizacjom w zabezpieczeniu swoich systemów informatycznych i zapobieganiu cyberataków.


## 23.4. Kontrole CIS

Implementation Groups (IGs) są zalecanymi wytycznymi w zakresie ustalania priorytetów wdrażania krytycznych kontroli bezpieczeństwa CIS (CIS Controls). Aby pomóc przedsiębiorstwom każdej wielkości, IGs dzielą się na trzy grupy. Opierają się one na profilu ryzyka i zasobach, którymi przedsiębiorstwo dysponuje w celu wdrożenia CIS Controls.

Każdy IG identyfikuje zestaw zabezpieczeń, które musi wdrożyć. W CIS Controls v8 dostępne są łącznie 153 zabezpieczenia.

<p align="center">
Rys. 23.4.1. Kontrole CIS
<br>
  <img src="\assets\img\Sieci\73.png" width="650" alt="CIS">
</p>

CIS Controls v8 definiuje grupę wdrożeniową 1 (IG1) jako niezbędną higienę cybernetyczną i reprezentuje wyłaniający się minimalny standard bezpieczeństwa informacji dla wszystkich przedsiębiorstw. IG1 jest wstępem do CIS Controls składa się z podstawowego zestawu 56 Zabezpieczeń cyberobrony. Zabezpieczenia zawarte w IG1 są tym, co każde przedsiębiorstwo powinno stosować w celu obrony przed najczęstszymi atakami.

W większości przypadków przedsiębiorstwa IG1 są zazwyczaj małymi lub średnimi przedsiębiorstwami z ograniczoną wiedzą w zakresie IT i bezpieczeństwa cybernetycznego, które można poświęcić na ochronę zasobów IT i personelu. Wspólną troską tych przedsiębiorstw jest utrzymanie działalności operacyjnej, ponieważ mają one ograniczoną tolerancję na przestoje.

Wrażliwość danych, które starają się chronić, jest niska i dotyczy głównie informacji pracowniczych i finansowych. Zabezpieczenia wybrane dla IG1 powinny być możliwe do wdrożenia przy ograniczonej wiedzy na temat cyberbezpieczeństwa i mieć na celu udaremnienie ogólnych, nieukierunkowanych ataków. Te zabezpieczenia będą również zwykle zaprojektowane do pracy w połączeniu z gotowym sprzętem i oprogramowaniem dla małych lub domowych biur.

<p align="center">
Rys. 23.4.2. Kontrole CIS
<br>
  <img src="\assets\img\Sieci\74.png" width="650" alt="CIS-1">
</p>

IG2 składa się z 74 dodatkowych Zabezpieczeń i opiera się na 56 Zabezpieczeniach określonych w IG1.

74 Zabezpieczenia wybrane dla IG2 mogą pomóc zespołom ds. bezpieczeństwa radzić sobie ze zwiększoną złożonością operacyjną. Prawidłowa instalacja i konfiguracja niektórych Zabezpieczeń będzie zależeć od technologii klasy korporacyjnej i specjalistycznej wiedzy specjalistycznej.

Przedsiębiorstwo IG2 zatrudnia osoby odpowiedzialne za zarządzanie i ochronę infrastruktury IT. Przedsiębiorstwa te zazwyczaj obsługują wiele działów o różnych profilach ryzyka w zależności od funkcji stanowiska i misji. Jednostki małych przedsiębiorstw mogą mieć obciążenia związane z przestrzeganiem przepisów. Przedsiębiorstwa IG2 często przechowują i przetwarzają poufne informacje o klientach lub przedsiębiorstwach i są w stanie wytrzymać krótkie przerwy w świadczeniu usług. Głównym problemem jest utrata zaufania publicznego w przypadku naruszenia.

<p align="center">
Rys. 23.4.3. Kontrole CIS
<br>
  <img src="\assets\img\Sieci\75.png" width="650" alt="CIS-2">
</p>

IG3 składa się z dodatkowych 23 Zabezpieczeń. Opiera się na zabezpieczeniach określonych w IG1 (56) i IG2 (74), w sumie 153 zabezpieczeniach w CIS Controls v8.

Przedsiębiorstwo IG3 zwykle zatrudnia ekspertów ds. bezpieczeństwa, którzy specjalizują się w różnych aspektach cyberbezpieczeństwa (np. zarządzanie ryzykiem, testy penetracyjne, bezpieczeństwo aplikacji). Aktywa i dane IG3 zawierają poufne informacje lub funkcje, które podlegają nadzorowi regulacyjnemu i zgodności. Przedsiębiorstwo IG3 musi zająć się dostępnością usług oraz poufnością i integralnością wrażliwych danych. Udane ataki mogą spowodować znaczne szkody dla dobra publicznego.

Zabezpieczenia wybrane dla IG3 muszą ograniczać ukierunkowane ataki wyrafinowanego przeciwnika i zmniejszać wpływ ataków typu zero-day.


# 24. Architektura bezpieczeństwa

Architektura bezpieczeństwa to strategiczne podejście do projektowania, implementacji i zarządzania zabezpieczeniami informacji w organizacji. Obejmuje ona procesy, narzędzia, protokoły i praktyki, które mają na celu ochronę zasobów informacyjnych przed zagrożeniami związanymi z cyberbezpieczeństwem.

Architektura bezpieczeństwa pomaga organizacjom w zapewnieniu skutecznego zarządzania ryzykiem związanym z cyberbezpieczeństwem oraz w zapewnieniu integralności, poufności i dostępności informacji w organizacji.


## 24.1. Obrona w głębi (Defense in Depth)

Obrona w głębi (ang. Defense in Depth) to podejście do bezpieczeństwa informatycznego, które polega na tworzeniu wielu warstw zabezpieczeń, aby zminimalizować ryzyko naruszenia bezpieczeństwa w przypadku, gdy jedna z warstw zostanie naruszona lub usunięta.

Obrona w głębi polega na tym, aby tworzyć kilka niezależnych warstw zabezpieczeń, które chronią system przed różnego rodzaju zagrożeniami, takimi jak ataki hakerskie, wirusy czy ataki fizyczne. Każda warstwa powinna mieć unikalne funkcje i cechy, które są przeznaczone do obrony przed określonymi rodzajami zagrożeń.

<p align="center">
Rys. 24.1.1. Defense in Depth
<br>
  <img src="\assets\img\Sieci\76.png" width="650" alt="DiD">
</p>

Przykłady warstw zabezpieczeń w ramach obrony w głębi to:
+ Zabezpieczenia fizyczne - systemy alarmowe, kamery monitoringu, kontrola dostępu do pomieszczeń itp.
+ Zabezpieczenia sieciowe - zaporę ogniową, antywirusy, filtry treści, systemy wykrywania i zapobiegania włamaniom (IDS/IPS) itp.
+ Zabezpieczenia aplikacji - autoryzacja użytkowników, szyfrowanie danych, testy penetracyjne, weryfikacja kodu źródłowego itp.
+ Zabezpieczenia danych - kopie zapasowe, szyfrowanie danych, systemy kontroli dostępu itp.
+ Zabezpieczenia użytkowników - szkolenia z zakresu bezpieczeństwa, polityki bezpieczeństwa, autoryzacja użytkowników, hasła itp.

W przypadku, gdy jedna z warstw zostanie naruszona, pozostałe warstwy zabezpieczeń powinny działać w celu zminimalizowania szkód i zapewnienia ciągłości działania systemu. Obrona w głębi jest szczególnie ważna w przypadku systemów o wysokim poziomie krytyczności, takich jak systemy bankowe, medyczne czy wojskowe, ale może być stosowana w każdym rodzaju systemu informatycznego.

## 24.2. Architektura zerowego zaufania (Zero Trust Architecture)

Architektura zerowego zaufania (Zero Trust Architecture) to podejście do bezpieczeństwa sieciowego, w którym każde połączenie i żądanie jest traktowane jako potencjalne zagrożenie. W tym modelu nie ma założenia, że urządzenia i użytkownicy są już bezpieczni, zamiast tego wymaga się od nich ciągłej autentykacji i weryfikacji uprawnień w czasie rzeczywistym.

<p align="center">
Rys. 24.2.1. Zero Trust Architecture
<br>
  <img src="\assets\img\Sieci\77.png" width="650" alt="ZTA">
</p>

W architekturze zerowego zaufania stosuje się kilka podstawowych zasad, takich jak:
+ Identyfikacja i autoryzacja użytkowników i urządzeń na każdym etapie sieci, nie tylko przy dostępie do systemów zewnętrznych.
+ Kontrola dostępu na poziomie aplikacji i danych, a nie tylko sieci, w celu zapobiegania ruchowi niepożądanego ruchu sieciowego.
+ Wdrożenie zaawansowanych technologii zabezpieczeń, takich jak sieci prywatne wirtualne (VPN), uwierzytelnianie wieloskładnikowe (MFA), izolacja aplikacji (sandboxing) i analiza ruchu sieciowego w czasie rzeczywistym.
+ Utrzymywanie i aktualizowanie systemów zabezpieczeń w celu zapewnienia ciągłej ochrony przed nowymi zagrożeniami.

Architektura zerowego zaufania jest szczególnie przydatna w przypadku firm i organizacji, które korzystają z chmury publicznej lub mają rozproszone środowisko IT. Zapewnia ona większą kontrolę nad ruchem sieciowym i lepszą ochronę przed atakami hakerskimi.


## 24.3. Architektura bezpieczeństwa w chmurze (Cloud Security Architecture)

Architektura bezpieczeństwa w chmurze (Cloud Security Architecture) to sposób projektowania i implementacji rozwiązań bezpieczeństwa dla systemów i usług chmurowych. Obejmuje ona zarówno prywatne chmury, jak i chmury publiczne.

Celem architektury bezpieczeństwa w chmurze jest zapewnienie ochrony danych, aplikacji i infrastruktury w chmurze poprzez zastosowanie odpowiednich mechanizmów bezpieczeństwa, takich jak autentykacja, autoryzacja, szyfrowanie, zarządzanie kluczami, zarządzanie tożsamością i dostępem, wirtualne sieci prywatne (VPN), zapory sieciowe, monitorowanie zdarzeń i audytowanie.

Architektura bezpieczeństwa w chmurze składa się z kilku warstw, w tym warstwy infrastruktury, platformy, aplikacji i danych. Każda warstwa wymaga odpowiednich mechanizmów bezpieczeństwa i kontroli dostępu.

<p align="center">
Rys. 24.3.1. Cloud Security Architecture
<br>
  <img src="\assets\img\Sieci\78.png" width="650" alt="CSA">
</p>

Ważnym elementem architektury bezpieczeństwa w chmurze jest również monitorowanie i zarządzanie bezpieczeństwem. W tym celu stosuje się różne narzędzia i usługi, takie jak systemy monitorowania zdarzeń (SIEM), usługi zarządzania zabezpieczeniami (MSS), narzędzia analizy zagrożeń i oprogramowanie zarządzania politykami bezpieczeństwa.

Dobrze zaprojektowana architektura bezpieczeństwa w chmurze powinna uwzględniać wymagania regulacyjne i zgodność z przepisami dotyczącymi prywatności i bezpieczeństwa danych, takimi jak RODO czy PCI-DSS.


## 24.4. Zarządzanie tożsamością i dostępem IAM (Identity and Access Management IAM)

Zarządzanie tożsamością i dostępem (IAM) to procesy, narzędzia i technologie związane z zarządzaniem cyfrowymi tożsamościami użytkowników, ich uprawnieniami i dostępem do zasobów informatycznych w organizacji. IAM umożliwia administrację użytkownikami, atrybutami, autoryzacją i uwierzytelnieniem, dostępem do systemów, aplikacji i innych zasobów oraz przepływem informacji między nimi.

<p align="center">
Rys. 24.4.1. Identity and Access Management IAM
<br>
  <img src="\assets\img\Sieci\79.png" width="650" alt="IAM">
</p>

W skład IAM wchodzą narzędzia takie jak zarządzanie tożsamością, zarządzanie uprawnieniami, uwierzytelnianie wieloskładnikowe (MFA), jednokrotne uwierzytelnienie (SSO), zarządzanie sesjami, zarządzanie hasłami, zarządzanie certyfikatami i federacja tożsamości. IAM odgrywa kluczową rolę w zapewnieniu bezpieczeństwa w organizacji, a także w spełnieniu wymagań regulacyjnych i zgodności z przepisami, takimi jak GDPR czy HIPAA.


## 24.5. Ochrona danych (Data Protection)

Ochrona danych to kluczowy element bezpieczeństwa informacji i sieci. Chodzi tu o zapewnienie, że dane są bezpieczne, poufne i integralne w czasie ich przetwarzania, przechowywania i przesyłania. Ochrona danych obejmuje różne aspekty, w tym:
+ Szyfrowanie danych - to proces konwertowania danych na postać nieczytelną dla osób trzecich. Szyfrowanie może odbywać się na różnych poziomach, od pliku do dysku twardego lub całej sieci.
+ Kontrola dostępu - to mechanizmy zapewniające, że tylko uprawnione osoby mają dostęp do danych. Kontrola dostępu może obejmować mechanizmy uwierzytelniania, autoryzacji, weryfikacji tożsamości i zarządzania uprawnieniami.
+ Monitorowanie i audytowanie - to procesy śledzenia aktywności użytkowników w systemie, w tym dostępu do danych i operacji na nich. Monitorowanie i audytowanie umożliwiają wykrycie i reagowanie na nieautoryzowane aktywności.
+ Backup i recovery - to proces tworzenia kopii zapasowych danych i przywracania ich w przypadku awarii systemu lub incydentu związanych z bezpieczeństwem. Backup i recovery są kluczowe dla zapewnienia ciągłości biznesowej i minimalizacji ryzyka utraty danych.
+ Zarządzanie informacją - to procesy zarządzania cyklem życia informacji, w tym zbieranie, przetwarzanie, przechowywanie, usuwanie i archiwizowanie danych. Zarządzanie informacją obejmuje również polityki i procedury dotyczące bezpieczeństwa informacji.

<p align="center">
Rys. 24.5.1. Data Protection
<br>
  <img src="\assets\img\Sieci\80.png" width="650" alt="DP">
</p>

Wszystkie te elementy muszą działać wspólnie, aby zapewnić ochronę danych na każdym etapie ich przetwarzania i przesyłania. Bezpieczeństwo danych jest kluczowe dla zapewnienia prywatności, integralności i dostępności informacji, co jest podstawą każdej organizacji.


## 24.6. Planowanie reagowania na incydenty (Incident Responce Planning)

Planowanie reagowania na incydenty (Incident Response Planning) to proces planowania i organizacji działań w przypadku wystąpienia incydentu w bezpieczeństwie informacji. Celem planowania reagowania na incydenty jest szybka reakcja na wykryte zagrożenie oraz minimalizacja skutków incydentu.

Plan reagowania na incydenty powinien zawierać szczegółowe procedury, które określają kto jest odpowiedzialny za podjęcie działań w przypadku wystąpienia incydentu, jakie narzędzia należy wykorzystać, jakie informacje należy zbierać i jakie działania podjąć w celu wyeliminowania zagrożenia. Plan powinien być dokumentowany, przechowywany w bezpiecznym miejscu i regularnie aktualizowany, aby uwzględniać nowe rodzaje zagrożeń i zmiany w infrastrukturze IT.

W ramach planowania reagowania na incydenty należy przeprowadzać regularne ćwiczenia i testy, aby upewnić się, że plan działa poprawnie i umożliwia szybką reakcję na incydenty. Należy także zapewnić szkolenia pracowników, aby zwiększyć ich świadomość w zakresie bezpieczeństwa informacji oraz przygotować ich do działań w przypadku wystąpienia incydentu.

<p align="center">
Rys. 24.6.1. Incident Responce Planning 
<br>
  <img src="\assets\img\Sieci\81.png" width="650" alt="IRP">
</p>

Planowanie reagowania na incydenty jest kluczowe dla zapewnienia bezpieczeństwa informacji w organizacji i minimalizacji skutków incydentów. Dzięki odpowiedniej organizacji i szybkiej reakcji można zminimalizować straty finansowe, utratę wizerunku firmy oraz zagrożenie dla danych klientów i pracowników.


# 25. Narzędzia i technologie bezpieczeństwa

Narzędzia i technologie bezpieczeństwa to zbiór oprogramowania, narzędzi i metodologii, które pomagają zapewnić bezpieczeństwo systemów informatycznych, sieci oraz danych. Istnieje wiele różnych narzędzi i technologii, które służą różnym celom w zakresie bezpieczeństwa, od narzędzi do monitorowania ruchu sieciowego, poprzez programy antywirusowe, po systemy zarządzania tożsamością.

## 25.1. SIEM

SIEM (Security Information and Event Management) to narzędzie i technologia bezpieczeństwa, które pozwala na zbieranie, przetwarzanie, analizowanie i raportowanie informacji dotyczących zdarzeń związanych z bezpieczeństwem w sieciach komputerowych oraz systemach informatycznych.

<p align="center">
Rys. 25.1.1. SIEM
<br>
  <img src="\assets\img\Sieci\82.png" width="650" alt="SIEM">
</p>

Narzędzia SIEM pozwalają na monitorowanie różnego rodzaju zdarzeń związanych z bezpieczeństwem, takich jak próby nieudanych logowań, ataki typu phishing, próby włamania, a także nieprawidłowe lub nieautoryzowane działania na serwerach i systemach. Dane z różnych źródeł, takich jak dzienniki systemowe, narzędzia antywirusowe, systemy detekcji intruzów, są agregowane i przetwarzane w celu wykrycia podejrzanych zdarzeń.

Systemy SIEM zwykle wykorzystują algorytmy uczenia maszynowego i technologie sztucznej inteligencji, aby identyfikować anomalie i potencjalne zagrożenia, a także generować alerty i raporty dla administratorów systemów i zespołów bezpieczeństwa.

<p align="center">
Rys. 25.1.2. Solving security management challenges
<br>
  <img src="\assets\img\Sieci\83.png" width="650" alt="SIEM-1">
</p>

Przykłady narzędzi SIEM to Splunk, ArcSight, QRadar, czy Elastic Stack. SIEM jest kluczowym elementem w dzisiejszych środowiskach sieciowych i systemach informatycznych, ponieważ pozwala na skuteczne wykrywanie i reagowanie na zagrożenia dla bezpieczeństwa w czasie rzeczywistym.


## 25.2. IDS/IPS

IDS (Intrusion Detection System) oraz IPS (Intrusion Prevention System) to narzędzia stosowane w celu wykrywania i zapobiegania nieautoryzowanemu dostępowi do sieci komputerowej lub systemu informatycznego.

<p align="center">
Rys. 25.2.1. Działanie IDS/IPS
<br>
  <img src="\assets\img\Sieci\84.png" width="650" alt="IDS/IPS">
</p>

IDS działa w trybie pasywnym, monitorując ruch sieciowy i analizując go pod kątem zachowań, które mogą wskazywać na próbę ataku lub naruszenia zasad bezpieczeństwa. IDS może wykryć wiele różnych typów ataków, w tym próby skanowania sieci, ataki DDoS, ataki na protokoły sieciowe, próby uwierzytelnienia, a także infekcje złośliwym oprogramowaniem.

IPS działa w trybie aktywnym, w którym dokonuje analizy ruchu sieciowego i podejmuje decyzje o blokowaniu niebezpiecznych działań. IPS wykorzystuje różne techniki, aby zidentyfikować i zablokować niebezpieczne ruchy, w tym filtrację pakietów, wykrywanie anomalii ruchu sieciowego, a także wykrywanie znanych sygnatur ataków.

IDS/IPS są często stosowane wraz z innymi narzędziami bezpieczeństwa, takimi jak firewalle, systemy kontroli dostępu i rozwiązania antywirusowe, aby zapewnić kompleksową ochronę przed atakami na sieci i systemy informatyczne.


## 25.3. WAF

Web Application Firewall (WAF) to narzędzie i technologia bezpieczeństwa, które zapewnia ochronę aplikacji internetowych przed różnymi atakami, takimi jak ataki SQL injection, ataki XSS (Cross-Site Scripting) i inne. WAF działa na poziomie aplikacji i działa jako filtr, blokując żądania, które nie spełniają określonych reguł bezpieczeństwa.

WAF może działać w różnych trybach, takich jak tryb zapobiegania atakom, tryb wykrywania ataków i tryb korekty. W trybie zapobiegania atakom WAF blokuje wszystkie nieautoryzowane żądania i zapytania. W trybie wykrywania ataków WAF pozwala na przepuszczenie żądań, ale rejestruje wszelkie podejrzane aktywności, takie jak próby ataków. W trybie korekty WAF koryguje lub zmienia niebezpieczne elementy w żądaniach przed przekazaniem ich do serwera aplikacji.

<p align="center">
Rys. 25.3.1. Działanie WAF
<br>
  <img src="\assets\img\Sieci\85.png" width="650" alt="WAF">
</p>

WAF może być implementowany jako sprzętowy lub programowy, a także może działać jako usługa w chmurze. WAF może działać w połączeniu z innymi narzędziami i technologiami bezpieczeństwa, takimi jak SIEM (Security Information and Event Management) czy IDS/IPS (Intrusion Detection System / Intrusion Prevention System).


## 25.4. Skanery luk w zabezpieczeniach (Vulnerability Scanners)

Skanery luk w zabezpieczeniach, nazywane również skanerami podatności lub narzędziami do wykrywania podatności, to oprogramowanie wykorzystywane do automatycznego skanowania systemów, aplikacji lub sieci w celu wykrycia ich podatności na ataki.

<p align="center">
Rys. 25.4.1. Vulnerability Scanners
<br>
  <img src="\assets\img\Sieci\86.png" width="650" alt="Vulnerability Scanners">
</p>

Skanery luk w zabezpieczeniach analizują systemy pod kątem znanych podatności, wykorzystując bazy danych z informacjami na temat znanych podatności i metod ich wykorzystania. Następnie generują raporty, w których opisują wykryte podatności i proponują środki zaradcze.

<p align="center">
Rys. 25.4.2. Protect Against Common Security Vulnerabilities
<br>
  <img src="\assets\img\Sieci\87.png" width="650" alt="PACSV">
</p>

Skanery luk w zabezpieczeniach mogą działać w różnych trybach, takich jak:
+ Skanowanie sieci: Skanowanie sieci w celu wykrycia podatności na różnych urządzeniach, takich jak routery, przełączniki, serwery i inne.
+ Skanowanie hostów: Skanowanie pojedynczych hostów, takich jak serwery, w celu wykrycia podatności na poziomie aplikacji lub systemu operacyjnego.
+ Skanowanie aplikacji: Skanowanie aplikacji internetowych w celu wykrycia podatności, takich jak SQL injection, Cross-Site Scripting (XSS) lub podatności związane z uwierzytelnianiem i autoryzacją.
+ Skanowanie kodu źródłowego: Skanowanie kodu źródłowego aplikacji w celu wykrycia podatności i innych błędów programistycznych.
+ Skanery luk w zabezpieczeniach są narzędziem pomocnym w zwiększaniu bezpieczeństwa systemów i aplikacji. Jednakże, ze względu na fakt, że skanery mogą przegapić niektóre podatności lub wygenerować fałszywie pozytywne wyniki, powinny być one stosowane w połączeniu z innymi narzędziami i metodami testowania bezpieczeństwa, takimi jak testy penetracyjne czy audyty bezpieczeństwa.


## 25.5. Narzędzia do testów penetracyjnych

Narzędzia do testów penetracyjnych to specjalne oprogramowanie służące do testowania bezpieczeństwa systemów informatycznych poprzez symulowanie ataków hakerów i innych cyberprzestępców. Ich celem jest wykrycie i wykorzystanie słabości systemów w celu przetestowania ich odporności na ataki oraz wykrycia luk, które mogą prowadzić do naruszenia bezpieczeństwa i wycieku danych.

<p align="center">
Rys. 25.5.1. Działanie testów penetracyjnych
<br>
  <img src="\assets\img\Sieci\88.png" width="650" alt="Testy">
</p>

Przykłady popularnych narzędzi do testów penetracyjnych to:
+ Metasploit – jedno z najpopularniejszych narzędzi do testowania penetracyjnego, umożliwiające wykonywanie zaawansowanych testów i ataków na różne warstwy systemów;
+ Nmap – skaner sieciowy służący do wykrywania hostów i otwartych portów w sieci, wykorzystywany także do testów penetracyjnych;
+ Burp Suite – narzędzie do testów penetracyjnych aplikacji webowych, pozwalające na wykrywanie słabości w konfiguracji serwera, filtrowanie żądań i odpowiedzi, a także ataki na protokoły HTTP;
+ Aircrack-ng – narzędzie do testowania penetracyjnego sieci bezprzewodowych, pozwalające na złamanie haseł szyfrowanych protokołem WEP i WPA.

<p align="center">
Rys. 25.5.2. Narzędzia testów penetracyjnych 
<br>
  <img src="\assets\img\Sieci\89.png" width="650" alt="Testy-1">
</p>

Jest także wiele innych narzędzi dostępnych na rynku, a ich wybór zależy od potrzeb i specyfiki testowanego systemu czy aplikacji. Warto jednak pamiętać, że testy penetracyjne powinny być przeprowadzane przez doświadczonych specjalistów z odpowiednimi uprawnieniami i w ramach odpowiednich procedur, aby uniknąć naruszenia bezpieczeństwa i wycieku danych.


## 25.6. Rozwiązania w zakresie bezpieczeństwa punktów końcowych (Endpoint Security Solutions)

Rozwiązania w zakresie bezpieczeństwa punktów końcowych (Endpoint Security Solutions) to technologie i narzędzia, które służą do ochrony urządzeń końcowych, takich jak komputery, smartfony, tablety czy drukarki, przed różnego rodzaju zagrożeniami związanymi z cyberprzestępczością.

<p align="center">
Rys. 25.6.1. Endpoint Security Solutions
<br>
  <img src="\assets\img\Sieci\90.png" width="650" alt="ESS">
</p>

W skład takich rozwiązań wchodzą między innymi antywirusy, firewalle osobiste, programy antyspyware, oprogramowanie do ochrony przed phishingiem, narzędzia do wykrywania i blokowania szkodliwych programów oraz programy do monitorowania aktywności użytkowników.

<p align="center">
Rys. 25.6.2. Jak Endpoint Bezpieczeństwa działa
<br>
  <img src="\assets\img\Sieci\91.png" width="650" alt="ES">
</p>

Endpoint Security Solutions wykorzystują wiele technologii, takich jak machine learning, sztuczna inteligencja, heurystyka i behavioral analysis, aby wykrywać nowe zagrożenia oraz chronić przed atakami na bazie już istniejących exploitów.

Dzięki rozwiązaniom w zakresie bezpieczeństwa punktów końcowych, organizacje mogą zabezpieczyć swoje sieci przed różnymi rodzajami zagrożeń, takimi jak wirusy, trojany, ransomware, phishing czy keylogger. W ten sposób minimalizują ryzyko ataków i kradzieży danych, a także zwiększają ogólny poziom bezpieczeństwa swoich systemów.

## 25.7. Zapobieganie utracie danych DLP (Data Loss Prevention)

Rozwiązania w zakresie zapobiegania utracie danych, zwane także rozwiązaniami Data Loss Prevention (DLP), to narzędzia i technologie, które pozwalają na wykrywanie, monitorowanie, kontrolowanie i blokowanie przepływu danych z wewnętrznych źródeł organizacji. Celem DLP jest ochrona poufnych informacji, takich jak dane klientów, dokumenty wewnętrzne, wrażliwe informacje finansowe i dane związane z własnością intelektualną.

<p align="center">
Rys. 25.7.1. Data Loss Prevention
<br>
  <img src="\assets\img\Sieci\92.png" width="650" alt="ES">
</p>

DLP jest stosowany w organizacjach, aby zapobiegać wyciekom danych, a także w celu zapewnienia zgodności z regulacjami dotyczącymi prywatności i bezpieczeństwa danych, takimi jak RODO czy HIPAA. W ramach systemów DLP stosuje się szereg narzędzi, takich jak:
+ Skanery wrażliwych danych - narzędzia te skanują systemy, sieci i urządzenia w poszukiwaniu wrażliwych danych, takich jak numery kart kredytowych, dane osobowe czy hasła.
+ Systemy monitorujące ruch sieciowy - narzędzia te analizują ruch sieciowy w poszukiwaniu nieautoryzowanych przepływów danych, takich jak próby wysyłania wrażliwych danych na zewnątrz organizacji.
+ Systemy kontroli dostępu - narzędzia te kontrolują dostęp do wrażliwych danych wewnątrz organizacji i pozwalają na określenie, kto ma dostęp do danych i w jakim celu.
+ Systemy kryptograficzne - narzędzia te pozwalają na zaszyfrowanie wrażliwych danych, co zapewnia dodatkową warstwę ochrony przed wyciekiem danych.
+ Systemy zarządzania politykami bezpieczeństwa - narzędzia te pozwalają na określenie i zarządzanie politykami bezpieczeństwa w organizacji, takimi jak polityki dotyczące korzystania z internetu czy korzystania z prywatnych urządzeń w miejscu pracy.

<p align="center">
Rys. 25.7.3. Działanie Data Loss Prevention
<br>
  <img src="\assets\img\Sieci\93.png" width="650" alt="ES-1">
</p>

DLP wymaga odpowiedniego wdrożenia i konfiguracji, aby działał skutecznie i nie wpłynął negatywnie na normalne działanie organizacji. Wymaga także ścisłej współpracy między działami IT, bezpieczeństwa i zarządzania organizacją.

# 26. Operacje związane z cyberbezpieczeństwem

Operacje związane z cyberbezpieczeństwem (Cyber Security Operations) to kompleksowe podejście do zarządzania zagrożeniami związanymi z cyberbezpieczeństwem. Celem tych operacji jest ochrona sieci i systemów przed atakami oraz szybka reakcja w przypadku naruszenia bezpieczeństwa. Operacje związane z cyberbezpieczeństwem obejmują wiele działań, w tym:
+ Monitoring i analiza zdarzeń bezpieczeństwa - monitorowanie sieci i systemów w celu wykrycia nieprawidłowości, a następnie analizowanie zgromadzonych danych w celu oceny zagrożeń.
+ Reagowanie na incydenty - szybka reakcja na wykryte incydenty, aby zminimalizować skutki i przywrócić normalne funkcjonowanie systemów.
+ Zarządzanie zdarzeniami bezpieczeństwa - dokumentowanie i śledzenie wszystkich zdarzeń bezpieczeństwa w celu zapewnienia ciągłości działań i udokumentowania działań podejmowanych w przypadku naruszeń bezpieczeństwa.
+ Analiza ryzyka - ocena ryzyka związanego z cyberbezpieczeństwem oraz opracowanie planów zarządzania ryzykiem.
+ Zarządzanie dostępem - kontrola dostępu do sieci i systemów, zarządzanie kontami użytkowników i uprawnieniami.
+ Testy penetracyjne - testowanie systemów i sieci w celu identyfikacji słabości i zapewnienia skuteczności zabezpieczeń.
+ Wdrażanie i zarządzanie zabezpieczeniami - wdrożenie i zarządzanie rozwiązaniami zabezpieczającymi, takimi jak firewall, SIEM, IDS/IPS, WAF itp.
+ Szkolenia i świadomość użytkowników - edukacja użytkowników w zakresie bezpiecznego korzystania z systemów informatycznych i identyfikacja zagrożeń związanych z cyberbezpieczeństwem.

Operacje związane z cyberbezpieczeństwem są kluczowe dla zapewnienia bezpieczeństwa sieci i systemów informatycznych w organizacjach.


# 26.1. Centrum operacyjne bezpieczeństwa SOC (Security Operations Center)

Security Operations Center (SOC) to zaawansowane centrum operacyjne, które odpowiada za monitorowanie, wykrywanie, analizowanie i reagowanie na zagrożenia dla bezpieczeństwa informatycznego. SOC ma na celu chronienie organizacji przed zagrożeniami, które mogą prowadzić do naruszenia bezpieczeństwa danych, a także zapewnienie ciągłości działania usług informatycznych.

<p align="center">
Rys. 26.1.1. SOC
<br>
  <img src="\assets\img\Sieci\94.png" width="650" alt="SOC">
</p>

SOC zazwyczaj składa się z wysoko wykwalifikowanych specjalistów, którzy pracują w kilku różnych obszarach, takich jak monitorowanie zdarzeń (security monitoring), zarządzanie incydentami (incident management), analiza zagrożeń (threat intelligence), badanie zdarzeń (incident investigation), zarządzanie identyfikacją i dostępem (identity and access management), zarządzanie ryzykiem (risk management) oraz zapewnienie ciągłości działania usług (business continuity).

SOC może korzystać z różnych narzędzi i technologii, takich jak systemy zarządzania zdarzeniami bezpieczeństwa (SIEM), systemy wykrywania i zapobiegania atakom sieciowym (IDS/IPS), skanery luk w zabezpieczeniach, narzędzia do testów penetracyjnych, systemy ochrony punktów końcowych (endpoint security solutions) i wiele innych. SOC często wykorzystuje również sztuczną inteligencję (AI) i uczenie maszynowe (machine learning), aby zwiększyć efektywność wykrywania i reagowania na zagrożenia.

Koncepcja SOC jest coraz bardziej popularna w dzisiejszych czasach, ponieważ organizacje muszą być gotowe na szybkie i skuteczne reagowanie na nowe zagrożenia, które pojawiają się na co dzień. SOC zapewnia organizacjom skuteczne rozwiązanie, które pozwala na szybkie wykrywanie i reagowanie na zagrożenia, co przekłada się na zwiększenie bezpieczeństwa danych i ciągłości działania usług.


## 26.2. Informacje o zagrożeniach (Threat Intelligence)

Threat intelligence to informacje o zagrożeniach, które umożliwiają organizacjom identyfikowanie, analizowanie i reagowanie na potencjalne zagrożenia dla ich systemów informatycznych. Może to obejmować dane dotyczące źródeł zagrożeń, metod ataków, typów malware oraz sposobów wykorzystywania podatności w systemach informatycznych.

<p align="center">
Rys. 26.2.1. Threat Intelligence 
<br>
  <img src="\assets\img\Sieci\95.png" width="650" alt="Threat Intelligence">
</p>

Istnieją różne źródła informacji o zagrożeniach, takie jak bazy danych o podatnościach, analizy ruchu sieciowego, systemy wykrywania intruzów (IDS) oraz systemy zarządzania zdarzeniami bezpieczeństwa (SIEM). Wiele organizacji korzysta z publicznie dostępnych źródeł informacji o zagrożeniach, takich jak raporty branżowe, ostrzeżenia CERT oraz dane dotyczące zidentyfikowanych ataków.

<p align="center">
Rys. 26.2.2. Działanie Threat Intelligence
<br>
  <img src="\assets\img\Sieci\96.png" width="650" alt="Threat Intelligence">
</p>

Threat intelligence może być wykorzystywane do monitorowania aktywności sieciowej, identyfikowania niebezpiecznych zachowań oraz wykrywania nieznanych wcześniej zagrożeń. Dzięki temu organizacje mogą szybciej reagować na potencjalne zagrożenia, unikać strat wynikających z incydentów bezpieczeństwa oraz lepiej zabezpieczyć swoje systemy informatyczne.


## 26.3. Polowanie na zagrożenia (Threat Hunting)

Polowanie na zagrożenia (ang. Threat Hunting) to proces aktywnego przeszukiwania sieci w celu odkrywania obecności zagrożeń, które mogą unikać wykrycia przez tradycyjne metody monitorowania bezpieczeństwa. W przeciwieństwie do automatycznych systemów wykrywania zagrożeń, które opierają się na zasadzie sygnatur, czyli porównywania wzorców znanych ataków z analizowanymi danymi, Threat Hunting to proces aktywnego przeszukiwania systemów i sieci w celu odnalezienia nieoczekiwanych zachowań, anomalii lub podejrzanych aktywności, które mogą wskazywać na obecność nieznanych dotąd ataków lub zagrożeń.

<p align="center">
Rys. 26.3.1. Działanie Threat Hunting
<br>
  <img src="\assets\img\Sieci\97.png" width="650" alt="Threat Hunting">
</p>

Polowanie na zagrożenia obejmuje wykorzystanie różnorodnych technik i narzędzi, w tym analizę logów systemowych, analizę ruchu sieciowego, skanowanie systemów pod kątem podatności, wykorzystanie narzędzi do analizy kodu źródłowego i obrazów systemów, czy też korzystanie z wywiadu i danych o zagrożeniach (Threat Intelligence).

Celem polowania na zagrożenia jest wczesne wykrycie nieznanych dotąd ataków i zagrożeń, co pozwala na szybką reakcję i minimalizację skutków ataku. Wymaga to jednak wysoko wykwalifikowanych specjalistów oraz zaawansowanych narzędzi i technik analitycznych.

## 26.4. Cyfrowa kryminalistyka (Digital Forencis)

Cyfrowa kryminalistyka (Digital Forensics) to proces zbierania, analizy i interpretacji danych związanych z działaniami przestępczymi dokonanymi z wykorzystaniem technologii cyfrowych. W ramach cyfrowej kryminalistyki, specjaliści z zakresu bezpieczeństwa cyfrowego poszukują dowodów w postaci plików, metadanych, rejestrów, logów, czy zapisów z komunikatorów i innych źródeł.

Proces cyfrowej kryminalistyki może obejmować różne etapy, takie jak zbieranie informacji, analizę dowodów, identyfikację podejrzanych, a także pomoc w prowadzeniu śledztwa i zabezpieczeniu materiału dowodowego przed sądem.

W celu skutecznego przeprowadzenia cyfrowej kryminalistyki konieczne jest wykorzystanie specjalistycznych narzędzi i technologii, takich jak oprogramowanie do odzyskiwania danych, narzędzia do analizy rejestru systemowego, czy programy służące do analizy ruchu sieciowego.

<p align="center">
Rys. 26.4.1. Digital Forencis
<br>
  <img src="\assets\img\Sieci\98.png" width="650" alt="Digital Forencis">
</p>

Cyfrowa kryminalistyka znajduje zastosowanie w wielu dziedzinach, takich jak śledztwa kryminalne, wykrywanie nadużyć finansowych, czy dochodzenie roszczeń w związku z naruszeniami praw autorskich. W dzisiejszych czasach, wraz z coraz większą ilością danych przetwarzanych i przechowywanych w cyfrowej formie, cyfrowa kryminalistyka staje się coraz bardziej istotna dla zapewnienia bezpieczeństwa cyfrowego.


## 26.5. Reagowanie na incydenty (Incident Response)

Reagowanie na incydenty (Incident Response) to proces, który ma na celu przywrócenie normalnego działania systemów informatycznych po ich uszkodzeniu lub ataku. Obejmuje on również działania zmierzające do zminimalizowania negatywnych skutków incydentu oraz zapobieżenia przyszłym atakom.

<p align="center">
Rys. 26.5.1. Incident Response
<br>
  <img src="\assets\img\Sieci\99.png" width="650" alt="Incident Response">
</p>

W przypadku incydentu związanego z bezpieczeństwem informacji, odpowiedź na incydent musi być natychmiastowa i skoordynowana. W tym celu organizacje powinny mieć przygotowany plan reagowania na incydenty (Incident Response Plan), który zawiera procedury postępowania w przypadku różnych rodzajów incydentów, takich jak atak hakerski, wyciek danych, utrata sprzętu, itp.

Plan reagowania na incydenty powinien obejmować cztery główne etapy: wykrycie incydentu, analizę incydentu, eliminację incydentu i przywrócenie normalnego działania systemów informatycznych. W każdym z tych etapów stosowane są specjalistyczne narzędzia i techniki, takie jak narzędzia do zbierania i analizowania logów systemowych, skanery wirusów, narzędzia do odzyskiwania danych, itp.

Oprócz działań technicznych, odpowiedź na incydent powinna uwzględniać również aspekt prawny, tak aby zminimalizować ryzyko odpowiedzialności prawnej. W związku z tym ważne jest, aby organizacje miały przygotowany plan reagowania na incydenty, który uwzględnia wszystkie aspekty reakcji na incydent i jest regularnie aktualizowany.


## 26.6. Odzyskiwanie po awarii (Disaster Recovery)

Odzyskiwanie po awarii (Disaster Recovery) to proces przywracania działania systemów informatycznych, aplikacji i danych po awarii lub innym zdarzeniu, które zakłóca normalne funkcjonowanie systemu. Celem odzyskiwania po awarii jest przywrócenie normalnej działalności biznesowej w jak najkrótszym czasie, minimalizacja utraty danych oraz zapewnienie ciągłości działania organizacji.

<p align="center">
Rys. 26.6.1. Disaster Recovery
<br>
  <img src="\assets\img\Sieci\100.png" width="650" alt="Disaster Recovery">
</p>

W procesie odzyskiwania po awarii wykorzystuje się różne technologie i strategie, takie jak backup i recovery, replikację danych, wirtualizację, konteneryzację, przetwarzanie w chmurze i wiele innych. Planowanie odzyskiwania po awarii powinno obejmować ocenę ryzyka, strategie odzyskiwania, harmonogramy testów i ćwiczeń, a także procedury zarządzania incydentami.

Odzyskiwanie po awarii jest częścią szerszego procesu zarządzania ciągłością działania biznesu (Business Continuity Management, BCM). BCM obejmuje planowanie i zarządzanie ciągłością działania organizacji w przypadku zakłóceń działalności biznesowej spowodowanych przez czynniki zewnętrzne i wewnętrzne, takie jak awarie systemów, ataki cybernetyczne, katastrofy naturalne, choroby, strajki i inne zdarzenia losowe.


# 27. Najlepsze praktyki w zakresie bezpieczeństwa cybernetycznego

Najlepsze praktyki w zakresie bezpieczeństwa cybernetycznego to zestaw zasad i procedur, które pomagają organizacjom w minimalizowaniu ryzyka naruszeń bezpieczeństwa i ochronie przed atakami cybernetycznymi.

## 27.1. Szkolenie ze świadomości bezpieczeńśtwa (Security Awareness Training)

Szkolenie ze świadomości bezpieczeństwa (Security Awareness Training) to proces edukacyjny, którego celem jest zwiększenie świadomości pracowników na temat zagrożeń związanych z bezpieczeństwem informacji oraz zapewnienie im wiedzy i umiejętności potrzebnych do zapobiegania cyberatakom i ochrony danych przed utratą lub kradzieżą.

<p align="center">
Rys. 27.1.1. Security Awareness Training
<br>
  <img src="\assets\img\Sieci\101.png" width="650" alt="SAT">
</p>

Szkolenie ze świadomości bezpieczeństwa jest ważnym elementem strategii bezpieczeństwa cybernetycznego każdej organizacji, ponieważ większość incydentów związanych z bezpieczeństwem informacji wynika z działań użytkowników końcowych, którzy nie są świadomi zagrożeń lub nie wiedzą, jak postępować w przypadku podejrzenia ataku.

Podczas szkolenia ze świadomości bezpieczeństwa pracownicy uczą się zasad bezpiecznego korzystania z systemów informatycznych, w tym sposobów tworzenia mocnych haseł, ochrony danych przed utratą lub kradzieżą, rozpoznawania ataków phishingowych i innych podstawowych zagrożeń związanych z bezpieczeństwem informacji.

Szkolenie ze świadomości bezpieczeństwa powinno być regularne i dostosowane do specyfiki pracy i potrzeb pracowników w organizacji. W ramach szkolenia można wykorzystać różne narzędzia, takie jak filmy edukacyjne, quizy, scenariusze symulujące ataki lub szkolenia online.

Wprowadzenie szkoleń ze świadomości bezpieczeństwa może przyczynić się do znacznego zmniejszenia ryzyka wystąpienia incydentów związanych z bezpieczeństwem informacji oraz zwiększenia efektywności i skuteczności działań związanych z ochroną danych w organizacji.


## 27.2. Zarządzanie hasłami (Password Management)

Zarządzanie hasłami to kluczowy element bezpieczeństwa cybernetycznego. Wiele naruszeń bezpieczeństwa wynika z niewłaściwego zarządzania hasłami lub korzystania z haseł słabych i łatwych do odgadnięcia. W celu zapewnienia bezpieczeństwa, należy stosować się do najlepszych praktyk w zakresie zarządzania hasłami, takich jak:

<p align="center">
Rys. 27.2.1. Password Management
<br>
  <img src="\assets\img\Sieci\102.png" width="650" alt="PM">
</p>

+ Silne hasła - hasła powinny składać się z co najmniej 12 znaków i zawierać różne rodzaje znaków, takie jak litery (w tym duże i małe litery), cyfry i znaki specjalne.
+ Niepowtarzalne hasła - każde konto powinno mieć inne, unikalne hasło. Nigdy nie należy używać tego samego hasła do wielu kont.
+ Regularna zmiana hasła - hasła należy zmieniać co najmniej co 90 dni.
+ Nieprzechowywanie haseł w jawnie dostępnych miejscach - nigdy nie należy przechowywać haseł w postaci czystego tekstu lub w plikach tekstowych.
+ Używanie menedżerów haseł - menedżery haseł to narzędzia, które pozwalają na bezpieczne przechowywanie haseł i automatyczne wypełnianie formularzy logowania.
+ Weryfikacja tożsamości - przed ujawnieniem poufnych informacji lub zmianą ustawień konta, należy zweryfikować tożsamość użytkownika.
+ Używanie autoryzowanych aplikacji - przed instalacją nowych aplikacji, należy upewnić się, że są one autoryzowane przez organizację i nie stanowią zagrożenia dla bezpieczeństwa.
+ Szkolenia dla pracowników - pracownicy powinni być regularnie szkoleni w zakresie bezpieczeństwa haseł i najlepszych praktyk ich zarządzania.


## 27.3. Zarządzanie poprawkami (Patch Management)

Zarządzanie poprawkami (ang. Patch Management) to proces zapewnienia, że wszystkie systemy informatyczne są aktualizowane regularnie w celu poprawienia ich bezpieczeństwa i stabilności. Poprawki, czyli łatki, są to modyfikacje kodu źródłowego lub programów, które usuwają znane błędy lub luki w zabezpieczeniach.

W przypadku oprogramowania, zwłaszcza systemów operacyjnych i aplikacji, łatki są niezbędne dla zapewnienia bezpieczeństwa systemów. Dzięki nim, twórcy oprogramowania mogą naprawić błędy, które mogą zostać wykorzystane przez atakujących do przejęcia kontroli nad systemem.

<p align="center">
Rys. 27.3.1. Patch  Management
<br>
  <img src="\assets\img\Sieci\103.png" width="650" alt="PM-1">
</p>

Proces zarządzania poprawkami powinien obejmować identyfikację dostępnych aktualizacji, ich ocenę pod kątem wpływu na systemy i aplikacje, testowanie łatek na środowisku testowym przed wdrożeniem ich na produkcji oraz wdrażanie ich na systemach produkcyjnych. Ważne jest również monitorowanie systemów i aplikacji, aby upewnić się, że wszystkie poprawki są aktualne i systemy są bezpieczne.

Efektywny proces zarządzania poprawkami jest kluczowy dla zapewnienia bezpieczeństwa systemów informatycznych i minimalizowania ryzyka ataków. Wiele narzędzi dostępnych na rynku może pomóc w automatyzacji tego procesu, co ułatwia zarządzanie łatkami i umożliwia szybkie reagowanie na nowe zagrożenia.


## 27.4. Segmentacja sieci (Network Segmentation)

Segmentacja sieci (ang. network segmentation) to technika polegająca na podziale sieci na mniejsze, izolowane od siebie segmenty. Jest to ważne narzędzie w zarządzaniu bezpieczeństwem sieciowym, które pozwala na ograniczenie ryzyka ataku, rozprzestrzeniania się złośliwego oprogramowania i niepożądanego ruchu w sieci.

<p align="center">
Rys. 27.4.1. Network Segmentation
<br>
  <img src="\assets\img\Sieci\104.png" width="650" alt="NS">
</p>

Segmentacja sieci umożliwia ograniczenie dostępu do poszczególnych zasobów sieciowych tylko dla uprawnionych użytkowników i urządzeń. Oznacza to, że użytkownicy i urządzenia w jednym segmencie sieci nie mają dostępu do zasobów w innych segmentach, chyba że posiadają odpowiednie uprawnienia.

Podział sieci na mniejsze segmenty umożliwia też łatwiejsze monitorowanie i zarządzanie ruchem sieciowym oraz wdrożenie bardziej skutecznych zasad bezpieczeństwa sieciowego, takich jak kontrola dostępu, filtrowanie ruchu, detekcja i odpowiedź na incydenty bezpieczeństwa.

Segmentacja sieci jest jednym z podstawowych kroków w zapewnieniu bezpieczeństwa sieciowego i jest często stosowana wraz z innymi technikami i narzędziami bezpieczeństwa sieciowego, takimi jak zapora ogniowa, sieć prywatna wirtualna (VPN), detekcja zagrożeń itp.


## 27.5. Kopie zapasowe i odzyskiwanie (Backup and Recovery)

Kopie zapasowe i odzyskiwanie (Backup and Recovery) to proces tworzenia i przechowywania kopii danych, tak aby można było je przywrócić w przypadku awarii lub utraty danych. Jest to istotny element w ramach strategii bezpieczeństwa informacji, ponieważ zapewnia możliwość szybkiego przywrócenia systemów i danych do stanu sprzed awarii lub incydentu bezpieczeństwa.

<p align="center">
Rys. 27.5.1. Backup and Recovery
<br>
  <img src="\assets\img\Sieci\105.png" width="650" alt="BaR">
</p>

W przypadku awarii lub ataku, kopia zapasowa danych umożliwia przywrócenie systemów i danych do stanu sprzed zdarzenia, minimalizując tym samym straty wynikające z utraty danych lub czasu niedostępności systemów. Warto zauważyć, że kopia zapasowa powinna być regularnie tworzona, a także przechowywana w bezpiecznym miejscu, np. na zewnętrznym dysku twardym lub w chmurze.

Odzyskiwanie danych to proces przywracania danych z kopii zapasowej, a jego skuteczność zależy od tego, jak dobrze została wykonana kopia zapasowa. Warto pamiętać, że proces odzyskiwania danych może być czasochłonny, dlatego należy mieć odpowiedni plan odzyskiwania danych, który uwzględni czas potrzebny na przywrócenie systemów i danych.

W ramach strategii kopii zapasowych i odzyskiwania, ważne jest również testowanie i weryfikowanie procesu odzyskiwania danych, aby mieć pewność, że proces ten przebiegnie sprawnie w przypadku awarii lub incydentu bezpieczeństwa.


# 28. Nowe technologie w cyberbezpieczeństwie

Nowe technologie w cyberbezpieczeństwie są nieustannie rozwijane, aby skuteczniej przeciwdziałać rosnącej liczbie zagrożeń.

## 28.1. Sztuczna inteligencja i uczenie maszynowe w cyberbezpieczeństwie

Sztuczna inteligencja (AI) i uczenie maszynowe (ML) są coraz częściej wykorzystywane w cyberbezpieczeństwie, aby zapewnić szybką i skuteczną ochronę przed zagrożeniami. Technologie te mają zastosowanie w wielu obszarach cyberbezpieczeństwa, w tym w rozpoznawaniu i analizie zagrożeń, wykrywaniu anomali w zachowaniu użytkowników, rozpoznawaniu złośliwego oprogramowania oraz w modelowaniu ryzyka.

<p align="center">
Rys. 28.1.1. AI i ML w cyberbezpieczeństwie
<br>
  <img src="\assets\img\Sieci\106.png" width="650" alt="AI and ML">
</p>

AI i ML pozwalają na szybkie przetwarzanie dużych ilości danych, dzięki czemu mogą automatycznie wykrywać nieznane wcześniej zagrożenia, analizować zachowania użytkowników i dostarczać rekomendacje dotyczące działań obronnych. Wykorzystując te technologie, systemy bezpieczeństwa mogą przewidywać, które aplikacje i urządzenia są najbardziej narażone na ataki oraz dostarczać odpowiednie zabezpieczenia, takie jak automatyczne aktualizacje lub blokowanie niebezpiecznych aplikacji.

Jednym z głównych wyzwań związanych z wykorzystaniem AI i ML w cyberbezpieczeństwie jest potrzeba stałego uczenia i dostosowywania algorytmów do zmieniających się zagrożeń. Ponadto, AI i ML mogą generować fałszywie pozytywne lub negatywne wyniki, co wymaga dokładnej analizy przez ludzi.

W związku z tym, coraz więcej firm oferuje rozwiązania, które łączą AI i ML z ludzką wiedzą i doświadczeniem. W ten sposób, systemy bezpieczeństwa są w stanie zapewnić szybką i skuteczną ochronę przed zagrożeniami oraz umożliwić analizę wyników przez ekspertów.


## 28.2. Blockchain i kryptowaluty

Blockchain i kryptowaluty to dwie technologie, które wprowadziły rewolucję w dziedzinie finansów i transakcji cyfrowych. Blockchain jest to rozproszona baza danych, która działa na zasadzie sieci peer-to-peer, a każdy z węzłów przechowuje kopię danych. Jest to technologia niezwykle bezpieczna, gdyż każdy blok danych jest opatrzony niepowtarzalnym kodem, a cała sieć jest chroniona przez algorytm kryptograficzny. Właśnie z tego powodu blockchain jest stosowany do przechowywania i przesyłania informacji o wartości, takich jak kryptowaluty.

<p align="center">
Rys. 28.2.1. Jak działa Blockchain
<br>
  <img src="\assets\img\Sieci\107.png" width="650" alt="Blockchain">
</p>

Kryptowaluty, takie jak Bitcoin czy Ethereum, są cyfrowymi aktywami, które funkcjonują na podstawie technologii blockchain. Dzięki temu, że transakcje są zapisywane na blockchainie, a każdy blok danych jest chroniony algorytmem kryptograficznym, kryptowaluty zapewniają bezpieczeństwo transakcji oraz anonimowość użytkowników. Oczywiście, tak jak każda inna technologia, blockchain i kryptowaluty także niosą ze sobą pewne ryzyka, takie jak np. utrata kluczy prywatnych, ataki hakerskie czy złośliwe oprogramowanie. W związku z tym, wraz z rozwojem technologii, pojawiają się coraz bardziej zaawansowane narzędzia i rozwiązania, które pomagają zwiększać bezpieczeństwo i chronić użytkowników przed różnymi zagrożeniami.


## 28.3. Bezpieczeństwo Internetu Rzeczy (IoT)

Internet Rzeczy (IoT) to rozwijająca się dziedzina technologii, która pozwala na łączenie urządzeń ze sobą i z siecią internetową, aby wymieniały między sobą informacje. Urządzenia te to między innymi inteligentne urządzenia domowe, systemy kontroli przemysłowej, czy nawet maszyny medyczne.

<p align="center">
Rys. 28.3.1. Bezpieczeństwo Internetu Rzeczy (IoT)
<br>
  <img src="\assets\img\Sieci\108.png" width="650" alt="IoT">
</p>


Bezpieczeństwo Internetu Rzeczy jest jednym z najważniejszych wyzwań, jakie stawia przed nami ta technologia. Urządzenia IoT są zazwyczaj małe, mają ograniczone zasoby, a ich producenci często skupiają się na funkcjonalności, kosztem bezpieczeństwa. To sprawia, że takie urządzenia są podatne na ataki hakerskie, a zagrożenia te mogą mieć poważne konsekwencje, takie jak kradzież danych lub sterowanie urządzeniami przez niepowołane osoby.

Aby zapewnić bezpieczeństwo IoT, producenci muszą projektować urządzenia z myślą o bezpieczeństwie, uwzględniając takie kwestie jak autoryzacja, uwierzytelnianie, szyfrowanie i ochrona przed atakami typu DDoS. Istotne jest również aktualizowanie oprogramowania, które pozwala na łatanie luk w zabezpieczeniach.

Poza tym, ważne jest, aby użytkownicy sami również dbali o bezpieczeństwo swoich urządzeń IoT, np. poprzez stosowanie silnych haseł, ograniczenie dostępu do sieci Wi-Fi oraz korzystanie z narzędzi zabezpieczających takich jak firewall.


## 28.4. Obliczenia kwantowe i kryptografia

Obliczenia kwantowe i kryptografia to dziedziny, które są ze sobą ściśle powiązane. Obliczenia kwantowe to nowoczesna dziedzina informatyki, która zajmuje się wykorzystaniem własności kwantowych do przetwarzania informacji. Jednym z najważniejszych zastosowań obliczeń kwantowych jest kryptografia kwantowa, która umożliwia bezpieczne przesyłanie informacji w sposób odporny na ataki kwantowe.

Tradycyjne algorytmy kryptograficzne, takie jak RSA czy AES, opierają się na problemach matematycznych, których rozwiązanie jest bardzo trudne do uzyskania. Jednak z powodu rosnącej mocy obliczeniowej komputerów, te algorytmy zaczynają być coraz bardziej narażone na ataki. Obliczenia kwantowe oferują nowe sposoby rozwiązania problemów kryptograficznych, które są znacznie trudniejsze do złamania przez klasyczne komputery.

Kryptografia kwantowa wykorzystuje zjawisko splątania kwantowego, które pozwala na bezpieczne przesyłanie informacji. W kryptografii kwantowej, każda bitowa wartość (1 lub 0) jest zapisywana jako stan kwantowy. Zasada nieoznaczoności Heisenberga mówi, że każde pomiary w przypadku kwantów wprowadzają zakłócenia w stanie kwantowym, a zatem w przypadku próby odczytu informacji, atakujący wprowadza zmiany w transmisji, co może zostać wykryte. W ten sposób, w przypadku ataku na transmisję, od razu jest to widoczne, co daje możliwość przerwania transmisji.

Obecnie technologia kryptografii kwantowej jest jeszcze na etapie rozwoju, jednak już teraz można zauważyć zwiększające się zainteresowanie tym tematem. W najbliższych latach można oczekiwać coraz większego wykorzystania obliczeń kwantowych w celu zabezpieczenia informacji.
