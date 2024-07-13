[Kliknij tutaj, aby zobacyć pracę](https://github.com/Danchivskyi/Master-s-Dissertation/blob/main/Praca_dyplomowa_magisterska.pdf)


# Spis treści
[1. Wprowadzenie](#1-wprowadzenie) 

[1.1. Cel i zakres pracy](#11-cel-i-zakres-pracy) 

[2. Krytyka teorii: wyzwania w pracy badawczej](#2-Krytyka-teorii-:-wyzwania-w-pracy-badawczej) 

[2.1. Geneza i ewolucja ataków USB](#21-Geneza-i-ewolucja-atakow-USB) 

[2.1.1. Kluczowe pojęcia](#211-Kluczowe-pojecia) 

[2.2. Analiza przypadków i ich wpływ na firmware](#22-Analiza-przypadkow-i-ich-wplyw-na-firmware) 

[2.2.1. Czym jest atak USB?](#221-Czym-jest-atak-USB?) 

[2.3. Aspekty techniczne i prawne bezpieczeństwa firmware](#23-Aspekty-techniczne-i-prawne-bezpieczeństwa-firmware) 

[2.3.1. Analiza techniczna firmware](#231-Analiza-techniczna-firmware) 

[2.3.2. Aspekty prawne](#232-Aspekty-prawne) 

[2.3.3. Synergia technicznych i prawnych aspektów](#233-Synergia-technicznych-i-prawnych-aspektów) 

[3. Zastosowanie i analiza technik badUSB](#3-Zastosowanie-i-analiza-technik-badUSB) 

[3.1. Badanie zaawansowanych technik badUSB](#31-Badanie-zaawansowanych-technik-badUSB) 

[3.2. Technika ataków badUSB](#32-Technika-ataków-badUSB) 

[3.3. Analiza bezpieczeństwa systemów przed atakami badUSB](#33-Analiza-bezpieczeństwa-systemów-przed-atakami-badUSB) 

[3.4. Ataki ukierunkowane na system operacyjny i BIOS](#34-Ataki-ukierunkowane-na-system-operacyjny-i-BIOS) 

[3.4.1. Kontynuacja skryptu](#341-Kontynuacja-skryptu) 

[3.5. Sprzętowe podatności](#35-Sprzętowe-podatności) 

[4. Wyniki](#4-Wyniki) 

[4.1. Analiza danych](#41-Analiza-danych) 

[5. Dyskusja](#5-Dyskusja) 

[5.1. Podsumowanie i wnioski końcowe](#51-Podsumowanie-i-wnioski-końcowe) 

[Streszenie](#Streszenie) 

[A. Szczegółowe wyniki badań](#A-Szczegółowe-wyniki-badań) 

[B. Kod źródłowy](#B-Kod-źródłowy) 


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

# 2.3. Aspekty techniczne i prawne bezpieczeństwa firmware

Firmware, będąc nieodłącznym elementem urządzeń elektronicznych, odgrywa kluczową rolę w zapewnieniu ich poprawnego funkcjonowania. Jednakże, ta sama niezbędność czyni firmware atrakcyjnym celem dla cyberataków. Rozumienie technik analizy firmware jest krytyczne w identyfikowaniu i zapobieganiu takim atakom.

# 2.3.1. Analiza techniczna firmware

W dzisiejszych czasach analiza techniczna firmware jest ważnym czynnikiem procesu audytu bezpieczeństwa. Podczas tego procesu wykorzystywane są różne metody i narzędzia umożliwiające oceniania bezpieczeństwa firmware'u. 

Analiza firmware'u z punktu widzenia technicznego odbywa się na kilka faz. Pierwszą z nich jest odnalezienie samego firmware'u, aby móc przeprowadzić odpowiednie badania na nim. Kolejnym krokiem jest rozpakowanie i dekompilacja, aby mieć dostęp do kodu źródłowego. Ten krok potrzebuje zastosowania odpowiednich narzędzi i technik reverse engineering. Poniżej przedstawione techniki, które pomagają przeprowadzić odpowiednią analizę:  
- Inżynieria wsteczna: Ta metoda pozwala na analizowanie firmware poprzez rozkładanie skompilowanego kodu na jego pierwotne składniki. Jest to szczególnie przydatne w identyfikowaniu ukrytych funkcji lub potencjalnych luk bezpieczeństwa.
- Deasemblacja: Polega na konwersji kodu maszynowego na formę bardziej zrozumiałą dla człowieka. Deasemblacja jest niezbędna w zrozumieniu dokładnych działania i potencjalnych słabości firmware.
- Testowanie penetracyjne: Przeprowadzanie kontrolowanych ataków w celu identyfikacji słabych punktów w firmware, co pozwala na wzmocnienie jego odporności na potencjalne zagrożenia.

Podczas analizy technicznej firmware'u wykorzystywane są zarówno metody analizy statycznej, jak i dynamicznej. Analiza statyczna polega na skanowaniu kodu, który został użyty w procesie firmware. Analiza statyczna obejmuje poszukiwanie wzorców i błędów kodowania, odwołania do nieistniejących funkcji czy przepełnienia bufora. Jest to sposób, który uważa się za nieco trudniejszy z tej racji, że jest manualny. Z kolei analiza dynamiczna polega na uruchomieniu firmware'u w sandboxach lub jak inaczej są nazywane środowiska kontrolowane. Pozwala to na obserwację podatności w czasie rzeczywistym. 

Ważnym elementem analizy jest zrozumienia procesu, technik szyfrowania, maskowania czy kompresji. Również ważnym elementem jest poznanie architektur procesu, narzędzi wykorzystujących do analizy i coraz bardziej zaawansowane techniki zabezpieczeń stosowane przez dostawców. Dlatego też istotne jest ciągłe doskonalenie metod i narzędzi używanych do audytu firmware'u, aby zapewnić skuteczną ochronę przed zagrożeniami związanymi z oprogramowaniem wbudowanym \cite{17}.

# 2.3.2. Aspekty prawne

W dzisiejszych czasach, gdzie świat IT dość szybko się rozwija, potrzebna również jest pewna biegłość w zakresie prawnym, aby uniknąć działań, których później będziemy żałować. Twierdząc z poprzedniego zdania należy zrozumieć kiedy można używać narzędzia lub oprogramowania znalezionego w Internecie, kiedy można modyfikować go, a kiedy nie. W kontekście prawno-technicznym, BadUSB stawia przed nami wiele problemów, zarówno w zakresie identyfikacji, jak i egzekwowania odpowiedzialności za tego typu działania.

Ważnym aspektem w zakresie prawnym BadUSB jest ocena odpowiedzialności podmiotów za tego typu ataki. W sytuacji tradycyjnych prawnych systemów ciężko sklasyfikować prawny aspekt przy użyciu ataków BadUSB. Mimo tego pierwszym krokiem, który jest niezbędny dla oceny, jest sprawdzenie kto jest odpowiedzialny. Czy winę ponosi producent zainfekowanego urządzenia, użytkownik, który podłączył zainfekowany pendrive do swojego komputera, czy może osoba odpowiedzialna za stworzenie złośliwego oprogramowania? 

Kolejnym krokiem jest kwestia dotycząca ochrony danych osobowych i poufności informacji. Podczas ataku tego typu, dane przechowywane na urządzeniach różnego typu, serwerach itp. mogą być narażone na kradzież lub manipulację. W związku z tym konieczne jest dokładne zapoznanie się z przepisami dotyczącymi ochrony danych osobowych (RODO) oraz konsekwencjami prawnymi naruszenia tych regulacji.

Ataki BadUSB przy użyciu urządzeń USB mogą prowadzić do naruszenia przepisów RODO na kilka sposobów. Pierwszym aspektem jest nieuprawniony dostęp do danych osobowych, co powoduje do poważnych naruszeń zasad poufności i integralności danych. Zgodnie z przepisami które zawarte w RODO, jednostki przetwarzające dane osobowe muszą zapewniać odpowiedni poziom bezpieczeństwa tych danych, aby chronić te dane przed różnymi typu wyciekami oraz nieuprawnionym dostęp. Drugim aspektem jest wymóg na przetwarzanie danych osobowych. Zgodnie z przepisami dotyczącymi ochrony danych osobowych, przetwarzanie danych osobowych jest dopuszczalne tylko wtedy, gdy osoba, której dane dotyczą, wyraziła na to zgodę, lub gdy istnieje inna podstawa prawna umożliwiająca tego typu przetwarzanie.

Dodatkowo, ataki BadUSB mogą prowadzić do naruszenia zasady odpowiedzialności określonej w RODO. Zgodnie z tą zasad jednostki przetwarzające dane osobowe są odpowiedzialne za przestrzeganie przepisów RODO i muszą być w stanie wykazać zgodność z nimi poprzez stosowanie odpowiednich środków technicznych i organizacyjnych. W sytuacji ataków BadUSB organizacje muszą podejmować odpowiednie kroki, aby monitorować i zapobiegać tego typu atakom \cite{18}:
- Przepisy o ochronie danych: Przepisy takie jak GDPR nakładają na organizacje odpowiedzialność za ochronę danych przetwarzanych przez firmware urządzeń. Naruszenia tych przepisów mogą prowadzić do poważnych konsekwencji prawnych i finansowych.
- Standardy i regulacje branżowe: Istnieją różne standardy, takie jak ISO/IEC 27001, które określają wymagania dotyczące systemów zarządzania bezpieczeństwem informacji, w tym bezpieczeństwa firmware.
- Wyzwania związane z licencjonowaniem i prawami autorskimi: W kontekście inżynierii wstecznej firmware, istotne jest zrozumienie ograniczeń nałożonych przez prawa autorskie i licencje, aby unikać naruszania praw twórców oprogramowania.

# 2.3.3. Synergia technicznych i prawnych aspektów

Zrozumienie technicznych aspektów bezpieczeństwa firmware jest nierozerwalnie związane z przestrzeganiem przepisów prawa. Skuteczna ochrona firmware wymaga nie tylko zaawansowanej wiedzy technicznej, ale także znajomości i stosowania odpowiednich przepisów prawnych. Taka synergia pozwala na tworzenie kompleksowych strategii ochrony, które są zarówno technicznie wydajne, jak i zgodne z obowiązującymi regulacjami.

Dodatkowo, wzrasta znaczenie analizy zagrożeń związanych z łańcuchem dostaw firmware. Ataki takie jak SolarWinds wykazały, że nieautoryzowane modyfikacje firmware przez złośliwe podmioty mogą mieć dalekosiężne skutki na szeroko rozumiane bezpieczeństwo narodowe i infrastrukturę krytyczną. Analiza ryzyka w łańcuchu dostaw staje się nieodzownym elementem zarządzania bezpieczeństwem firmware, wymagając od organizacji i instytucji szczegółowej oceny potencjalnych zagrożeń i implementacji skutecznych strategii ich minimalizowania.

W tym kontekście, rośnie także rola narzędzi do zarządzania firmware i bezpieczeństwa urządzeń końcowych. Zastosowanie zaawansowanych rozwiązań do zarządzania firmware, takich jak systemy wykrywania i odpowiedzi na incydenty (EDR), pozwala na bieżącą kontrolę stanu firmware i szybką reakcję na potencjalne zagrożenia. Wspiera to strategie proaktywnego zarządzania ryzykiem i wzmacnia ogólne bezpieczeństwo systemów informatycznych.

# 3. Zastosowanie i analiza technik badUSB

# 3.1. Badanie zaawansowanych technik badUSB

BadUSB należy do rodzaju ataków, które wykorzystują zaufanie użytkowników do urządzeń USB, z pomocą których atakujący mogą naruszyć bezpieczeństwo systemów. Zazwyczaj osoby atakujące manipulują oprogramowaniem sprzętowym urządzeń USB, aby te urządzenia wdawały się w urządzenia innego typu, co pozwala im na wykonywanie złośliwych działań względem zaufanych urządzeń. Oto omówienie zaawansowanych technik i narzędzi badUSB powszechnie używanych w atakach takiego typu:

- Firmware Manipulation: Ataki typu BadUSB zazwyczaj polegają na zmianie oprogramowania sprzętowego urządzeń USB w celu zmiany ich codziennego zachowania. Przy użyciu specjalistycznych narzędzi atakujący mogą manipulować oprogramowaniem sprzętowym wykorzystując zaufanie użytkowników do urządzeń USB w celu naruszenia bezpieczeństwa systemów. Do tego typu ataków można zaliczyć takie narzędzia jak USBProxy i FaceDancer. Służą one do przechwytywania i modyfikowania ruchu USB, dodatkowo umożliwiając atakującym wstrzykiwanie złośliwych payloads do urządzeń USB.
- Emulation of HID Devices: Jedna z kolejnych powszechnych technik badUSB, która polega na emulowaniu takich urządzeń jak klawiatury, myszy, głośniki. Przeprogramowuje urządzenia w ten sposób, aby działały jako nośnik złośliwego oprogramowania, czyli aby po kliknięciu klawisza na klawiaturze odbył się atak. Narzędzia takie jak Rubber Ducky i MalDuino przedstawiają ten atak umożliwiając atakującym tworzenie payloads wykonujących polecenia w systemie ofiary po podłączeniu złośliwego urządzenia USB.
- Data Exfiltration: Ten typ ataku polega na modyfikowaniu urządzeń USB tak, aby działały jako urządzenia pamięci masowej lub karty sieciowe. Po podłaczeniu urządzenia do atakowanego systemu złośliwe oprogramowanie może pobrać poufne dane lub połączyć się z serwerami zewnętrznymi. Takie ataki przedstawiane przez takie narzędzia jak USB Rubber Dumper i USBHarpoon, które ułątwiają proces eksfiltracji danych, automatyzując proces kopiowania danych z systemu ofiary na serwer atakującego.
- Firmware Implants: W niektórych sytuacjach osoba atakująca może wstrzyknąć złośliwe oprogramowanie bezpośrednio na urządzenia USB podczas ich tworzenia, co może prowadzić do poważnych skutków, takich jak zainfekowania dużej liczby urządzeń, które póżniej mogą być szeroko rozpowszechniane. Podobne oprogramowanie jest trudne do wkrycia i usunięcia, co sprawia, że są one szczególnie niebezpieczne. Narzędzia takie jak USBKill i USBStealer służą do tworzenia takiego oprogramowania sprzętowego na urządzeniach USB.
- Persistent Payloads: Ataki badUSB mogą zawierać różne formy, zaczynając się od włączenia w to generowanych payloads-ów, które mogą zostać na zainfekowanym urządzeniu nawet po wielokrotnych uruchomieniach systemu. Poprzez przechowywanie złośliwego kodu w oprogramowaniu sprzętowym urządzeń USB osoba atakująca może zapewnić, że payloads wykonany przez niego może pozostać aktywny nawet po początkowej infekcji systemu. Takim przykładem moga być takie narzędzia jak BadUSB Firmware Patch i USB Persistent Payload Generatorm, które służą do tworzenia złośliwych payloads-ów.
- Cross-Platform Attacks: Tego typu ataki nie ograniczają się do konkretnego systemu operacyjnego lub platformy. Oosoby atakujące mogą tworzyć złośliwe payloads na systemy Windows, macOS, Linux i inne systemy operacyjne. Pozwala to złamać zabezpieczenia systemu za pomocą jednego złośliwego urządzenia USB. Narzędzia takie jak BadUSB Cross-Platform Exploit Framework (BadUSB-CPF) zapewniają wieloplatformowe możliwości tworzenia i wdrażania payloads badUSB.

# 3.2. Technika ataków badUSB

Nie wszystkie złośliwe urządzenia USB muszą być drogimi elementami sprzętu z zaawansowanym programowaniem, aby zaszkodzić komputerowi lub innemu urządzeniu. Takimi przykładami drogich rozwiązań mogą być Flipper Zero, Rubber Ducky, Malduino, Digispark. Za pomocą starego pendrive'a można zbudować własny złośliwy BadUSB, korzystając z plików skrótów złośliwych oprogramowań napisanych w Bash, CMD lub PowerShell

Zgodnie z wpisem na blogu ``Rise of LNK (Shortcut files) Malware'' okazuje się, że w drugim kwartale 2022 roku McAfee Labs zanotowało wzrost infekcji złośliwym oprogramowaniem dostarczanym za pomocą plików LNK. Atakujący wykorzystują łatwość użycia plików LNK do dostarczania złośliwego oprogramowania, takiego jak Emotet, Qakbot, IcedID, Bazarloaders itp.

W tej części pracy zostanie pokazane jak plik LNK może dostarczać złośliwe oprogramowanie na pozornie niewinnie wyglądającym pendrive'ie USB. Poprzez wykorzystanie trudno wykrywalnego oprogramowania złośliwego do plików skrótów systemowych Windows, ukryty odnośnik zmanipuluje użytkownika, aby kliknął na pozornie nieszkodliwy plik i uruchomił oprogramowanie złośliwe. Skrót pliku zapewnia szybki i łatwy dostęp do plików wykonywalnych bez konieczności nawigowania przez pełną ścieżkę programu. W tej sytuacji plik wykonywalny ze złośliwym  oprogramowaniem może znajdujować się w ukrytym katalogu, choć to nie jest konieczne. Użytkownik klika na folder, który zawiera odnośnik do pliku wykonywalnego uruchamiając w ten sposób oprogramowanie złośliwe. Plik, który zostanie wykorzystywany w tym ataku to Netcat lub inaczej tak jak jest nazwany nc64.exe, który został pobrany z repozytorium na GitHub (Rys.~\ref{fig:my_image1}).

<p align="center">
  Rys.3.1. Repozytorium na GitHub
<br>
  <img src="\assets\img\MasterThesis\1.png" width="650" alt="GitHub">
  <br>
</p>   

Aby pobrać złośliwe oprogramowanie Netcat należy wyłączyć ochronę w czasie rzeczywistym w Microsoft Defender co potwierdza, że to zabezpieczenie w Windows jednak jest na wysokim poziomie (Rys.~\ref{fig:my_image2}).

Ten rodzaj ataku stwarza niebezpieczeństwo nie tylko poprzez możliwość infekcji jednego urządzenia, ale także przez potencjalne rozprzestrzenianie się złośliwego kodu poprzez zainfekowane urządzenia, które mogą być szeroko rozpowszechniane w sieci. W rezultacie nawet pozornie nieszkodliwe urządzenia USB mogą stanowić istotne zagrożenie dla całego ekosystemu informatycznego.

<p align="center">
  Rys.3.2. Wyłączenie ochrony w Microsoft Defender
<br>
  <img src="\assets\img\MasterThesis\2.png" width="650" alt="Defender">
  <br>
</p>   

W tym celu należało posiadać pendrive, który zostanie skonfigurowany jako złośliwy. Rozmiar plików nie będzie duży, więc powinien działać na każdym pendrive. Po czym trzeba utworzyć jeden folder główny nazwany jako payload directory, w którym będą skrypty i plik Netcat (Rys.~\ref{fig:my_image3}). A drugi folder to jest właśnie skrót folderu utworzony na podstawie folderu głównego. 

<p align="center">
  Rys.3.3. Wygląd zawartości folderu
<br>
  <img src="\assets\img\MasterThesis\3.png" width="650" alt="folderu">
  <br>
</p>  

Częścią sukcesu tego ataku jest utworzenie skrótu systemowego Windows i odnośnika do złośliwego oprogramowania w ukrytym katalogu. Jest to robione, aby skłonić użytkownika do kliknięcia w złośliwe oprogramowanie nie widząc w co klika. W celu lepszej widoczności badań nie ukryto folderu. 

Po skopiowaniu nc64.exe na pendrive należy dokonać kilku zmian w systemie plików urządzenia, zaczynając od utworzenia pliku głównego tak zwanego skryptu. Po wpisaniu kodu należy zapisać go z odpowiednim rozszerzeniem. Katalog payload powinien zawierać dwa pliki: plik wykonywalny i plik wsadowy. Aby przetestować ogólne działanie został napisany prosty skrypt, który wyświetla "Hello, World!" w wierszu poleceń (Rys.~\ref{fig:my_image4})

<p align="center">
  Rys.3.4. Skrypt wyświetlający odpowiednie polecenie
<br>
  <img src="\assets\img\MasterThesis\4.png" width="650" alt="folderu">
  <br>
</p>  

Na początku zostanie przetestowane, jak działa skrypt bez wykrywania zagrożeń w Windows Defender. Badania zostały przeprowadzone na sprzęcie testowym i w tym celu wyłączono wszystkie ochrony w Microsoft Defender (Rys.~\ref{fig:my_image5}).

<p align="center">
  Rys.3.5. Wyłączenie ochrony w Microsoft Defender
<br>
  <img src="\assets\img\MasterThesis\5.png" width="650" alt="folderu">
  <br>
</p>  

Po uruchomieniu pliku można zauważyć, że operacja zakończyła się powodzeniem, co potwierdza poprawne wykonanie zadania. Ten wynik jest szczególnie zadowalający, biorąc pod uwagę skomplikowany charakter procesu oraz wymagające warunki, jakie należało spełnić. Wszystkie kroki zostały wykonane z należytą starannością i precyzją, co przyczyniło się do osiągnięcia oczekiwanych rezultatów (Rys.~\ref{fig:my_image6}).

<p align="center">
  Rys.3.6. Prezentacja wyników
<br>
  <img src="\assets\img\MasterThesis\6.png" width="650" alt="folderu">
  <br>
</p>  