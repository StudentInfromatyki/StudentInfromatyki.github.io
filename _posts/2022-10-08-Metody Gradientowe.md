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


**3. Metoda Gaussa-Seidla**
Metoda Gaussa-Seidla – iteracyjna metoda numerycznego rozwiązywania układów równań liniowych. Metoda stosowana jest głównie do rozwiązywania układów o dużej liczbie równań i niewiadomych (nawet rzędu milionów), których macierz główna jest macierzą przekątniowo dominującą. Równania tego typu występują powszechnie podczas rozwiązywania równań różniczkowych cząstkowych, np. równania Laplace’a. Dla małych układów równań dużo szybsze są metody bezpośrednie, np. metoda eliminacji Gaussa, natomiast dla ogromnych układów równań lepszą zbieżność zapewniają metody nadrelaksacyjne oraz wielosiatkowe.

**3.1. Rozwwiązanie analityczne**
W tej metodzie macierz A przedstawia się w postaci $\mathcal{A}=L+D+U$, gdzie D - macierz diagonalna, L - macierz trójkątna, zaś U - macierz trójkątna górna [1,7,8]. Wtedy układ równań $\mathcal{Ax}=b$ można przedstawić w postaci: $\mathcal{(D+L)x}=-Ux+b$.  

Zatem dla wzoru $\mathcal{Q}=D+L$. Dlatego proces iteracyjny można zapisać w postaci 
$\mathcal{\[ 
{x_{i}^{k+1}} = { \frac{1}{a_{ij}} * ( b_i - \{sum_{j=1}^{i-1} } ) }  
\]}$ 
dla $\mathcal{i}=1,2,...,n$ oraz iteracji $\mathcal{k}=0,1,...$.  

Zapis ten dobrze pokazuje rożnicę pomiędzy tą metodą iteracyjną a metoda Jacobiego. Widac, że metoda Gaussa-Seidla, wyznaczając w jednym kroku iteracyjnym klejne elementy wektora $\mathcal{x^k}$, korzysta zarówno z wartości wektora $\mathcal{x^{k+1}}$ jak i z wyznaczonych juz elementów wektora $\mathcal{x^k}$. W tej metodzie Jaobiego natomiast nowe przybliżenia składowych rozwiązania wykorzystywane są dopiero w kolejnej iteracji, dzięki czemu mozna je obliczać jednocześnie. 

Kryterium zbieżności metody Gaussa-Seidla jest takie samo jak dla metody Jacobiego, co pokazuje poniższe twierdzenie: Jeśli macierz A jest dominująca przekątniowo, to metoda Gaussa-Seidla jest zbieżna dla dowolnego wektora początkowego.