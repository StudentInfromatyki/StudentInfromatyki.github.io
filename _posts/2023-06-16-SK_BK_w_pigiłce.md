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

