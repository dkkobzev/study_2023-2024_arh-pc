---
## Front matter
title: "Отчет по лабораторной работе №2"
subtitle: "Архитектура компьютера"
author: "Дмитрий Константинович Кобзев"

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

Изучение идеологии и применение средств контроля версий. Приобретение практических навыков по работе с системой git.

# Задание

1. Создание отчет по выполнению лабораторной работы в соответствующем каталоге рабочего пространства (labs>lab02>report)

2. Скопируйте отчеты по выполнению предыдущих лабораторных работ в соответствующие каталоги созданного рабочего пространства.

3. Загрузите файлы на github.

# Выполнение лабораторной работы                                                |
[@gnu-doc:bash;@newham:2005:bash;@zarrelli:2017:bash;@robbins:2013:bash;@tannenbaum:arch-pc:ru;@tannenbaum:modern-os:ru]

Создаем учетную запись на сайте https://github.com/ и заполняем основные данные (рис. 1.1).
![Рис. 1.1: Учетная запись github.](image/1.1.png){#fig:001 width=70%}

Делаем предварительную конфигурацию git. Открываем терминал и вводим
следующие команды, указав имя и email владельца репозитория (рис. 1.2) .
![Рис. 1.2: Команды, содержащие имя и email.](image/1.2.png){#fig:002 width=70%}

Настраиваем utf-8 в выводе сообщений git (рис. 1.3).
![Рис. 1.3: Настройка utf-8 в выводе сообщений git.](image/1.3.jpg){#fig:003 width=70%}

Задаем имя начальной ветки(master) (рис. 1.4).
![Рис. 1.4: Имя начальной ветки.](image/1.4.jpg){#fig:004 width=70%}

Задаем параметр autocrlf (рис. 1.5).
![Рис. 1.5: Параметр autocrlf.](image/1.5.jpg){#fig:005 width=70%}

Задаем параметр safecrlf (рис. 1.6).
![Рис. 1.6: Параметр safecrlf.](image/1.6.jpg){#fig:006 width=70%}

Генерируем пару ключей (приватный и открытый) (рис. 1.7).
![Рис. 1.7: Генерация ключей.](image/1.7.jpg){#fig:007 width=70%}

Копируем ключ из локальной сети в буфер обмена (рис. 1.8).
![Рис. 1.8: Копирование ключа.](image/1.8.jpg){#fig:008 width=70%}

Загружаем сгенеренный открытый ключ (рис. 1.9).
![Рис. 1.9: SSH ключ.](image/1.9.jpg){#fig:009 width=70%}

Открываем терминал и создаем каталог для предмета “Архитектура компьютера” (рис. 1.10).
![Рис. 1.10: Каталог для предмета “Архитектура компьтера”.](image/1.10.jpg){#fig:010 width=70%}

Создаем репозиторий на основе шаблона (рис. 1.11).
![Рис. 1.11: Репозиторий курса.](image/1.11.jpg){#fig:011 width=70%}

Открываем терминал и переходим в каталог курса (рис. 1.12).
![Рис. 1.12: Каталог курса.](image/1.12.jpg){#fig:013 width=70%}

Клонируем созданный репозиторий (рис. 1.13).
![Рис. 1.13: Клонирование репозитория.](image/1.13.jpg){#fig:013 width=70%}

Переходим в каталог курса (рис. 1.14).
![Рис. 1.14: Каталог курса.](image/1.14.jpg){#fig:014 width=70%}

Удаляем лишние файлы (рис. 1.15).
![Рис. 1.15: Удаление лишних файлов.](image/1.15.jpg){#fig:015 width=70%}

Создаем необходимые каталоги (рис. 1.16).
![Рис. 1.16: Создание необходимых каталогов.](image/1.16.jpg){#fig:016 width=70%}

Отправляем файлы на сервер (рис. 1.17), (рис. 1.18), (рис. 1.19), (рис. 1.20), (рис. 1.21).
![Рис. 1.17: Отправление файлов на сервер.](image/1.17.jpg){#fig:017 width=70%}
![Рис. 1.18: Отправление файлов на сервер.](image/1.18.jpg){#fig:018 width=70%}
![Рис. 1.19: Отправление файлов на сервер.](image/1.19.jpg){#fig:019 width=70%}
![Рис. 1.20: Отправление файлов на сервер.](image/1.20.jpg){#fig:020 width=70%}
![Рис. 1.21: Отправление файлов на сервер.](image/1.21.jpg){#fig:021 width=70%}

Проверяем правильность создания иерархии рабочего пространства в локальном
репозитории и на странице github (рис. 1.22), (рис. 1.23).
![Рис. 1.22: Локальный репозиторий.](image/1.22.jpg){#fig:022 width=70%}
![Рис. 1.23: Репозиторий на github.](image/1.23.jpg){#fig:023 width=70%}

# Самостоятельная работа

Задание 1.

Создаем отчет по выполнению лабораторной работы в соответствующем каталоге
рабочего пространства (labs>lab02>report) (рис. 2.1).
![Рис. 2.1: Отчет по выполнению лабораторной работы каталоге (labs>lab02>report).](image/2.1.jpg){#fig:024 width=70%}

Задание 2.

Копируем отчеты по выполнению предыдущих лабораторных работ в соответствующие каталоги созданного рабочего пространства (рис. 2.2).
![Рис. 2.2: Отчет по выполнению 1 лабораторной работы каталоге (labs>lab01>report).](image/2.2.jpg){#fig:025 width=70%}

Задание 3.

Загружаем файлы на github (рис. 2.3).
![Рис. 2.3: Загрузка файлов на github.](image/2.3.jpg){#fig:026 width=70%}

# Выводы

В ходе выполнения лабораторной работы мною были изучены идеология и применение средств контроля версий. Приобретены практические навыки по работе с системой git.

# Список литературы{.unnumbered}

::: {#refs}
:::
