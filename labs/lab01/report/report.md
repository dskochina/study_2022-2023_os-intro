---
## Front matter
title: "Отчёт по лабораторной работе №1"
subtitle: "Установка ОС Linux"
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
biblatex: false
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

Целью данной работы является приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

# Задание

Приобрести практические навыки установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

# Теоретическое введение

*Операционная система (ОС)* — это комплекс взаимосвязанных программ, предназначенных для управления ресурсами компьютера и организации взаимодействия с пользователем. Сегодня наиболее известными операционными системами являются ОС семейства Microsoft Windows и UNIX-подобные системы.

*GNU Linux* — семейство переносимых, многозадачных и многопользовательских операционных систем, на базе ядра Linux, включающих тот или иной набор утилит и программ проекта GNU, и, возможно, другие компоненты. Как и ядро Linux, системы на его основе, как правило, создаются и распространяются в соответствии с моделью разработки свободного и открытого программного обеспечения (Open-Source Software). Linux-системы распространяются в основном бесплатно в виде различных дистрибутивов.

*Дистрибутив GNU Linux* — общее определение ОС, использующих ядро Linux и набор библиотек и утилит, выпускаемых в рамках проекта GNU, а также графическую оконную подсистему X Window System . Дистрибутив готов для конечной установки на пользовательское оборудование. Кроме ядра и, собственно, операционной системы дистрибутивы обычно содержат широкий набор приложений, таких как редакторы документов и таблиц, мультимедийные проигрыватели, системы для работы с базами данных и т.д. Существуют дистрибутивы, разрабатываемые как при коммерческой поддержке (Red Hat / Fedora, SLED / OpenSUSE, Ubuntu), так и исключительно усилиями добровольцев (Debian, Slackware, Gentoo, ArchLinux).

# Выполнение лабораторной работы

1. Запустила виртуальную машину, введя в командной строке VirtualBox &. (рис. [-@fig:001])

