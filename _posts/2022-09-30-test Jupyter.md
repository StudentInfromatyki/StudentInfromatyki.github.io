---
layout: post
title: Dodanie Jupyter 
subtitle: Dodanie Jupyter
cover-img: /assets/img/pobrane.png
thumbnail-img: /assets/img/1200px-Jupyter_logo.png
share-img: /assets/img/pobrane.png
tags: [jupyter, kod]
---

**JupyterLab** to najnowsze internetowe interaktywne środowisko programistyczne dla notatników, kodu i danych. Jego elastyczny interfejs pozwala użytkownikom konfigurować i organizować przepływy pracy w nauce o danych, obliczeniach naukowych, dziennikarstwie obliczeniowym i uczeniu maszynowym. Modułowa konstrukcja zachęca do rozszerzenia i wzbogacenia funkcjonalności.

**Notatnik Jupyter** to oryginalna aplikacja internetowa do tworzenia i udostępniania dokumentów obliczeniowych. Oferuje proste, usprawnione, zorientowane na dokumenty doświadczenie.

**Do czego służy Jupyter?** 
Jedną z nich jest Jupyter i jego notebook, który pozwala na tworzenie interaktywnych arkuszy mogących zawierać kod wykonywalny, opisy, tabele, wykresy i wiele innych danych, które mogą służyć nam między innymi do prezentacji wyników naszych prac

Zadaniem tej funkcjonalności było dodanie Jupytera po stronie statycznej. Żeby użytkownik, który będzie korzystał z tego repozytorium mógł dodać szablon kodu lub innych danych.  

Można to było zrobić na dwa sposoby. Pierwszy z nich to dodanie notatnika Jupytera po stronie zewnętrznej Cocalc. Poniżej zostanie umieszczony przykład, który to umożliwia: 

Tutaj przykładowy kod: [some code I wrote for code](code.md).

```python
x = 1
if x == 1:
    # indented four spaces
    print("x is 1.")
```

    x is 1.



```python

```

**CoCalc** to internetowa platforma do przetwarzania w chmurze (SaaS) i zarządzania kursami dla matematyki obliczeniowej. W ramach projektu Sage obsługuje edycję arkuszy roboczych Sage, dokumentów LaTeX i notatników Jupyter. CoCalc uruchamia środowisko Ubuntu Linux, z którym można komunikować się za pośrednictwem terminala, dodatkowo dając dostęp do większości możliwości Linuksa. 

Usługa została utworzona w 2007 roku przez Daniela Ha i Jasona Yana. W 2011 roku usługa zajęła pierwsze w rankingu Quantcast ze 379,8 miliona unikalnych wizyt. W 2016 roku usługa zajęła 278 miejsce w rankingu Alexa Internet. Disqus jest umieszczony na 750 tysiącach ston internetowych.

Drugim sposobem jest to skonfigurowanie w kodzie repozytorium, tzn. dodanie kawałku kodu, który będzie odpowiadał za dodanie funkcjonalności. Jest to trudne do zrealizowania, dlatego że blog jest relizowany z pomocą silnika Jekyll. Problem polega na tym, że każdy silnik działa inaczej, więc trzeba byłoby zmieniać konfigurację w silniku. 

Jest także opcja dodawania notatników, kodów oraz innych informacji w sposób, który będzie zaprezentowany poniżej. Jest to sposób, któy polega na dodawaniu informacji umieszczonych w znacznikach ~. Także można dodawać różnymi sposobami, tzn. żeby kod był numerowany oraz nienumerowany, a także, żeby było widocznie w jakim języku programowania jest napisany kod.


O to fragment kodu:

~~~
var foo = function(x) {
  return(x + 5);
}
foo(3)
~~~

A oto ten sam kod z podświetlaniem składni:

```javascript
var foo = function(x) {
  return(x + 5);
}
foo(3)
```

A oto ten sam kod jeszcze raz, ale z numerami linii:

{% highlight javascript linenos %}
var foo = function(x) {
  return(x + 5);
}
foo(3)
{% endhighlight %}

## Pudła
Możesz dodać pola powiadomień, ostrzeżeń i błędów w następujący sposób:

### Powiadomienie

{: .box-note}
**Notatka:** To jest pole powiadomień.

### Ostrzeżenia

{: .box-warning}
**Ostrzeżenia:** To jest pole ostrzeżeń.

### Błąd

{: .box-error}
**Błąd:** To jest pole błędu.

