---
## Front matter
title: "Шаблон отчёта по лабораторной работе 4"
subtitle: "Простейший вариант"
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

Получение навыков правильной работы с репозиториями git.

# Задание

Выполнить работу для тестового репозитория.

Преобразовать рабочий репозиторий в репозиторий с git-flow и conventional commits.

Последовательность выполнения работы

Установка программного обеспечения

Установка git-flow

установка gitflow

Enable the copr repository

dnf copr enable elegos/gitflow

Install gitflow

dnf install gitflow

![](image/1.png){#fig:001 width=100%}

![](image/2.png){#fig:001 width=100%}

Установка Node.js

На Node.js базируется программное обеспечение для

семантического версионирования и общепринятых коммитов.

![](image/3.png){#fig:001 width=100%}

![](image/4.png){#fig:001 width=100%}

у меня не получилось установить pnpm поэтому я установил его через его сайт 

![](image/4-1.png){#fig:001 width=100%}

![](image/4-2.png){#fig:001 width=100%}

Настройка Node.js

запустим 

ерелогиньтесь, или выполните

![](image/5.png){#fig:001 width=100%}

Общепринятые коммиты

установка git-cz

![](image/6.png){#fig:001 width=100%}

standard-changelog

![](image/7.png){#fig:001 width=100%}

Создание репозитория git

![](image/8.png){#fig:001 width=100%}

![](image/8-1.png){#fig:001 width=100%}

Делаем первый коммит и выкладываем на github:

![](image/9.png){#fig:001 width=100%}

![](image/10.png){#fig:001 width=100%}

![](image/11.png){#fig:001 width=100%}

Конфигурация для пакетов Node.js

![](image/12.png){#fig:001 width=100%}

Необходимо заполнить несколько параметров пакета.

Название пакета.
Лицензия пакета. Список лицензий для npm: https://spdx.org/licenses/. Предлагается выбирать лицензию CC-BY-4.0.

Сконфигурим формат коммитов. Для этого добавим в файл package.json команду для формирования коммитов:

![](image/12-1.png){#fig:001 width=100%}

![](image/12-2.png){#fig:001 width=100%}

Добавим новые файлы:

![](image/13.png){#fig:001 width=100%}

Выполним коммит:

![](image/14.png){#fig:001 width=100%}

отправил на гитхаб

Инициализируем git-flow

![](image/15.png){#fig:001 width=100%}

Проверьте, что Вы на ветке develop:

![](image/16.png){#fig:001 width=100%}

Загрузите весь репозиторий в хранилище:

![](image/17.png){#fig:001 width=100%}

Установите внешнюю ветку как вышестоящую для этой ветки:

![](image/18.png){#fig:001 width=100%}

Создадим релиз с версией 1.0.0

![](image/19.png){#fig:001 width=100%}

Создадим журнал изменений

![](image/20.png){#fig:001 width=100%}

Добавим журнал изменений в индекс

![](image/21.png){#fig:001 width=100%}

Зальём релизную ветку в основную ветку

![](image/22.png){#fig:001 width=100%}

![](image/22-1.png){#fig:001 width=100%}

![](image/22-2.png){#fig:001 width=100%}

Отправим данные на github

![](image/23.png){#fig:001 width=100%}

Создадим релиз на github. Для этого будем использовать утилиты работы с github:

![](image/24.png){#fig:001 width=100%}

Разработка новой функциональности

Создадим ветку для новой функциональности:

![](image/25.png){#fig:001 width=100%}

Далее, продолжаем работу c git как обычно.

По окончании разработки новой функциональности следующим 

шагом следует объединить ветку feature_branch c develop:

![](image/25-1.png){#fig:001 width=100%}

Создание релиза git-flow

![](image/26.png){#fig:001 width=100%}

Обновите номер версии в файле package.json. Установите её в 1.2.3.

![](image/26-1.png){#fig:001 width=100%}

Создадим журнал изменений

![](image/27.png){#fig:001 width=100%}

Добавим журнал изменений в индекс

![](image/28.png){#fig:001 width=100%}

Зальём релизную ветку в основную ветку

![](image/29.png){#fig:001 width=100%}

Отправим данные на github

![](image/30.png){#fig:001 width=100%}

Создадим релиз на github с комментарием из журнала изменений:

![](image/31.png){#fig:001 width=100%}

# Теоретическое введение

Здесь описываются теоретические аспекты, связанные с выполнением работы.

Например, в табл. [-@tbl:std-dir] приведено краткое описание стандартных каталогов Unix.

: Описание некоторых каталогов файловой системы GNU Linux {#tbl:std-dir}

| Имя каталога | Описание каталога                                                                                                          |
|--------------|----------------------------------------------------------------------------------------------------------------------------|
| `/`          | Корневая директория, содержащая всю файловую                                                                               |
| `/bin `      | Основные системные утилиты, необходимые как в однопользовательском режиме, так и при обычной работе всем пользователям     |
| `/etc`       | Общесистемные конфигурационные файлы и файлы конфигурации установленных программ                                           |
| `/home`      | Содержит домашние директории пользователей, которые, в свою очередь, содержат персональные настройки и данные пользователя |
| `/media`     | Точки монтирования для сменных носителей                                                                                   |
| `/root`      | Домашняя директория пользователя  `root`                                                                                   |
| `/tmp`       | Временные файлы                                                                                                            |
| `/usr`       | Вторичная иерархия для данных пользователя                                                                                 |

Более подробно про Unix см. в [@tanenbaum_book_modern-os_ru; @robbins_book_bash_en; @zarrelli_book_mastering-bash_en; @newham_book_learning-bash_en].

# Выполнение лабораторной работы

Описываются проведённые действия, в качестве иллюстрации даётся ссылка на иллюстрацию (рис. [-@fig:001]).

![Название рисунка](image/placeimg_800_600_tech.jpg){#fig:001 width=70%}

# Выводы

Здесь кратко описываются итоги проделанной работы.

# Список литературы{.unnumbered}

::: {#refs}
:::
