[Kliknij tutaj, aby zobacyć pracę](https://github.com/Danchivskyi/Master-s-Dissertation/blob/main/Praca_dyplomowa_magisterska.pdf)


# Spis treści
[1. Wprowadzenie](#1-wprowadzenie) 

[1.1. Cel i zakres pracy](#11-cel-i-zakres-pracy) 

[2. Krytyka teorii: wyzwania w pracy badawczej](#2-Krytyka-teorii-:-wyzwania-w-pracy-badawczej) 


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