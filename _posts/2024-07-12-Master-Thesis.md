[Kliknij tutaj, aby zobacyć pracę](https://github.com/Danchivskyi/Master-s-Dissertation/blob/main/Praca_dyplomowa_magisterska.pdf)


# Spis treści
[1. Wprowadzenie](#1-wprowadzenie) 

[1.1. Cel i zakres pracy](#11-cel-i-zakres-pracy) 

[2. Krytyka teorii: wyzwania w pracy badawczej](#2-Krytyka-teorii-:-wyzwania-w-pracy-badawczej) 

[2.1. Geneza i ewolucja ataków USB](#21-Geneza-i-ewolucja-ataków-USB) 

[2.1.1. Kluczowe pojęcia](#211-Kluczowe-pojecia) 

[2.2. Analiza przypadków i ich wpływ na firmware](#22-Analiza-przypadków-i-ich-wpływ-na-firmware) 

[2.2.1. Czym jest atak USB?](#221-Czym-jest-atak-USB?) 

# 1. Wprowadzenie

W dzisiejszych czasach, kiedy ma miejsce cyfrowa rewolucja, w obszarze bezpieczeństwa komputerowego jednym z kluczowych aspektów jest np. ochrona danych osobowych i firmowych. Istnieje wiele różnego rodzaju zagrożeń, które są powszechnie znane, oraz takich nieco ``zaskakujących'' jak urządzenia USB, które w chwili obecnej są używane jako jedne z bardziej popularnych i bezpiecznych nośników wymiany danych, ale jak się okazuje także przyczyniają się do różnych ataków hakerskich, co prowadzi do poważnych skutków w postaci wycieku danych i innych naruszeń bezpieczeństwa. Niniejsza praca dyplomowa ma na celu przedstawienie problematyki bezpieczeństwa komputerowego w kontekście ataków przy użyciu urządzeń USB.

Ataki te, jak historia pokazuje, mogą przybierać różne formy -- od prostych programów szpiegujących po zaawansowane złośliwe oprogramowanie takie jak Stuxnet. 

Jak sama nazwa wskazuje, urządzenia BadUSB to tak zwane urządzenia, które mają potencjalną możliwość przejęcia kontroli nad innymi urządzeniami różnego typu. BadUSB oznacza także lukę odkrytą w 2006 roku, która umożliwiała automatyczne uruchamianie programów przechowywanych na płytach CD-ROM po ich włożeniu do napędu czytnika w komputerze. Urządzenia BadUSB można znaleźć w wielu zaawansowanych rozwiązaniach technicznych, takich jak zewnętrzne dyski twarde, karty pamięci SD, czytniki kart pamięci itd. \cite{4}.

W kontekście niniejszej pracy kluczowe jest zrozumienie, jak ataki BadUSB ewoluowały, jakie są ich współczesne formy oraz jakie kroki można podjąć, aby skutecznie zabezpieczyć urządzenia i dane przed potencjalnymi zagrożeniami. Praca ta, opierając się na analizie literatury, studiach przypadków oraz własnych badaniach, ma na celu zwiększenie świadomości na temat tego zagrożenia oraz zaproponowanie efektywnych strategii obrony.

# 1.1. Cel i zakres pracy

Celem niniejszej pracy magisterskiej jest dogłębna analiza i zrozumienie zagrożeń związanych z atakami na bezpieczeństwo komputerów przy użyciu urządzeń USB. Praca skupia się na identyfikowaniu różnych metod, którymi atakujący mogą wykorzystywać urządzenia USB do infiltracji systemów komputerowych, kradzieży danych lub wprowadzania złośliwego oprogramowania.

Zakres tej pracy obejmuje:
- Analizę historyczną: Badanie przypadków ataków z przeszłości, by zrozumieć ewolucję taktyk i technik wykorzystywanych przez hakerów -- Rozdział 2.
- Studium technik ataków: Skupienie się na szczegółowym omówieniu różnorodnych technik stosowanych w atakach USB, włączając w to zarówno aspekty sprzętowe, jak i oprogramowanie -- Rozdział 3.
- Przegląd współczesnych metod obrony: Zbadanie aktualnych strategii i narzędzi stosowanych do ochrony przed tego typu atakami, ocena ich skuteczności. -- Rozdział 3.3.
- Praktyczna analiza: Wykonanie serii testów na wybranych urządzeniach USB, by empirycznie ocenić ich podatność na ataki i skuteczność zaimplementowanych środków ochrony -- Rozdział 4.

Zdaniem autora, praca powinna również przyczynić się do rozwoju skuteczniejszych metod ochrony komputerów przed atakami wykorzystującymi urządzenia USB.

# 2. Krytyka teorii: wyzwania w pracy badawczej

W ramach prezentowanej pracy magisterskiej skoncentrowano się na krytycznym przeglądzie obecnych teorii i metodologii stosowanych w badaniach nad atakami USB oraz na analizie wyzwań, które one stawiają. 
Kwestie, które zostaną omawiane przedstawią, jak bardzo skomplikowanym i zmiennym problemem jest bezpieczeństwo w sieci, zwłaszcza w kontekście ciągłego rozwoju technologii.

W czasach rewolucji informacyjnej oraz nowych zagrożeń, które wynikają w różnych sektorach ludzkiej działalności jak: polityka, gospodarka, biznes, finanse, transport, infrastruktura, poczta, telekomunikacja, medycyna oraz nauka. Rozwój technologii informacyjnych i potrzeba użycia Internetu na co dzień prowadzi do powstania wielu nowych wyzwań i zagrożeń w cyberprzestrzeni. Tradycyjne modele bezpieczeństwa często okazują się niewystarczające wobec szybko ewoluujących taktyk stosowanych przez cyberprzestępców. Brak odpowiednich zabezpieczeń pozwala cyberprzestępcom na wykorzystanie tych luk dla swoich celów. Szczególnie ataki typu BadUSB są trudne do wykrycia przy użyciu tradycyjnych metod. Wymaga to dostosowania zasad bezpieczeństwa do nowych rodzajów zagrożeń. \cite{5}.

Napotkano również na wyzwania metodologiczne. Istniejące metody badawcze okazują się niewystarczające do zrozumienia skomplikowanych i dynamicznych aspektów ataków USB. Te wyzwania podkreślają potrzebę rozwoju nowych metodologii, które mogą skutecznie analizować i przewidywać zagrożenia w tym obszarze.

Jednym z kluczowych problemów w badaniach była bariera w dostępie do danych o atakach i ich skutkach. Ograniczony dostęp do informacji wynika częściowo z poufności danych związanych z incydentami bezpieczeństwa, co utrudnia tworzenie solidnych teorii i modeli.

Wreszcie, badania wykazały, że potrzebne jest łączenie różnych dziedzin w podejściu do problemu ataków USB. Aby zrozumieć i skutecznie przeciwdziałać temu zagrożeniu, trzeba połączyć wiedzę z informatyki, inżynierii oprogramowania, cyberbezpieczeństwa i psychologii cybernetycznej. Takie połączenie dyscyplin jest konieczne do opracowania kompleksowego i efektywnego podejścia do tego problemu.

# 2.1. Geneza i ewolucja ataków USB

W dzisiejszych czasach coraz częściej wykorzystywane są ataki za pomocą urządzeń USB, które znacząco rozwinęły się na przestrzeni ostatnich dekad Z początkiem masowej popularności urządzeń przenośnych USB, takich jak pendrive'y czy zewnętrzne dyski twarde, pojawiły się także nowe możliwości dla atakujących. Pierwsze przypadki wykorzystania tych urządzeń do celów szkodliwych były stosunkowo proste i opierały się głównie na automatycznym uruchamianiu złośliwego oprogramowania poprzez funkcję autorun systemu Windows \cite{6}.

Nieco póżniej zaczęły być realizowane nowe bardziej zaawansowane techniki. Świetnym przykładem może być Stuxnet, który w 2010 roku zaatakował irański program nuklearny, choć prace nad nim prawdopodobnie rozpoczęły się już w 2005 roku. Obecnie powszechnie przyjmuje się, że Stuxnet został stworzony przez agencje wywiadowcze Stanów Zjednoczonych i Izraela. Choć żaden z rządów nigdy oficjalnie nie przyznał się do stworzenia Stuxneta, w filmie z 2011 roku pokazano ten atak jako sukces szefa izraelskich sił zbrojnych. W 2010 r. inspektorzy Agencji Energii Atomowej zauważyli awarie wielu irańskich wirówek, co mogło być skutkiem ataku Stuxneta. Cieżko było to wykryć, ponieważ irańskie obiekty nuklearne nie były podłączone do Internetu. Kiedy zespół ds. bezpieczeństwa z Białorusi przybył, aby zbadać nieprawidłowo działające komputery w Iranie, odkrył złośliwe oprogramowanie, które później nazwano Stuxnetem \cite{7}.

Mimo że twórcy Stuxnet zaprogramowali jego wygaśnięcie w czerwcu 2022 roku, atak ten zainspirował powstanie innych ataków uznawanych za podobne do niego lub za jego następców:
- Duqu, który powstał w 2011 roku, jest oparty na kodzie Stuxneta. Ten atak został zarejestrowany jako próba rejestrowania naciśnięć klawiszy i wyciągania danych z obiektów przemysłowych, aby w późniejszym czasie móc je wykorzystać do ataków. Polegał na ukrywaniu transmisji danych w ruchu HTTP i przesyłaniu złośliwych plików w formacie jpg.
- Flame, który powstał w 2012 roku, polegał na rejestrowaniu rozmów przez Skype, rejestrowaniu naciśnięć klawiszy i zbieraniu zrzutów ekranu. Jego celem były organizacje rządowe i edukacyjne oraz konkretne osoby prywatne.
- Havex, który został odkryty w 2013 roku, miał na celu zbieranie informacji m.in. od firm energetycznych, lotniczych, obronnych i farmaceutycznych. Szkodliwe oprogramowanie Havex atakowało głównie organizacje w USA, Europie i Kanadzie. Ten typ ataku atakował systemy kontroli przemysłowej i komunikował się z serwerem nadzorującym pracę złośliwego kodu, z którego dostarczane były kolejne moduły zawierające niebezpieczne narzędzia.
- Industroyer, który miał na celu niszczyć obiekty energetyczne. Atak ten został zauważony na Ukrainie, gdzie spowodował przerwę w dostawie prądu w grudniu 2016 roku.
- Triton, który powstał w 2017 roku i został zauważony podczas ataków na systemy bezpieczeństwa zakładu petrochemicznego na Bliskim Wschodzie.
- Most recent wirus, który miał cechy Stuxneta zaatakował nieokreśloną infrastrukturę sieciową w Iranie w październiku 2018 r.

Innym świetnym przykładem jest Conficker, który rozprzestrzeniał się przez sieci komputerowe oraz urządzenia USB, wykorzystując lukę w systemie Windows \cite{8}. Conficker pokazał, jak szybko i skutecznie może rozprzestrzeniać się złośliwe oprogramowanie, wykorzystując zarówno sieci, jak i fizyczne nośniki. Zainfekował wiele komputerów rządowych, biznesowych i domowych w ponad 190 krajach. Ten typ ataku pozostaje najbardziej uporczywym robakiem komputerowym, jaki kiedykolwiek powstał. Podobnie jak w przypadku ataku Stuxnet, zrodziło to wiele wersji Confickera. Każda wersja miała całkiem inne cele ataku, począwszy od wstrzykiwania złośliwego kodu do wiadomości phishingowych. Do tej pory zainfekowano około 11 milionów urządzeń. Najbardziej imponującą cechą Confickera było podejście kryptograficzne. Sposób szyfrowania w tym ataku był nietypowy; wykorzystano takie metody kodowania jak: RC4, RSA i MD6.

<p align="center">
  Rys.2.1. Przedstawienie ataku Conficker, źródło: https://tiny.pl/dw19h
<br>
  <img src="\assets\img\MasterThesis\18.png" width="650" alt="xss">
  <br>
  Źródło: https://www.cybereason.com/hubfs/image1-15.png
</p>

W ostatnich dekadach znacznie wzrosły zagrożenia cybernetyczne. Z każdym postępem w dziedzinie cyfrowej pojawiają się nowe zagrożenia, które są wykorzystywane przez cyberprzestępców. Teraz, dzięki odkryciu sztucznej inteligencji, atakujący posługują się bardziej wyrafinowanymi metodami ataku. Wzrost ataków obserwujemy od ataków ransomware po taktyki socjotechniczne. Według The Harvard Business Review w 2020 roku liczba ataków ransomware wzrosła o 150 procent w porównaniu z rokiem poprzednim. Kolejnym znanym zagrożeniem jest phishing, którego celem jest wyłudzenie poufnych informacji.

W latach 2009-2012 wzrosła liczba zaawansowanych zagrożeń ATP (ang. Advanced Persistent Threats). Są to ataki, które polegają na kradzieży danych z konkretnego celu. Atakujący spędzali długi czas, aby wydobyć informacje i poukładać z nich ``stos z klocków'', aby móc wyrządzić szkodę, ukraść pieniądze lub dane. Jednym z dobrze znanych przykładów jest zagrożenie, które miało miejsce w 2010 roku, znane jako ``Operacja Aurora''. Atakujący uzyskiwali dostęp do różnych wrażliwych danych, wykorzystując luki w zabezpieczeniach firmowych \cite{9}.

<p align="center">
  Rys.2.2. Przedstawienie Operacji Aurora źródło: https://tiny.pl/dw1r8
<br>
  <img src="\assets\img\MasterThesis\19.png" width="650" alt="xss">
  <br>
  Źródło: https://images.ctfassets.net/5natoedl294r/1bDvDHkf5nmdIEHUnHdkx5/892e0387ef35fdc64d02fe45d1786438/1_1400x1233.png?w=828&q=75&fit=fill&fm=webp
</p>

W latach 2013-2016 wzrosła liczba ataków ransomware oraz ataków BEC (ang. Business Email Compromise). Jak wiadomo, ransomware to rodzaj złośliwego oprogramowania, podczas gdy atak Business Email Compromise to atak, który polega na podszywaniu się i nakłanianiu innych osób do wykonania konkretnego działania. Ataki tego typu okazały się bardzo opłacalne, ponieważ dochody z nich sięgały miliardów dolarów rocznie. Przykładem ataków ransomware może być WannaCry, który dotknął setki tysięcy komputerów w wielu krajach. Polegał on na odblokowaniu zaatakowanych systemów w zamian za zapłatę pieniędzy. Również dobrym przykładem jest CEO Fraud w 2015 roku, w którym firma Ubiquiti Networks stała się ofiarą ataku BEC. Tego typu atak kosztował firmę 46,7 miliona dolarów.

W latach 2017-2020 zauważono wzrost zagrożeń związanych z IoT (Internet of Things) i AI (Artificial Intelligence). Urządzenia IoT stają się coraz bardziej popularne z każdym dniem. Zazwyczaj tego typu urządzenia nie posiadają odpowiednich zabezpieczeń, co sprawia, że stają się łatwym celem dla różnego rodzaju ataków. Z kolei sztuczna inteligencja odgrywa coraz większą rolę w ewolucji cyberzagrożeń. Z jednej strony AI pomaga w ulepszaniu bezpieczeństwa, a z drugiej strony cyberprzestępcy wykorzystują ją do tworzenia bardziej groźnych i ulepszonych ataków. Na przykład można wykorzystać ją do generowania realistycznych wiadomości phishingowych. W 2017 roku botnet Mirai był masowym atakiem, który skompromitował setki tysięcy urządzeń IoT, zamieniając je w sieć botów, które później wykorzystywano do przeprowadzania różnych ataków DDoS na strony internetowe. Innym przykładem jest DeepLocker, który w 2018 roku ominął tradycyjne zabezpieczenia, wykorzystując algorytmy sztucznej inteligencji do ukrycia się do momentu dostarczenia do celu

W latach 2021-2022 wzrosła liczba ataków typu supply chain i Ransomware-as-a-Service (RaaS). Polegały one na zaatakowaniu celu aby uzyskać dostęp do sieci. Ataki Ransomware-as-a-Service polegają na udostępnianiu oprogramowania ransomware innym cyberprzestępcom w zamian za część uzyskanych zysków. Jeden z najbardziej znanych ataków tego typu jest atak SolarWinds supply chain, który polegał na wykorzystaniu naruszenia aktualizacji oprogramowania SolarWinds do rozpowszechnienia złośliwego oprogramowania wśród swoich klientów. Innym przykładem może być Colonial Pipeline z 2021 roku.

W latach 2022 do chwili obecnej coraz bardziej popularne stają się ataki deep fake oraz oszustwa polegające na syntetycznej tożsamości. Deepfake polega na tworzeniu nagrań wideo lub audio, które mogą być wykorzystywane do ataków socjotechnicznych. Oszustwa polegające na syntetycznej tożsamości oznaczają, że osoby dokonujące przestępstw tworzą fałszywą tożsamość, którą wykorzystują do wyłudzania danych \cite{9}.

# 2.1.1. Kluczowe pojęcia

W świecie cyberbezpieczeństwa istnieje wiele pojęć. Liczba pojęć związanych z dziedziną bezpieczeństwa jest naprawdę duża. Jeśli dobrze się zastanowić, można wskazać około 100 różnych pojęć. Zacznijmy od najważniejszych terminów, takich jak:
- Firmware -- jest to oprogramowanie wbudowane w urządzeniu elektrycznym, które kontroluje jego podstawowe funkcje i operacje. Zazwyczaj to oprogramowanie uruchamia się po włączeniu urządzenia. Firmware dostosowany jest do routerów, kart sieciowych, dysków twardych, drukarek oraz innych urządzeń peryferyjnych. 
- Cybersecurity -- to dziedzina zajmująca się ochroną systemów komputerowych, sieci, danych oraz urządzeń przed różnymi zagrożeniami związanymi z cyberprzestrzenią. W ramach cyberbezpieczeństwa wyróżnia się zapewnianie poufności, integralności, dostępności, autentyczności oraz zgodności z przepisami.
- BadUSB -- to rodzaj zagrożeń związanych z obszarem cyberbezpieczeństwa, polegających na modyfikacji firmware'u urządzeń USB w celu ich złośliwego wykorzystania.
- Advanced Persistent Threat (APT) -- jest to atak w którym osoba atakująca wykorzystuje najbardziej znane taktyki i technologie. Celem tego ataku jest pozostawianie ‘under the radar’ i przeszukanie sieci 'pozostając w cieniu', aby nikt nie wykrył po dłuższym czasie, że osoba atakująca przebywa w sieci. 
- Advanced Threat Protection (ATP) -- jest to rozwiązanie, które zabezpiecza przed złośliwym oprogramowaniem lub atakami hakerskimi. Advanced Threat Protection obejmuje zarówno oprogramowanie, jak i zarządzane usługi bezpieczeństwa.
- Malware -- jest to ogólne pojęcie, które określa rodzaj złośliwego oprogramowania komputerowego. 
- Exploit -- jest to wykorzystanie luki lub wady w systemach sieciowych aby zaatakować go. 
- Endpoint Protection -- jest to system, który monitoruje urządzenia końcowe w celu zabezpieczenia ich od złośliwych działań lub oprogramowań.
- Sandbox(ing) -- jest to odizolowane środowisko w którym można bezpiecznie uruchomić złośliwe oprogramowanie bez ryzyka uszkodzenia urządzenia hosta lub sieci.
- Threat Hunting -- jest to aktywne działanie w zakresie obrony przed cyberzagrożeniami, w którym odpowiedni specjalista przeszukuje sieć w celu wykrycia i naprawienia zagrożeń. 
- Virus -- jest to złośliwy program uruchamiany na komputerze w celu zainfekowania urządzenia, po czym ten może przejąc kontrolę nad przeglądarką, wysyłać spam bądź wyłączyć ustawienia zabezpieczeń i inne złośliwe działania.
- Vulnerability -- to słabe punkty oprogramowania, które mogą zostać wykorzystane przez cyberprzestępców w celu naruszenia bezpieczeństwa.
- Zero-day Exploit -- odnosi się do rodzaju exploitu, który został stworzony w celu wykorzystania luki w zabezpieczeniach, przed tym jak inna osoba zdąży ją wykryć i naprawić \cite{10}.

# 2.2. Analiza przypadków i ich wpływ na firmware

Sekcja ta skupia się na przeglądzie literatury naukowej oraz analizie konkretnych przypadków ataków na bezpieczeństwo komputera, które wykorzystują urządzenia USB. Celem jest zrozumienie, jak te ataki mogą naruszyć spójność firmware urządzeń, co stanowi poważne zagrożenie dla bezpieczeństwa systemów komputerowych.

Jak wiadomo, świat technologii nie stoi w miejscu, co niesie za sobą pojawienie się nowych zagrożeń przy każdym otwarciu. Każdego dnia pojawiają się nowe ataki, dlatego ważne jest, aby być świadomym takich kwestii jak utrata danych, kradzież poufnych informacji, ataki ransomware, infekcje złośliwym oprogramowaniem, i tak dalej. Jedną z form takiego ataku jest atak z wykorzystaniem złośliwego firmware na urządzeniach USB.

# 2.2.1. Czym jest atak USB?

Każdego dnia pojawiają się nowe ataki, dlatego ważne jest, aby być świadomym takich kwestii jak utrata danych, kradzież poufnych informacji, ataki ransomware, infekcje złośliwym oprogramowaniem, i tak dalej. Jedną z form takiego ataku jest atak z wykorzystaniem złośliwego firmware na urządzeniach USB.

Wśród różnych form można wymienić następujące typy ataku, które zostaną opisane w dalszym kroku: BadUSB, Tailgating i USB drop. Chociaż istnieją różne rodzaje ataków USB, można podzielić ich na kilka grup: 
- Przeprogramowanie wewnętrznego mikrokontrolera USB -- jest to sytuacja, w której urządzenia USB się być bezpieczne, ale wykonuje złośliwe działania, takie jak wprowadzanie naciśnięcia klawiszy, Rubber Ducky, PHUKD/URFUKED, USBdriveby, Evilduino i inne.
- Przeprogramowanie oprogramowania sprzętowego USB w celu wykonania złośliwych działań -- odnosi się do działań, w których pobierane są złośliwe oprogramowania, eksfiltracja danych itp. Przykładem mogą być maszyny wirtualne, które zostają złamane, zaliczają się do tego także omijanie ochrony hasłem, itp.  
- Wykorzystywanie niedociągnięć w sposobie interakcji systemów operacyjnych z USB -- jest to sytuacja, w której oprogramowanie układowe USB nie zostaje zmienione, a zachowanie systemów operacyjnych w odniesieniu do protokołów USB jest wykorzystywane w sprytny sposób. Przykłady to backdoor USB do hostów Air-Gapped, exploity Autorun, ukrywanie danych na urządzeniach pamięci masowej USB i inne.
- Electrical attacks -- ataki, w których urządzenia USB wysyłają impuls elektryczny po podłączeniu, co prowadzi do uszkodzenia maszyny. Przykładem tego typu ataków może być USB Killer, który niszczy urządzenie końcowe od razu po włożeniu do portu za pomocą wyładowania elektrycznego.

Za pomocą ataków USB można zrobić wiele różnych szkodliwych rzeczy, takich jak zniszczenie poufnych danych, uzyskanie dostępu do systemu lub innego typu groźne konsekwencje. Teraz należy zrozumieć, jak działają tego typu ataki. Jednym ze sposobów jest stworzenie złośliwego oprogramowania i przesłanie go do urządzenia USB. Kod można zarówno napisać samemu, jak i pobrać z sieci. Złożoność oprogramowania może być różna, zarówno prosta, jak i skomplikowana. Po podłączeniu takiego pendrive'a do urządzenia końcowego może on zostać uruchomiony, gdy użytkownik otworzy zainfekowany plik zapisany na dysku.  

Drugą prostszą techniką jest podszywanie się urządzenia USB za inne urządzenia, na przykład aby urządzenie końcowe myślało, że USB jest klawiaturą. Jest to bardzo znana i pewna metoda, dzięki której atakujący może zniszczyć poufne dane. Przykładem tego typu oprogramowania może być urządzenie Rubber Ducky, które uważa się za jedno z najpopularniejszych. Z pomocą tego narzędzia można rozpocząć wykonywanie złośliwego kodu poprzez "naciśnięcie" określonych klawiszy.

Następnie, analiza skupia się na bardziej zaawansowanych przypadkach, takich jak ataki typu BadUSB. Te ataki polegają na modyfikacji firmware urządzeń USB w taki sposób, aby urządzenie mogło emulować różne typy urządzeń wejściowych, takich jak klawiatury czy myszy, i wykonują szkodliwe działania bez wiedzy użytkownika. Przykłady te ilustrują, jak ataki na firmware mogą być wykorzystywane do wykonania zaawansowanych operacji, takich jak kradzież danych czy instalacja backdoorów \cite{11}.

#### Czym jest atak BadUSB?
Atak BadUSB polega na wykorzystaniu luki w zabezpieczeniach USB. Zazwyczaj jest tak, że odbywa się zamiana urządzenia USB w urządzenie z interfejsem człowieka. Chodzi głównie o to, żeby urządzenie USB naśladowało działania użytkownika na klawiaturze i wykonywało groźne polecenia. Atak BadUSB został stworzony przez Karsten Nohl i Jakob Lell. W dzisiejszych czasach kod BadUSB jest dostępny publicznie na repozytoriach GitHub. 

#### Jak działa BadUSB?
Atak BadUSB opiera się na zaprojektowaniu urządzenia USB w sposób programowy, który będzie mieścił w sobie złośliwe oprogramowanie. USB może łączyć się z różnymi urządzeniami, na przykład z komputerami, klawiaturami, kamerami internetowymi, modemami i innymi urządzeniami podobnego typu.

Jak wiadomo USB ma wbudowany chip, który zazwyczaj zawiera dedykowane oprogramowanie. Ten chip służy do rozpoznawania USB przez urządzenie, do których zostanie podłączony. Tego typu urządzenia są bardzo podatne na ataki ze względu na oprogramowanie, które jest łatwe do złamania. Atak taki polega na zamianie kodu poprzez metodę inżynierii wstecznej urządzenia. Istnieją różne sposoby ochrony przed tego rodzaju atakami. Jedną z najbardziej zalecanych praktyk jest wybór rozwiązania do bezpieczeństwa danych, które obejmuje szeroki zakres funkcji:
- Pliki zawierające dane osobowe PII nie mogą być kopiowane na prywatne urządzenia, takie jak urządzenia USB, ze względu na ryzyko wycieku danych.
- Wykrywanie ryzyka i złamania podejrzanego oprogramowania poprzez generowanie raportów wraz z wysyłaniem powiadomień drogą elektroniczną.
- W sytuacji wykrycia ataku przeprowadzonego przez osobę trzecią lub nieautoryzowaną, zainfekowane urządzenie końcowe zostaje izolowane od sieci, co podnosi poziom bezpieczeństwa.
- Wykrywanie anomalii w podłączonych urządzeniach do stacji roboczych w nietypowych godzinach odbywa się poprzez skanowanie wszystkich punktów końcowych. 

#### Czym jest atak typu USB drop?
Jest to bardzo nietypowa i swoją drogą trudna metoda ataku, ponieważ polega na tym, żeby ofiara sama, bez wiedzy o zagrożeniu, podłączyła zainfekowane urządzenie do swojego komputera. Ofiara może być zmylona, gdyż zainfekowane urządzenie może wyglądać na zwykły pendrive, który wydaje się niewinną ciekawostką do podłączenia. Gdy ktoś podłączy zainfekowane urządzenie do swojego komputera, które jest dodatkowo podłączone do sieci domowej, staje się potencjalną ofiarą ataku. To otwiera drogę do dostępu do urządzenia, ujawnienia poufnych danych, wpływu na sieć domową lub nawet wykonania innych działań, o ile wystarczy zasobów.

#### Jakie są rodzaje ataków USB drop?
- Social engineering -- W tym rodzaju ataków osoba atakująca podszywa się pod inną osobę w celu przeprowadzenia złośliwych działań. Może to być podszywanie się pod pracownika firmy w celu wejścia do siedziby firmy, aby podłączyć urządzenie USB w celach naszkodzić lub uzyskać dostęp do całej sieci firmowej.
- Public placement -- W tej formie ataku osoba atakująca jest przekonana, że jeśli zostawi urządzenie USB, to na pewno ktoś z pewnością weźmie go i podłączy do swojego urządzenia. Jest to atak, który często odnosi sukces, ponieważ nie wszyscy zdają sobie sprawę z ryzyka związanego z podłączaniem obcych urządzeń. W tej formie ataku osoba atakująca nie traci czasu na planowanie, a polega na tym, że znajdą się osoby, które będą dociekliwe lub nie świadome ryzyka. 

#### Jakie są cele ataków USB drop?
- Keylogging -- W tym typie ataku cel jest taki, aby urządzenie USB, które zostanie podłączone do komputera, zliczało naciśnięcia klawisz na klawiaturze ofiary i później przesłało te dane na zdalny serwer do osoby atakującej. W późniejszym czasie osoba atakująca analizuje dane, aby móc wykraść dane poufne.  
- Malware infection -- W tym typie ataku głównym celem jest uszkodzenie kluczowych informacji ofiary. Informacjami kluczowymi użytkownika mogą być dokumenty robocze, dane poufne, dokumenty zawierające dane osobiste. Osiąga się zazwyczaj tego z pomocą oprogramowania ransomware. 
- Hardware damage -- Ten typ ataku polega na uszkodzeniu sprzętu poprzez podłączenie urządzeń takich jak USBKill, które po podłączeniu do sprzętu wysyłają impuls elektryczny tym samym fizycznie niszcząc sprzęt, po czym urządzenie docelowe staje się bezużyteczne. Zazwyczaj tego typu atak jest przeprowadzany przez złośliwych insiderów, takich jak niezadowoleni pracownicy firmy lub wrodzy ofiary, które znajdują się najbliżej ofiary. 
- Human Interface Device (HID) Spoofing -- Jest to typ ataku, który w pewnej mierze jest podobny do ataku Keylogging, lecz różni się tym, że Human Interface Device (HID) Spoofing naśladuje wzorce na klawiaturze i dostaje się do wiersza poleceń, aby uzyskać zdalny dostęp bądź zakłócić obronę komputera.

#### Czym jest atak typu Tailgating?
Celem tego typu ataków jest uzyskanie dostępu do obszaru chronionego hasłem. Firmy IT lub inne przedsiębiorstwa są bardziej narażone na tego rodzaju ataki z następujących powodów:
- Ze względu na pracowników wchodzących i wychodzących z pomieszczeń, korzystających z różnych wejść do biura.
- Ze względu na podwykonawców pracujących dla firmy.
- Ze względu na nieświadomych pracowników, którzy nie zdają sobie sprawy z ryzyka związanego z bezpieczeństwem.

Aby uchronić się przed tego typu atakami należy korzystać z inteligentnych identyfikatorów i kart, które pozwalają ograniczać dostęp pracownikom do niepozwolonych miejsc. Także dobrym pomysłem będzie wdrożenie skanerów biometrycznych, które nadal uważają się za solidne urządzenia skanujące cechy fizyczne lub inne cechy osoby. Ostatnim sposobem są nadzory wideo lub CCTV oparte na sztucznej inteligencji, które można wykorzystać, aby nie tylko nagrywać, a dodatkowo analizować nagrania wideo w celach porównania z osobami, które mają pozwolenia na wejście \cite{11}.

Przykładami wszystkich powyższych rodzajów ataków mogą być zarówno duże, jak i małe firmy, które codziennie stają się ofiarami różnych ataków. Według badania przeprowadzonego w 2021 roku wśród Specjalistów Bezpieczeństwa IT około trzy na dziesięć firm odnotowało od 11 do 50 złośliwych ataków USB \cite{12}.

Jakiś czas temu znana amerykańska firma Industrial and Commercial Bank of China Ltd’s US padła ofiarą ataku za pomocą narzędzia USB. W rezultacie bank nie mógł rozliczyć kilku transakcji skarbowych w USA \cite{13}.

Ostatnio doszło do ataku na publiczne i prywatne firmy przeprowadzony przez SOGU i SNOWYDRIVE. Są to znane cyberataki, które wykorzystują narzędzia USB i są uważane za jedne z najbardziej agresywnych kampanii cyberszpiegowskich. SNOWYDRIVE jest znane z ataków na organizacje naftowe i gazowe w Azji. Jak twierdzą badacze, Rommel Joven i Ng Choon Kiat: ``Po załadowaniu SNOWYDRIVE tworzy backdoora w systemie hosta, dając atakującym możliwość zdalnego wydawania poleceń systemowych, a także rozprzestrzenia się na inne pamięci flash USB i rozprzestrzenia się w całej sieci'' \cite{14}.

Ważnym aspektem tej analizy jest również zrozumienie, jak te ataki wpływają na integralność i spójność firmware. Naruszenie spójności firmware nie tylko stanowi zagrożenie dla bezpieczeństwa danego urządzenia, ale może także prowadzić do szerszych kompromitacji systemów, na które urządzenie USB zostanie podłączone.

Rozważając dalsze implikacje, istotne jest także zrozumienie, w jaki sposób ataki te mogą wpływać na ciągłość działania organizacji i ich infrastruktury IT. Ataki te mogą prowadzić do przestojów w działaniu systemów, strat finansowych oraz uszkodzenia reputacji.

Według znanej ekspertki w dziedzinie cyberbezpieczeństwa Dr. Emily Thompson: ``ataki BadUSB uosabiają ewoluujący krajobraz zagrożeń, przed którymi stoją współczesne organizacje. Ich podstępny charakter i niezrównana zdolność adaptacji stanowią ogromne wyzwanie dla ustalonych paradygmatów cyberbezpieczeństwa''. Według powyższych słów ekspertki w dziedzinie cyberbezpieczeństwa można stwierdzić, że dziedzina cyberzagrożeń jest dynamicznie zmieniająca, co potrzebuje codziennego poznawania nowych rzeczy i konieczności wprowadzania obronnych strategii w celach zabezpieczenia na najwyższym poziomie \cite{15}. 

Dodatkowo, rozwój technologii Internetu Rzeczy (IoT) i wzrost liczby podłączanych urządzeń USB wymaga szczególnej uwagi w kontekście bezpieczeństwa. Urządzenia IoT często mają ograniczone możliwości ochrony, co sprawia, że są one łatwym celem dla ataków wykorzystujących luki w zabezpieczeniach firmware. Również należy zwrócić uwagę na pojawienie się 5G i szybki rozwój sztucznej inteligencji, które też powodują ryzyko w cyberprzestrzeni, mimo tego, że wprowadzane zostały w celach pomocnych. Ale wiadomo, gdzie rozwój tam również znajdują się luki w bezpieczeństwach.  

Z powodu rosnących zagrożeń ze strony ataków BadUSB rządy i instytucje prywatne coraz częściej wprowadzają metody obrony i różne protokoły ochrony danych. Znane instytucje takie jak RODO i CCPA wyraźnie podkreślają, że należy działać zgodnie z rekomendacjami ustalonymi z góry przez nie, ponieważ istnieje wielkie ryzyko nie stosując się tych zasad. 

Przegląd ten podkreśla konieczność stosowania zaawansowanych metod ochrony, zarówno na poziomie sprzętu, jak i oprogramowania, aby skutecznie przeciwdziałać tego rodzaju zagrożeniom. Włączenie praktyk takich jak regularne aktualizacje oprogramowania, monitorowanie ruchu sieciowego i stosowanie zasad minimalnych uprawnień może znacznie zwiększyć odporność na ataki tego typu.