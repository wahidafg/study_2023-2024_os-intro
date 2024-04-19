---
## Front matter
title: "Шаблон отчёта по лабораторной работе 11"
author: "Абдуллахи Абдул Вахид"

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

Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором Emacs.

# Задание

1. Ознакомиться с теоретическим материалом.

2. Ознакомиться с редактором emacs.

3. Выполнить упражнения.

4. Ответить на контрольные вопросы.

# Последовательность выполнения работы

1. Открыть emacs.

![](image/1.png){#fig:001 width=100%}

2. Создать файл lab07.sh с помощью комбинации Ctrl-x Ctrl-f (C-x C-f).

![](image/2.png){#fig:001 width=100%}

3. Наберите текст

![](image/3.png){#fig:001 width=100%}

4. Сохранить файл с помощью комбинации Ctrl-x Ctrl-s (C-x C-s).

![](image/4.png){#fig:001 width=100%}

5. Проделать с текстом стандартные процедуры редактирования, каждое действие должно осуществляться комбинацией клавиш.

5.1. Вырезать одной командой целую строку (С-k).

5.2. Вставить эту строку в конец файла (C-y).

![](image/5-1-2.png){#fig:001 width=100%}

5.3. Выделить область текста (C-space).

![](image/5-3.png){#fig:001 width=100%}

5.4. Скопировать область в буфер обмена (M-w).

![](image/5-4.png){#fig:001 width=100%}

5.5. Вставить область в конец файла.

![](image/5-5.png){#fig:001 width=100%}

5.6. Вновь выделить эту область и на этот раз вырезать её (C-w).

![](image/5-6.png){#fig:001 width=100%}

![](image/5-6-1.png){#fig:001 width=100%}

5.7. Отмените последнее действие (C-/).

![](image/5-7.png){#fig:001 width=100%}

6. Научитесь использовать команды по перемещению курсора.

6.1. Переместите курсор в начало строки (C-a).

![](image/6-1.png){#fig:001 width=100%}

6.2. Переместите курсор в конец строки (C-e).

![](image/6-2.png){#fig:001 width=100%}

6.3. Переместите курсор в начало буфера (M-<).

![](image/6-3.png){#fig:001 width=100%}

6.4. Переместите курсор в конец буфера (M->).

![](image/6-4.png){#fig:001 width=100%}

7. Управление буферами.

7.1. Вывести список активных буферов на экран (C-x C-b).

![](image/7-1.png){#fig:001 width=100%}

8. Управление окнами.

8.1. Поделите фрейм на 4 части: разделите фрейм на два окна по вертикали (C-x 3), а затем каждое из этих окон на две части по горизонтали (C-x 2) (см. рис. 9.1).

![](image/8-1.png){#fig:001 width=100%}

8.2. В каждом из четырёх созданных окон откройте новый буфер (файл) и введите несколько строк текста.

![](image/8-2.png){#fig:001 width=100%}

9. Режим поиска

9.1. Переключитесь в режим поиска (C-s) и найдите несколько слов, присутствующих в тексте.

![](image/9-1.png){#fig:001 width=100%}

9.2. Переключайтесь между результатами поиска, нажимая C-s.

![](image/9-2.png){#fig:001 width=100%}

9.4. Перейдите в режим поиска и замены (M-%), введите текст, который следует найти и заменить, нажмите Enter , затем введите текст для замены. После того как будут подсвечены результаты поиска, нажмите ! для подтверждения замены.

![](image/9-4.png){#fig:001 width=100%}

# Выводы

Здесь кратко описываются итоги проделанной работы.

# Список литературы{.unnumbered}

::: {#refs}
:::
