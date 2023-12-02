---
## Front matter
title: "Отчет по лабораторной работе №8"
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
Приобретение навыков написания программ с использованием циклов и обработкой аргументов командной строки.

# Задание
1. Напишите программу, которая находит сумму значений функции f(x) для x = x1, x2, ..., xn, т.е. программа должна выводить значение f(x1) + f(x2) + ... + f(xn). Значения xi передаются как аргументы. Вид функции f(x) выбрать из таблицы 8.1 вариантов заданий в соответствии с вариантом, полученным при выполнении лабораторной работы № 7. Создайте исполняемый файл и проверьте его работу на нескольких наборах x = x1, x2, ..., xn.

# Выполнение лабораторной работы                                             |
[@gnu-doc:bash;@newham:2005:bash;@zarrelli:2017:bash;@robbins:2013:bash;@tannenbaum:arch-pc:ru;@tannenbaum:modern-os:ru]

Создаем каталог для программ лабораторной работы №8, переходим в него и
создаем файл lab8-1.asm:.
![Рис. 1.1: Создание файла lab8-1.asm.](image/1.1.jpg){#fig:001 width=70%}

Вводим в файл lab8-1.asm текст программы из листинга 8.1. Создаем исполняемый файл и проверяем его работу (рис. 1.2), (рис. 1.3).
![Рис. 1.2: Файл lab8-1.asm.](image/1.2.jpg){#fig:002 width=70%}
![Рис. 1.3: Запуск исполняемого файла.](image/1.3.jpg){#fig:003 width=70%}

Измените текст программы добавив изменение значение регистра ecx в цикле (рис. 1.4).
![Рис. 1.4: Файл lab8-1.asm.](image/1.4.jpg){#fig:004 width=70%}

Создаем исполняемый файл и запускаем его (рис. 1.5).
![Рис. 1.5: Запуск исполняемого файла(программа выведет бесконечное количество чисел).](image/1.5.jpg){#fig:005 width=70%}

Вносим изменения в текст программы добавив команды push и pop (добавления в стек и извлечения из стека) для сохранения значения счетчика цикла
loop (рис. 1.6).
![Рис. 1.6: Создание файла lab8-1.asm.](image/1.6.jpg){#fig:006 width=70%}

Создаем исполняемый файл и запускаем его (рис. 1.7).
![Рис. 1.7: Файл lab8-1.asm.](image/1.7.jpg){#fig:007 width=70%}

Создаем файл lab8-2.asm в каталоге ~/work/arch-pc/lab08 и вводим в него текст программы из листинга 8.2. (рис. 1.8).
![Рис. 1.8: Создание файла lab8-2.asm.](image/1.8.png){#fig:008 width=70%}
![Рис. 1.9: Файл lab8-2.asm.](image/1.9.jpeg){#fig:009 width=70%}

Создаем исполняемый файл и запускаем его, указав аргументы (рис. 1.10).
![Рис. 1.10: Запуск исполняемого файла.](image/1.10.jpg){#fig:010 width=70%}

Создаем файл lab8-3.asm в каталоге ~/work/arch-pc/lab08 и вводим в него текст программы из листинга 8.3. (рис. 1.11).
![Рис. 1.11: Создание файла lab8-3.asm.](image/1.11.png){#fig:011 width=70%}
![Рис. 1.12: Файл lab8-3.asm.](image/1.12.jpg){#fig:012 width=70%}

Создаем исполняемый файл и запускаем его, указав аргументы (рис. 1.13).
![Рис. 1.13: Запуск исполняемого файла.](image/1.13.jpg){#fig:013 width=70%}

Изменяем текст программы из листинга 8.3 для вычисления произведения аргументов
командной строки. (рис. 1.11).
![Рис. 1.14: Файл lab8-3.asm.](image/1.14.jpg){#fig:014 width=70%}
![Рис. 1.15: апуск исполняемого файла.](image/1.15.jpg){#fig:015 width=70%}

# Самостоятельная работа
Задание 1.
Пишем программу, которая находит сумму значений функции f(x) для x = x1, x2, ..., xn, т.е. программа должна выводить значение f(x1) + f(x2) + ... + f(xn). Значения xi передаются как аргументы. Вид функции f(x) выбрать из таблицы 8.1 вариантов заданий в соответствии с вариантом, полученным при выполнении лабораторной работы № 7. Создаем исполняемый файл и проверяем его работу на нескольких наборах x = x1, x2, ..., xn. (рис. 2.1).
![Рис. 2.1: Файл sr.asm.](image/2.1.jpg){#fig:016 width=70%}
![Рис. 2.2: Запуск исполняемого файла.](image/2.2.jpg){#fig:017 width=70%}


# Выводы
В ходе выполнения лабораторной работы мною были приобретены навыки написания программ с использованием циклов и обработки аргументов командной строки.

# Список литературы{.unnumbered}
::: {#refs}
:::
