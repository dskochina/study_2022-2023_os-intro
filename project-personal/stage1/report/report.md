---
## Front matter
title: "Отчёт по первому этапу индивидуального проекта"
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

Целью первого этапа индивидуального проекта является размещение на Github pages заготовки для персонального сайта.

# Выполнение лабораторной работы

1. Я перешла по ссылке на сайт https://github.com/gohugoio/hugo/releases и скачала необходимый файл. (рис. [-@fig:001], [-@fig:002])

![Сайт](image/Рис.1.png){ #fig:001 width=70% }

![Файл, скаченный с сайта](image/Рис.2.png){ #fig:002 width=70% }

2. Я создала в домашней папке пустую папку под названием bin и скопировала в неё из загрузок файл hugo. (рис. [-@fig:003], [-@fig:004])

![Папка bin](image/Рис.3.png){ #fig:003 width=70% }

![Файл hugo в папке bin](image/Рис.4.png){ #fig:004 width=70% }

3. Я открыла ссылку из ТУИСа на репозиторий (в качестве шаблона индивидуального сайта используется шаблон Hugo Academic Theme). Перешла по этой ссыллке и создала новый репозиторий под названием blog. (рис. [-@fig:005], [-@fig:006], [-@fig:007])

![Создание нового репозитория](image/Рис.5.png){ #fig:005 width=70% }

![Создание нового репозитория](image/Рис.6.png){ #fig:006 width=70% }

![Создание нового репозитория](image/Рис.7.png){ #fig:007 width=70% }

4. Я скопировала ссылку своего репозитория (SSH), открыла терминал и прописала команду клонирования. (рис. [-@fig:008], [-@fig:009])

![Ссылка](image/Рис.8.png){ #fig:008 width=70% }

![Клонирование в "blog"](image/Рис.9.png){ #fig:009 width=70% }

5. Перешла в каталог cd/blog и просмотрела все файлы с помощью команды ls -l. (рис. [-@fig:010])

![Просмотр файлов](image/Рис.10.png){ #fig:010 width=70% }

6. При помощи команды ls -l просмотрела все файлы, перешла в mc для того, чтобы удалить каталог public.

7. Я набрала в терминале команду ~/bin/hugo server, скопировала ссылку, вставила её в Браузер. После произведённых мною действий открылся сайт. (рис. [-@fig:011], [-@fig:012])

![Команды](image/Рис.11.png){ #fig:011 width=70% }

![Переход по ссылке на сайт](image/Рис.12.png){ #fig:012 width=70% }

8. Я создала новый репозиторий со специальным названием "dskochina.github.io". (рис. [-@fig:013], [-@fig:014])

![Создание репозитория](image/Рис.13.png){ #fig:013 width=70% }

![Создание репозитория](image/Рис.14.png){ #fig:014 width=70% }

9. Я перешла на уровень выше из каталога blog, скопировала ссылку репозитория, применила команду git clone --recursive, чтобы клонировать репозиторий. (рис. [-@fig:015], [-@fig:016])

![Клонирование репозитория](image/Рис.15.png){ #fig:015 width=70% }

![Клонирование репозитория](image/Рис.16.png){ #fig:016 width=70% }

10. Я ввела команду для создания новой ветки main. (рис. [-@fig:017])

![Создание новой ветки](image/Рис.17.png){ #fig:017 width=70% }

11. Я создала пустой файл и отправила его на Github. (рис. [-@fig:018], [-@fig:019], [-@fig:020])

![Создание пустого файла](image/Рис.18.png){ #fig:018 width=70% }

![Отправка файла на Github](image/Рис.19.png){ #fig:019 width=70% }

![Отправка файла на Github](image/Рис.20.png){ #fig:020 width=70% }

![Отправка файла на Github](image/Рис.21.png){ #fig:021 width=70% }

12. Я перешла в cd blog/, с помощью команды pwd убедилась, что я нахожусь в данном каталоге. (рис. [-@fig:022])

![Команда pwd](image/Рис.22.png){ #fig:022 width=70% }

13. Я ввела команду, которая подключила новый репозиторий к папке public внутри blog. (рис. [-@fig:023])

![Команда](image/Рис.23.png){ #fig:023 width=70% }

14. Я открыла mc, перешла в .gitignore, поставила знак "#" возле "public" и сохранила изменения. (рис. [-@fig:024])

![public](image/Рис.24.png){ #fig:024 width=70% }

15. При помощи команды cat я убедилась, что файл public со знаком "#", чтобы не происходило игнорирование этих каталогов. (рис. [-@fig:025])

![public](image/Рис.25.png){ #fig:025 width=70% }

16. Я повторила команду из пункта 13, чтобы моя папка была видна в репозитории. (рис. [-@fig:026])

![Команда](image/Рис.26.png){ #fig:026 width=70% }

17. После ввода ~/bin/hugo автоматически появились папки. (рис. [-@fig:027], [-@fig:028])

![~/bin/hugo](image/Рис.27.png){ #fig:027 width=70% }

![Файлы в папке public](image/Рис.28.png){ #fig:028 width=70% }

18. Я ввела команду git remote, чтобы подключить каталог к моему репозиторию. (рис. [-@fig:029], [-@fig:030], [-@fig:031])

![Команда git remote](Рис.29.png){ #fig:029 width=70% }

![Команды git add и git commit](image/Рис.30.png){ #fig:030 width=70% }

![Команда git push](image/Рис.31.png){ #fig:031 width=70% }

19. Я обновила репозиторий и убедилась в том, что появились все файлы. (рис. [-@fig:032])

![Репозиторий с файлами](image/Рис.32.png){ #fig:032 width=70% }

20. Я ввела в Браузер ссылку на сайт из репозитория и перешла по ней. (рис. [-@fig:033])

![Сайт](image/Рис.33.png){ #fig:033 width=70% }

# Выводы

Я сделала первый этап индивидуального проекта, целью которого являлось размещение на Github pages заготовки для персонального сайта.