![Запуск виртуальной машины](image/Рис.1.png){ #fig:001 width=70% }

2. В свойства VirtualBox изменила месторасположение каталога для виртуальных машин, указав учётную запись на месте «имя пользователя». (рис. [-@fig:002])

![Окно "Свойства VirtualBox"](image/Рис.2.png){ #fig:002 width=70% }

3. Сменила комбинацию хост-клавиши, использующейся для освобождения курсора мыши, который может захватывать виртуальная машина. (рис. [-@fig:003])

![Смена хост-клавиши](image/Рис.3.png){ #fig:003 width=70% }

4. Создадала новую виртуальную машину, указав имя виртуальной машины (учётная запись) и тип операционной системы (Linux, Fedora (64-bit)). (рис. [-@fig:004])

![Окно "Имя машины и тип ОС"](image/Рис.4.png){ #fig:004 width=70% }

5. Указала размер основной памяти виртуальной машины (2048 МБ). (рис. [-@fig:005])

![Окно "Размер основной памяти"](image/Рис.5.png){ #fig:005 width=70% }

6. Задала конфигурацию жесткого диска (загрузочный, VDI, динамический виртуальный диск). (рис. [-@fig:006], [-@fig:007], [-@fig:008])

![Окно создания жесткого диска на виртуальной машине](image/Рис.6.png){ #fig:006 width=70% }

![Окно определения типа подключения виртуального жесткого диска](image/Рис.7.png){ #fig:007 width=70% }

![Окно определения формата виртуального жесткого диска](image/Рис.8.png){ #fig:008 width=70% }

7. Задала расположение диска и его размер (80 ГБ). (рис. [-@fig:009])

![Размер виртуального динамического жесткого диска и его расположение](image/Рис.9.png){ #fig:009 width=70% }

8. настройках виртуальной машины во вкладке «дисплей -> экран» увеличила доступный объём видеопамяти до 128 МБ. (рис. [-@fig:010])

![Настройка виртуальной машины](image/Рис.10.png){ #fig:010 width=70% }

9. В настройках виртуальной машины добавила новый привод оптических дисков. (рис. [-@fig:011])

![Окно «Носители» виртуальной машины: выбор оптического диска](image/Рис.11.png){ #fig:011 width=70% }

10. Скорректировала настройки системы (раскладку клавиатуры, часовой пояс, место установки). (рис. [-@fig:012], [-@fig:013], [-@fig:014])

![Окно выбора языка](image/Рис.12.png){ #fig:012 width=70% }

![Окно выбора часового пояса](image/Рис.13.png){ #fig:013 width=70% }

![Окно выбора места установки](image/Рис.14.png){ #fig:014 width=70% }

11. Запустила установку операционной системы.

12. Создала имя пользователя, используя свой логин в дисплейном классе, и установила пароль. (рис. [-@fig:015], [-@fig:016])

![Окно создания имя пользователя](image/Рис.15.png){ #fig:015 width=70% }

![Окно установки пароля](image/Рис.16.png){ #fig:016 width=70% }

13. Выключила систему и совершила изъятие образа диска из дисковода. (рис. [-@fig:017])

![Извлечение образа диска](image/Рис.17.png){ #fig:017 width=70% }

14. Я вошла в ОС под заданной мной при установке учётной записью. Нажала комбинацию Win+Enter для запуска терминала.

15. Я переключилась на роль супер-пользователя и ввела пароль. (рис. [-@fig:018])

![Команда sudo -i](image/Рис.18.png){ #fig:018 width=70% }

16. Я обновила все пакеты. (рис. [-@fig:019], [-@fig:020], [-@fig:021])

![Команда dnf -y update](image/Рис.19.png){ #fig:019 width=70% }

![Обновление пакетов, запуск скриптлетов](image/Рис.20.png){ #fig:020 width=70% }

![Обновление пакетов](image/Рис.21.png){ #fig:021 width=70% }

17. Я использовала программы для удобства работы в консоли. (рис. [-@fig:022])

![Команда dnf install tmux mc](image/Рис.22.png){ #fig:022 width=70% }

18. Я использовала автоматическое обновление. Задала необходимую конфигурацию в файле /etc/dnf/automatic.conf. Запустите таймер при помощи команды: systemctl enable --now dnf-automatic.timer. (рис. [-@fig:023], [-@fig:024])

![Команда dnf install dnf-automatic](image/Рис.23.png){ #fig:023 width=70% }

![Результат](image/Рис.24.png){ #fig:024 width=70% }

19. Я открыла mc и в файле /etc/selinux/config заменила значение SELINUX=enforcing на значение SELINUX=permissive. (рис. [-@fig:025])

![Окно mc](image/Рис.25.png){ #fig:025 width=70% }

20. Я установила пакет DKMS. (рис. [-@fig:026], [-@fig:027])

![Команда dnf -y install dkms](image/Рис.26.png){ #fig:026 width=70% }

![Результат](image/Рис.27.png){ #fig:027 width=70% }

21. В меню виртуальной машины я подключила образ диска дополнений гостевой ОС. Подмонтировала диск. Установила драйвера: /media/VBoxLinuxAdditions.run. Перезагрузила виртуальную машину с помощью команды reboot. (рис. [-@fig:028])

![Команда mount /dev/sr0 /media](image/Рис.28.png){ #fig:028 width=70% }

22. Нажала комбинацию Win+Enter для запуска терминала. Запустила терминальный мультиплексор tmux. Переключилась на роль супер-пользователя: sudo -i.

23. Я установила pandoc. (рис. [-@fig:029], [-@fig:030])

![Команда dnf -y install pandoc](image/Рис.29.png){ #fig:029 width=70% }

![Результат](image/Рис.30.png){ #fig:030 width=70% }

24. Я установила дистрибутив TeXlive. (рис. [-@fig:031])

![Команда dnf -y install texlive texlive-\*](image/Рис.31.png){ #fig:031 width=70% }


**Домашнее задание**

1. Версия ядра Linux: 5.2.0-kali2-amd64.

2. Частота процессора: 1995.390 МГц.

3. Модель процессора: Intel(R)Core(TM) i3-5005U CPU @ 2.00GHz.

4. Объём доступной оперативной памяти: 2096628 КБ.

5. Тип обнаруженного гипервизора: Vmware.

6. Тип файловой системы корневого раздела и последовательность монтирования файловых систем: Тип файловой системы корневого раздела - EXT4.

**Ответы на контрольные вопросы**

1. Учётная запись пользователя – это необходимая для системы информация о пользователе, хранящаяся в специальных файлах. Информация используется Linux для аутентификации пользователя и назначения ему прав доступа. Аутентификация – системная процедура, позволяющая Linux определить, какой именно пользователь осуществляет вход. Вся информация о пользователе обычно хранится в файлах /etc/passwd и /etc/group.
Учётная запись пользователя содержит:
-Имя пользователя (user name)
-Идентификационный номер пользователя (UID)
-Идентификационный номер группы (GID)
-Пароль (password)
-Полное имя (full name)
-Домашний каталог (home directory)
-Начальную оболочку (login shell)

2. Команды терминала:
-Для получения справки по команде:
man. Например, команда «man ls» выведет справку о команде «ls».
-Для перемещения по файловой системе:
cd [путь]. Например, команда «cd newdir» осуществляет переход в
каталог newdir.
-Для просмотра содержимого каталога:
ls. Например, команда «ls –a ~/newdir» отобразит имена скрытых файлов в каталоге newdir.
-Для определения объёма каталога:
du. Например, команда «du –k ~/newdir» выведет размер каталога newdir в килобайтах.
-Для создания / удаления каталогов / файлов:
mkdir  / rmdir  / rm . Например, команда «mkdir –p ~/newdir1/newdir2» создаст иерархическую цепочку подкаталогов, создав каталоги newdir1 и newdir2; команда «rmdir -v ~/newdir» удалит каталог newdir; команда «rm –r ~/newdir» так же удалит каталог newdir.
-Для задания определённых прав на файл / каталог: сhmod. Например, команда «сhmod g+r ~/text.txt» даст группе право на чтение файла text.txt.
-Для просмотра истории команд:
history. Например, команда «history 5» покажет список последних 5 команд.

3. Файловая система имеет два значения: с одной стороны – это архитектура хранения битов на жестком диске, с другой – это организация каталогов в соответствии с идеологией Unix.
Файловая система (англ. «file system») – это архитектура хранения данных в системе, хранение данных в оперативной памяти и доступа к конфигурации ядра. Файловая система устанавливает физическую и логическую структуру файлов, правила их создания и управления ими. В физическом смысле файловая система Linux представляет собой пространство раздела диска, разбитое на блоки фиксированного размера. Их размер кратен размеру сектора: 1024, 2048, 4096 или 8120
байт.
Существует несколько типов файловых систем:
**XFS** – начало разработки 1993 год, фирма Silicon Graphics, в мае 2000 года предстала в GNU GPL, для пользователей большинства Linux систем стала доступна в 2001-2002 гг. Отличительная черта системы – прекрасная поддержка больших файлов и файловых томов, 8 эксбибайт (8*260 байт) для 64-х битных систем.
**ReiserFS (Reiser3)** – одна из первых журналируемых файловых систем под Linux, разработана Namesys, доступна с 2001 г. Максимальный объём тома для этой системы равен 16 тебибайт (16*240 байт).
**Tux2** – известная, но так и не анонсированная публично файловая система. Создатель Дэниэл Филипс (Daniel Phillips). Cистема базируется на алгоритме «Фазового Дерева», который как и журналирование защищает файловую систему от сбоев. Организована как надстройка на ext2.

4. Команда «findmnt» или «findmnt --all» будет отображать все подмонтированные файловые системы или искать файловую систему.

5. Основные сигналы (каждый сигнал имеет свой номер), которые используются для завершения процесса:
-SIGINT – самый безобидный сигнал завершения, означает Interrupt. Он отправляется процессу, запущенному из терминала с помощью сочетания клавиш Ctrl+C. Процесс правильно завершает все свои действия и возвращает управление;
-SIGQUIT – это еще один сигнал, который отправляется с помощью сочетания клавиш, программе, запущенной в терминале. Он сообщает ей что нужно завершиться и программа может выполнить
корректное завершение или проигнорировать сигнал. В отличие отпредыдущего, она генерирует дамп памяти. Сочетание клавиш Ctrl+/;
-SIGHUP – сообщает процессу, что соединение с управляющим терминалом разорвано, отправляется, в основном, системой при разрыве соединения с интернетом;
-SIGTERM – немедленно завершает процесс, но обрабатывается программой, поэтому позволяет ей завершить дочерние процессы и освободить все ресурсы;
SIGKILL – тоже немедленно завершает процесс, но, в отличие от предыдущего варианта, он не передается самому процессу, а обрабатывается ядром. Поэтому ресурсы и дочерние процессы остаются запущенными.
Также для передачи сигналов процессам в Linux используется утилита kill, её синтаксис: kill [-сигнал] [pid_процесса] (PID – уникальный идентификатор процесса). Сигнал представляет собой один из выше перечисленных сигналов для завершения процесса.
Перед тем, как выполнить остановку процесса, нужно определить его PID.
Для этого используют команды ps и grep. Команда ps предназначена для вывода списка активных процессов в системе и информации о них. Команда grep запускается одновременно с ps (в канале) и будет выполнять поиск по результатам команды ps.
Утилита pkill – это оболочка для kill, она ведет себя точно так же, и имеет тот же синтаксис, только в качестве идентификатора процесса ей нужно передать его имя.
killall работает аналогично двум предыдущим утилитам. Она тоже принимает имя процесса в качестве параметра и ищет его PID в директории /proc. Но эта утилита обнаружит все процессы с таким именем и завершит их.

# Выводы

В ходе выполнения данной лабораторной работы я научилась устанавливать операционную систему Linux (дистрибутив Fedora 36) на виртуальную машину VirtualBox и настраивать минимально необходимые параметры для дальнейшей работы с системой в соответствии с методическими рекомендациями, приложенными к работе.

