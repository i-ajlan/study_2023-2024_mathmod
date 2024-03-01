---
## Front matter
title: "Отчёта по лабораторной работе"
subtitle: "Отчет Лаб 4"
author: "Аристид Жан Лоэнс"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Постройте фазовый портрет гармонического осциллятора и решение уравнения 
гармонического осциллятора в разных случаев. 




# Выполнение лабораторной работы

В этом рисунке написаны параметры дифф. уравнение гармонического осциллятора без затухании и без действия внешней силы. И написано тоже функция моделирующая такой случай. (рис. [-@fig:001]).

![Параметры первого случай](image/img01.png){#fig:001 width=70%}

График соотвествует первому случай (рис. [-@fig:002]).

![Первый график](image/img02.png){#fig:002 width=70%}

В этом рисунке написаны параметры дифф. уравнение гармонического осциллятора c затуханием и без действия внешней силы. И написано тоже функция моделирующая такой случай (рис. [-@fig:003]).

![Параметры второго случай](image/img03.png){#fig:003 width=70%}

График соотвествует второму случай (рис. [-@fig:004]).

![Второй график](image/img04.png){#fig:004 width=70%}

В этом рисунке написаны параметры дифф. уравнение гармонического осциллятора c затуханием и под действием внешней силы. И написано тоже функция моделирующая такой случай (рис. [-@fig:005]).

![Параметры третьего случай](image/img05.png){#fig:005 width=70%}

График соотвествует третьему случай (рис. [-@fig:006]).

![Третий график](image/img06.png){#fig:006 width=70%}

# Выводы

В первом случай когда у нас нет потера энергия в плоскости xy оциллиатор рисует траектория который безконечно повторится.

# Список литературы{.unnumbered}


