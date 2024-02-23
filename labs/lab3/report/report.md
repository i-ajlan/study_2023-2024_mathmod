---
## Front matter
title: "Отчёта по лабораторной работе"
subtitle: "Лабораторная работа 3"
author: "Аристид Жан Лоэнс Аристобуль Надаль"

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

Моделирование численности войски между соперниками с помощью временной функции.

# Задание

В моей задание, мне спросили построить графики изменения численности войск армии Х и армии У для
следующих случаев:
1. Модель боевых действий между регулярными войсками
2. Модель ведение боевых действий с участием регулярных войск и
партизанских отрядов 


# Выполнение лабораторной работы

Использавание библиотеки Plots и DifferentialEquations (рис. [-@fig:001]).

![Plots and DifferentialEquations library](image/img01.png){#fig:001 width=70%}

Разные Коэффициенты систем дифференциальных уравнении (рис. [-@fig:002]).

![Коэффициенты систем дифференциальных уравнении](image/img02.png){#fig:002 width=70%}

Модель боевых действий между регулярными войсками (рис. [-@fig:003]).

![Первый модель](image/img03.png){#fig:003 width=70%}

Граф первово моделя. (рис. [-@fig:004]).

![Граф первово моделя](image/img04.png){#fig:004 width=70%}

Модель ведение боевых действий с участием регулярных войск и партизанских отрядов  (рис. [-@fig:005]).

![Второй модель](image/img05.png){#fig:005 width=70%}

Граф второго моделя (рис. [-@fig:006]).

![Граф второго моделя](image/img06.png){#fig:006 width=70%}

# Выводы

В первой модель можно наметить что Армия Страна Y выиграл благодария их численному превосходство и в второй модель Страна Y проиграла даже с ихчисленном превосходством из-за того что не сражала регулярная армия.

