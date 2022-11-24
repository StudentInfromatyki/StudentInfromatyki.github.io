---
layout: post
title: Iteracje metodą Jacobiego oraz Gaussa-Seidla
subtitle: Metody numeryczne
cover-img: /assets/img/geometry.jpg
thumbnail-img: /assets/img/menuin.jpg
share-img: /assets/img/geometry.jpg
tags: [metody numeryczne, Jacobiego, Gaussa-Seidla, iteracje]
---

**1. Wstęp**

Zaletą metod iteracyjnych jest możliwość wyznaczenia przybliżenia rozwiązania z zadaną dokładnością, niekiedy kosztem istotnie mniejszym od kosztu metod skończonych. Dla niektórych zadań metody iteracyjne są więc efektywniejsze. Jedną z najprostszych metod iteracyjnych jest metoda iteracji prostej. Polega ona na przejściu od danego układu równań liniowych do równoważnego (tzn. mającego te same rozwiązania) układu: $\mathcal{x}=Bx+c$.

**2. Metoda Jacobiego**
Metoda Jacobiego jest metodą iteracyjną i pozwala nam obliczyć układ n równań z n niewiadomymi $\mathcal{Ax}=b$.


**2.1 Rozwiązanie analityczne:**

$\mathcal{
f(x)=\left\{ \begin{array}{lr} x+1 & dla \ x\in(-\infty;0) \\ x-1 & dla \ x\in\langle0;+\infty) \end{array}\right
}$

1. Przyjąć punkt startowy $\mathcal{x_0}$, $\mathcal{C^2}$.długość kroku e, współczynnik redukcji kroku 𝒂 < 𝟏, limit liczby redukcji kroku k (np. 𝒌 = 𝟓) i dokładność wyznaczenia ekstremum (zerowania się gradientu) ε (np. $\mathcal{ε}={10^-3}$).
2. Obliczyć w punkcie $\mathcal{x_i}$ wartość funkcji celu $\mathcal{f(x_i)}$ i jej gradientu $\mathcal{g(x_i)}$.
3. Wyznaczyć kierunek poszukiwań przeciwny do kierunku gradientu $\mathcal{d}={-g(x_i)}$.
4. Wykonać z punktu $\mathcal{x_i}$ krok o długości e w wyznaczonym kierunku d, przechodząc do punktu $\mathcal{x_i+1}={x_i+e*d}$.
5. Obliczyć wartość funkcji celu. Jeśli $\mathcal{f(x_i+1)}>={f(x_i)}$ , dokonać redukcji kroku (mnożąc jego wartość przez a) i ponowić próby. Po k niepomyślnych próbach zakończyć postępowanie.
6. Obliczyć wartość gradientu w nowym punkcie $\mathcal{g(x_i+1)}$. Jeśli $\mathcal{|g^T*g|>ε}$, przyjąć 𝒊 = 𝒊 + 𝟏 i przejść do
punktu 2. W przeciwnym razie zakończyć postępowanie.


**3. Metoda najszybszego spadku**
Metoda najszybszego spadku stanowi modyfikację metody gradientu prostego. W metodzie
najszybszego spadku po określeniu kierunku poszukiwań wyznaczane jest minimum funkcji w tym
kierunku, a nie przesunięcie ze stałym krokiem. Ważną własnością metody najszybszego spadku jest to, że
przy jej zastosowaniu każdy nowy kierunek poruszania się ku optimum jest ortogonalny do poprzedniego.
Tłumaczy się to tym, że poruszanie się w jednym kierunku trwa do tego czasu, dopóki kierunek ten nie
okaże się stycznym do jakiejś linii stałej wartości funkcji celu.

![Photo](https://upload.wikimedia.org/wikipedia/commons/thumb/a/ab/Metoda_najszybszego_spadku.svg/1280px-Metoda_najszybszego_spadku.svg.png)


**Algorytm metody najszybszego spadku:**
1. Przyjąć punkt startowy $\mathcal{x_0}$, i dokładność wyznaczenia ekstremum (zerowania się gradientu) ε (np. $\mathcal{ε}={10^-3}$).
2. Obliczyć w punkcie $\mathcal{x_i}$ wartość funkcji celu $\mathcal{f(x_i)}$ i jej gradientu $\mathcal{g(x_i)}$.
3. Wyznaczyć kierunek poszukiwań przeciwny do kierunku gradientu $\mathcal{d}={-g(x_i)}$.
4. Wykonać z punktu $\mathcal{x_i}$ krok w wyznaczonym kierunku d, o takiej długości e, by osiągnąć minimum w tym kierunku, przechodząc do punktu $\mathcal{x_i+1}={x_i+e*d}$.
5. Obliczyć wartość funkcji celu i jej gradientu w nowym punkcie.
6. Jeśli $\mathcal{g^T*g>ε}$, przyjąć 𝒊 = 𝒊 + 𝟏 i przejść do punktu 2. W przeciwnym razie zakończyć postępowanie.

**Uwaga**
W punkcie 4. powyższego algorytmu należy rozwiązać zadanie optymalizacji funkcji jednej zmiennej min $\mathcal{f(e)=f(x_i+e*d)}$. Do utworzenia funkcji 𝑓(𝑒) wygodnie jest się posłużyć poleceniem matlabFunction, które pozwala na przekształcenie wyrażenia symbolicznego w funkcję anonimową. 

Do obliczania minimum funkcji 𝑓(𝑒) zastosować można jedną z metod poszukiwania minimum funkcji jednej zmiennej, które zostały zaimplementowane na poprzednim laboratorium. Niektóre z tych metod wymagają wyznaczenia przedziału, na którym spodziewamy się znaleźć minimum. W tym celu skorzystać można z heurystycznej metody opracowanej przez W. Swanna, według której (k+1) punkt określa się z rekurencyjnego wzoru:
$\mathcal{x_k+1}={x_k+2^k*\bigtriangleup}$, 𝑘 = 0,1,2,3, … , 𝑙

gdzie: 

$\mathcal{x_0}$ - punkt początkowy
$\mathcal{\bigtriangleup}$ – długość kroku (stała, np. $\mathcal{\bigtriangleup}={10^-2}$.

Znak $\mathcal{\bigtriangleup}$ określa się drogą porównań wielkości $\mathcal{f(x_0)+\bigtriangleup}$ i $\mathcal{f(x_0)-\bigtriangleup}$. Jeżeli $\mathcal{f(x_0)-\bigtriangleup}>{f(x_0)+\bigtriangleup}$, to zgodnie z założeniem o wypukłości w dół, punkt minimum powinien się znajdować na prawo od punktu $\mathcal{x_0}$ i wielkość $\mathcal{\bigtriangleup}$ powinna być wybierana jako dodatnia. Jeżeli zmienić znak nierówności na przeciwny, to $\mathcal{\bigtriangleup}$ należy wybrać jako wielkość ujemną. Jeżeli $\mathcal{f(x_l)}>={f(x_0)}$, to punkt minimum leży między $\mathcal{f(x_0)}$ i $\mathcal{f(x_l)}$ i poszukiwanie punktów granicznych zostaje zakończone.