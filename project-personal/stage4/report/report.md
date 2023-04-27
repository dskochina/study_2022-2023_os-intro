---
## Front matter
title: "Отчёт по четвёртому этапу индивидуального проекта"
subtitle: "*дисциплина: Операционные системы*"
author: "Дарья Сергеевна Кочина"

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
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Целью четвёртого этапа индивидуального проекта является добавление к сайту ссылок на научные и библиометрические ресурсы.

# Задание

1. Зарегистрироваться на соответствующих ресурсах и разместить на них ссылки на сайте:
eLibrary : https://elibrary.ru/;
Google Scholar : https://scholar.google.com/;
ORCID : https://orcid.org/;
Mendeley : https://www.mendeley.com/;
ResearchGate : https://www.researchgate.net/;
Academia.edu : https://www.academia.edu/;
arXiv : https://arxiv.org/;
github : https://github.com/.

2. Сделать пост по прошедшей неделе.

3. Добавить пост на тему по выбору:
Оформление отчёта.
Создание презентаций.
Работа с библиографией.

# Выполнение лабораторной работы

1. Вместо данных ресурсов я добавила ссылки на свой канал на youtube, ВК и гитхаб. Для этого перешла в папку "content" -> "authors" -> "admin" и в файле изменила информацию. Затем проверила информацию на сайте. (рис. [-@fig:001], [-@fig:002])

![Изменение ссылок](image/Рис.1.png){#fig:001 width=80%}

![Изменение ссылок](image/Рис.2.png){#fig:002 width=80%}

2. Я ввела в терминале команду ~/bin/hugo new post/last_week2. Далее написала пост по прошедшей неделе и проверила изменения на сайте. (рис. [-@fig:003], [-@fig:004], [-@fig:005])

![Пост недели](image/Рис.3.png){#fig:003 width=80%}

![Пост недели](image/Рис.4.png){#fig:004 width=80%}

![Пост недели](image/Рис.5.png){#fig:005 width=80%}

3. Я ввела в терминале команду ~/bin/hugo new post/making_presentations. Затем я создала пост на тему по выбору: Создание презентаций. Я создала пост, размещая необходимую информацию и проверила изменения на сайте. (рис. [-@fig:006], [-@fig:007], [-@fig:008]) 

![Пост на тему](image/Рис.6.png){#fig:006 width=80%}

![Пост на тему](image/Рис.7.png){#fig:007 width=80%}

![Пост на тему](image/Рис.8.png){#fig:008 width=80%}

# Выводы

В ходе выполнения четвёртого этапа индивидуального проекта я приобрела практические навыки по созданию сайта, получила новые знания. Добавила к сайту ссылки на научные и библиометрические ресурсы.

