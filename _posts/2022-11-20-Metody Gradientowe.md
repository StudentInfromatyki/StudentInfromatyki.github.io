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

**4. Implementacja metody Jacobiego, Gaussa-Seidla oraz SOR i gradientów spężonych**
W tym punkcie dokonamy implementacji metody Jacobiego, Gaussa-Seidla, oraz SOR i gradientów sprężonych, a nastepnie rozwiążemy przy ich pomocy zadany układ równań. Sprawdzimy poprawność obliczeń odręcznych. 

**4.1. Implemetacja metody Jacobiego**

~~~
function[xx,kk] = f_jacobi(A,b, k_max, tol)

n = length(b);
C = zeros(n,l);
D = zeros(n,n);

for ii = 1:n
    C(ii) = b(ii)/A(ii,ii);
    for jj = 1:n
    if(ii~=jj)
        D(ii,jj) = -A(ii,jj)/A(ii,ii);
    endif
    endfor
endfor

xx=C;
    for kk = 1:k_max
    xx = C + D*xx;
    bk = A*xx;
    blad = abs(bk-b);
    suma = sum(blad);
    if(suma<tol) break;
    endif
    endfor
endfunction
~~~


**4.2. Implementacja metody Gaussa-Seidla**
~~~
function[x, Ar] = f_gauss(A,b)

[n,m] = size(A);

if(n~=m), error('Macierz A musi byc kwadratowa');
endif

Ar = [A,b];
x = zeros(n,1);
for kk = 1:(n-1)
    for jj = (kk+1):(n+1)
        for ii = (kk+1):n
        Ar(ii,jj) = Ar(ii,jj)-(Ar(ii,kk)*Ar(kk,jj)/Ar(kk,kk));
        endfor
    endfor
endor

for ii = n:-1:1
    suma = 0;
    for jj = (ii+1):n
        suma = suma + Ar(ii,jj)*x(jj);
    endfor
    x(ii) = (1/Ar(ii,ii))*(Ar(ii,n+1)-suma);
endfor
endfunction
~~~

**4.3. Implementacja metody SOR**
~~~
function[x,info,iter,resid] = sor(A,b,omega=1,tol=1e-10,maxit=1000,x0)

if(nargin < 6)
    x0 = zeros(size(b));
end

resid = zeros(maxit,1);
iter = 1;
x = x0;
resid(iter) = norm(b - A*x);
M = tril(A,-1) + spdiag(diag(A)/omega);
Z = spdiag((1/omega - 1)*diag(A)) - triu(A,1);

while((resid(iter) > tol*resid(1)) && (info = (iter < maxit)))
    x = M \ (Z*x + b);
    iter = iter + 1;
    resid(iter) = norm(b - A*x);
end
end
~~~

**4.4. Implemetacja metodą gradientów sprężonych**
Jeśli właściwie dobierzemy sprzężone wektory $\mathcal{p_k}$, możemy nie potrzebować ich wszystkich do dobrej aproksymacji rozwiązania $\mathcal{x_*}$ Możemy więc spojrzeć na CG jak na metodę iteracyjną. Co więcej, pozwoli nam to rozwiązać układy równań, gdzie n jest tak duże, że bezpośrednia metoda zabrałaby zbyt dużo czasu. 

