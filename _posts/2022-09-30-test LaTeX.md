---
layout: post
title: Test LaTeX 
subtitle: Test for me
cover-img: /assets/img/LaTeX_logo.svg.png
thumbnail-img: /assets/img/LaTeX_cover.png
share-img: /assets/img/LaTeX_logo.svg.png
tags: [lalala, test]
---

## Tryb inline - wersja z $
Słynne równanie Albert Einsteina, to $\mathcal{E}=mc^2$

Odkryte zostało w 1905.

## Indeksy górne i dolne
Indeks dolny definiowany jest za pomocą kreski podkreslenia _.

Indeks górny definiowany jest za pomocą daszka ^.

$\mathcal{[ \int_0^1 x^2 + y^2 \ dx \]}$

## Indeksy górne i dolne
$\mathcal{\[ a_1^2 + a_2^2 = a_3^2 \]}$

$\mathcal{\[ x^{2 \alpha} - 1 = y_{ij} + y_{ij} \]}$

$\mathcal{\[ (a^n)^{r+s} = a^{nr+ns} \]}$

## Indeksy górne i dolne
$\mathcal{\[ \sum_{i=1}^{\infty} \frac{1}{n^s} = \prod_p \frac{1}{1 - p^{-s}} \]}$

## Ułamki oraz n-nad-k (tzw. binomial)
\binom – definiuje tzw. n-nad-k

\frac – definuje ułamek

$\mathcal{
\[
\binom{n}{k} = \frac{n!}{k!(n-k)!}
\]
}$

Kiedy ułamki umiejscowione są wewnątrz tekstu,
na przykład $\mathcal{\(\frac{3x}{2}\)}$
można zmienić styl wyświetlania poprzez
komende \displaystyle:
$\mathcal{\( \displaystyle \frac{3x}{2} \)}$.

Podobnie jeśli wyświetlamy w stylu wyróżnionym
można zmienić styl wyświetlania poprzez
komende \textstyle:

$\mathcal{\[ f(x)=\frac{P(x)}{Q(x)} \ \ \textrm{and} \ \
f(x)=\textstyle\frac{P(x)}{Q(x)} \]}$

## Zagniezdżanie ułamków
$\mathcal{\[ \frac{1+\frac{a}{b}}
{1+\frac{1}{1+\frac{1}{a}}} \]}$

Komenda \cfrac{}{} dostarczona jest przez pakiet amsmath.

Komenda wyświetla zagnieżdżone ułamki bez zmiany ich rozmiaru.

$\mathcal{
\[
a_0+\cfrac{1}{a_1+\cfrac{1}
{a_2+\cfrac{1}{a_3+\cdots}}}
\]
}$

## Środowsko multiline
Środowisko multiline spowoduje, że pierwsza linia będzie wyświetlana do lewej, a złamana (druga) do prawej. Gwiazdka zapewnia, że równanie nie jest numerowane.

$\mathcal{
p(x) = 3x^6 + 14x^5y + 590x^4y^2 + 19x^3y^3 - 12x^2y^4 - 12xy^5 + 2y^6 - a^3b^3
}$

## Operatory i funkcje matematyczne
$\mathcal{
\[
\sin(a + b ) = \sin(a)\cos(b) + \cos(b)\sin(a)
\]
}$

Tryb wyświetlanie: 
$\mathcal{
\[
\lim_{h \rightarrow 0 } \frac{f(x+h)-f(x)}{h} \]
}$

Tryb inline: 

$\lim_{h \rightarrow 0 }
\frac{f(x+h)-f(x)}{h}$.


## Odstępy w trybie matematycznym
Odstępy we wzorze możemy robić przy pomocy komendy \quad:

$\mathcal{
\[ S = \{ z \in \mathbb{C}\, |\, |z| < 1 \}
\quad \textrm{and} \quad S_2=\partial{S} \]
}$


## Macierze
$\mathcal{
$$
\mathbf{X} = 
\left| \begin{array}{ccc} 
x_{11} & x_{12} & \ldots\\
x_{21} & x_{22} & \ldots\\
\vdots & \vdots & \ddots
\end{array} \right|
$$
}$


## Tabelka

Możliwość dodawania tabelki:

| Cyfra | Nastepna cyfra | Poprzednia cyfra |
| :------ |:--- | :--- |
| 5 | 5 | 4 |
| 10 | 11 | 9 |
| 7 | 8 | 6 |
| 2 | 3 | 1 |