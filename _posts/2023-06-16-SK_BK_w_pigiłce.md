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

- [Architektura sieciowa](#1. Architektura-sieciowa)
- [Rozdział 2](#rozdział-2)
- [Rozdział 3](#rozdział-3)



# 1. Architektura sieciowa

Architektura sieciowa to sposób organizacji i połączenia urządzeń sieciowych, który umożliwia wymianę danych i zasobów pomiędzy nimi. Składa się z różnych elementów, które mają określone role i funkcje, a ich współpraca umożliwia poprawne działanie sieci. Oto kilka podstawowych elementów architektury sieciowej:

<p align="center">
  <img src="\assets\img\Sieci\1.png" width="650" alt="architektura">
  <br>
  Rys.1 Architektura sieci komputerowej
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


## Model TCP/IP

Model TCP/IP to model warstwowy, który opisuje sposób, w jaki urządzenia sieciowe komunikują się ze sobą w sieciach opartych o protokół TCP/IP. Model ten składa się z 4 warstw, każda z nich odpowiada za określone zadania i protokoły. Oto opis każdej z nich:

<p align="center">
Rys. 1.1.1. Model TCP/IP
<br>
  <img src="\assets\img\Sieci\2.JPG" width="650" alt="TCP/IP">
  <br>
  Źródło: https://pasja-informatyki.pl/pliki/model-tcp-ip.jpg
</p>

+ Warstwa aplikacji: to warstwa, która umożliwia aplikacjom korzystanie z sieci (np. WWW, poczta elektroniczna, wymiana plików, połączenia terminalowe czy komunikatory). Zawiera protokoły, takie jak HTTP, SMTP, FTP, DNS, SSH, które pozwalają na przesyłanie danych między aplikacjami. Protokoły te są zwykle napisane w języku wysokiego poziomu, co umożliwia programistom łatwe korzystanie z nich.
+ Warstwa transportowa: to warstwa, która zapewnia poprawne przesyłanie danych między aplikacjami. Zawiera protokoły, takie jak TCP i UDP, które umożliwiają kontrolę przepływu danych, kontrolę błędów i segmentację danych na mniejsze pakiety.
+ Warstwa sieciowa: to warstwa, która odpowiada za kierowanie ruchem między różnymi sieciami. Zawiera protokoły, takie jak IP, ICMP, ARP, które pozwalają na przesyłanie danych między różnymi sieciami oraz na znajdowanie adresów urządzeń w sieci.
+ Warstwa dostępu do sieci: to warstwa, która umożliwia urządzeniom komunikację z fizycznymi urządzeniami sieciowymi, takimi jak karty sieciowe, switch'e i routery. Zawiera protokoły, takie jak Ethernet, Token Ring, FDDI, które określają sposób transmisji danych między urządzeniami.

Wiadomość jest wysyłana od najwyżej do najniższej warstwy, a w każdej z nich do wiadomości dodawane są kolejne nagłówki zapewniające prawidłowe dostarczanie danych – proces ten nazywany jest enkapsulacją. Dane zwrotne powracają od najniższej do najwyżej warstwy do punktu docelowego.