Oznaczmy punkt startowy przez $\mathcal{x_0}$. Bez starty ogólności możemy założyć, że $\mathcal{x_0}=0$ (w przeciwnym przypadku, rozważymy układ $\mathcal{Az}=b-Ax_0$. Zauważmy, że rozwiązanie $\mathcal{x_*}$ minimalizuje formę kwadratową: $\mathcal{f(x)}=\frac{1}{2} * x^T * Ax - b^T * x$.

Co sugeruje, by jako pierwszy wektor bazowy $\mathcal{p_1}$ wybrać gradient f w $\mathcal{x}=x_0$, który wynosi $\mathcal{Ax_0}-b$, a ponieważ wybraliśmy $\mathcal{x}=x_0$, otrzymujemy -b. Pozostałe wektory w bazie będą sprężone do gradientu (stąd nazwa metoda gradientu sprężonego).

Niech $\mathcal{r_k}$ oznacza rezyduum w k-tym kroku: $\mathcal{r_k}=b-Ax_k$.

Zauważmy, że $\mathcal{r_k}$ jest przeciwny do gradientu f w $\mathcal{x}=x_k$, więc metoda gradientu prostego nakazywałaby ruch w kierunku $\mathcal{r_k}$. Tutaj jednak założyliśmy wzajemną sprężoność kierunków $\mathcal{p_k}$, więc wybieramy kierunek najbliższy do $\mathcal{r_k}$ pod warunkiem sprężoności. Co wyraża się wzorem: 
$\mathcal{p_{k+1}}=r_k - \frac{p_k^T * Ar_k}{p_k^T * Ap_k} * p_k$


~~~
function[x] = conjgrad(A,b,x0)

r = b - A*x0;
w = -r;
z = A*w;
a = (r'*w)/(w'*z);
x = x0 + a*w;

for i = 1:size(A,1);
    r = r - a*z;
    if(norm(r) < 1e-10)
        break;
    end
    B = (r'*z)/(w'*z);
    w = -r + B*w;
    z = A*w;
    a = (r'*w)/(w'*z);
    x = x + a*w;
    end
end
~~~

**5. Porównanie wyników czterech powyższyh metod**
Algorytmy przetestowano o rozmiarze N=100. Jeśli zależność czasu obliczeń t od rozmiaru macierzy N jest funckją potęgową typu $\mathcal{t(N)}=aN^B$, to po zlogarytmowaniu tego równania stronami mamy $\mathcal{log t(N)}=B log(N)+log(a)$.

| Metoda iteracyjna| Wykładnik B | 
| :------ |:--- |
| Jacobiego | 3.58 |
| Gaussa-Seidla | 3.17 |
| SOR | 3.38 |
| Gradientów spręzonych | 3.04 |

Z tej racji najmniej czasu na wykonanie algorytmu potrzebno dla metody gradientów sprężonych, potem dla metody GaussaSeidla, na trzecim miejscu znajduje się metoda SOR, a najdłuższą metodą z tych czterech jest metoda Jacobiego.


**5.1. Porównanie dokładności**
Na mój pogląd najdokładniejszą metodą jest metoda Gaussa – Seidla. Dlatego, że metoda Gaussa – Seidla jest metodą relaksacyjną, w której
poszukiwanie rozwiązania rozpoczyna się od dowolnie wybranego rozwiązania próbnego $\mathcal{x^0}$, po czym w kolejnych krokach, zwanych iteracjami, za pomocą prostego algorytmu zmienia się kolejno jego
składowe, tak by coraz lepiej odpowiadały rzeczywistemu rozwiązaniu.
Metoda Gaussa – Seidla bazuje na metodzie Jacobiego, w której krok
iteracyjny zmieniono w ten sposób, by każda modyfikacja rozwiązania
próbnego korzystała ze wszystkich aktualnie dostępnych przybliżonych
składowych rozwiązania. Pozwala to zaoszczędzić połowę pamięci operacyjnej i w większości zastosowań praktycznych zmniejsza około
dwukrotnie liczbę obliczeń niezbędnych do osiągnięcia zadanej dokładności rozwiązania. 

**5.2. Dokonanie analizy wyników**
Każda metoda polega na odnajdywaniu przybliżenia rozwiązania z zadaną
dokładnością. Oczywiste jest to, że implementacja zawsze jest dokładniejsza od wyznaczenia przybliżenia na kartce. Wynika to z tego powodu, iż na kartce obliczamy ręcznie i jest łatwiej dokonać błędu. W implementacji możemy wyznaczyć z którą chcemy dokładnością i wyniki będą poprawne i można będzie sprawdzić czy dobrze mamy obliczono na kartce, pacząc na implementację i to jest wielka zaleta implementacji.

Także dane nam cztery metody różnią się, dlatego że każda metoda jest
obliczana inaczej i niektóre metody są efektywniejsze od innych. Jedną z
najprostszych metod iteracyjnych jest metoda iteracji prostej. Polega ona na przejściu od danego układu równań liniowych do równoważnego układu: $\mathcal{x}=Bx+c$