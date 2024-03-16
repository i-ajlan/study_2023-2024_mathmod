---
## Front matter
title: "Отчёта по Игра блотто"
subtitle: "Теория Игр"
author: "Аристид Жан Лоэнс Аристобуль"

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

 Описание Игра блотто

# Задание

Рассмотрим игру, в которой каждый из двух игроков записывает по три положительных целых числа в неубывающем порядке так, чтобы их сумма составляла заранее заданное число S. Впоследствии два игрока показывают друг другу свои записи и сравнивают соответствующие числа. Игрок, у которого на два числа больше соответствующих чисел противника, побеждает в игре. Наити лучше стратегия и Nash equilibrum.

# Теоретическое введение

Классическая версия игры Blotto сталкивает двух игроков с одинаковым количеством ресурсов друг против друга с задачей распределить свои ресурсы по N полям. Игрок, разместивший на поле больше ресурсов, выигрывает поле, а победа достается игроку, выигравшему больше полей.

# Выполнение лабораторной работы

- Игроки: А и Б.
- Ресурсы: 6 солдат
- Поля: 3 поля битвы
- Стратегии: S1(1, 1, 4), S2(2, 2, 2), S3(1, 2, 3).

- S1 против S1 — ничья.
- S2 против S2 — ничья.
- S3 против S3 - Ничья.
- S2 бьёт S1.

Отсюда следует, что оптимальной стратегией является (2, 2, 2), поскольку она не хуже, чем достижение безубыточности по сравнению с любой другой стратегией, одновременно превосходя другую стратегию. Однако существует несколько равновесий Нэша. Если оба игрока выбирают стратегию (2, 2, 2) или (1, 2, 3), то ни один из них не сможет победить другого, меняя стратегии, поэтому каждая такая пара стратегий является равновесием Нэша.


# Выводы

Игра с блотто можно применить к американским президентским выборам, где каждый штат представляет собой поле битвы, за которое нужно победить, и где ваша избирательная команда, ваш бюджет, количество избирательных собраний представляют собой ресурсы, которые вы должны распределить. И тот, кто победит в большинстве штатов, побеждает на выборах.

# Список литературы{.unnumbered}

- The Theory of Play and Integral Equations with Skew Symmetric Kernels (1953 translation from the French paper "La théorie du jeu et les équations intégrales à noyau symétrique gauche")
- Emile Borel and Jean Ville. Application de la théorie des probabilités aux jeux de hasard. Gauthier-Villars, Paris, 1938. Reprinted in: by E.Borel and A. Chéron Théorie mathématique du bridge à la portée de tous, Editions Jacques Gabay, Paris, 1991.
- Guillermo Owen, Game Theory, Academic Press (1968)
- A Continuous Colonel Blotto Game
