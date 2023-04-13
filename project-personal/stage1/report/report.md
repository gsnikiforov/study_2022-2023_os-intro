---
## Front matter
title: "Индивидуальный проект"
subtitle: "Этап 1"
author: "Никифоров Георгий Сергеевич"

## Generic otions
lang: ru-RU
toc-title: "Ход работы"

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

Создать сайт, привязанный к созданным репозиториям

# Задание

# Теоретическое введение



# Выполнение лабораторной работы

Создал репозиторий для сайта


![Создание репозитория сайта](image/image1.png)


Клонировал его на ПК


![git clone](image/image2.png)


Проверил файлы


![Проверка](image/image3.png)


Удалил паблик


![Удаление овсянки](image/image4.png)


Вызвал хюго сервер


![Hugo server](image/image5.png)


Получил локалхост


![Сайт по локалке](image/image6.png)


Создаем пустой доп репозиторий с основными файлами сайта


![rep.github.io](image/image7.png)


Создал в репозитории текст файл и подключил репозиторий к основной ветке


![Ветка main](image/image8.png)


Объединил репозитории по ветке main


![Submodule](image/image9.png)


Закомментировал public


![Комментирование](image/image10.png)


Объединил по мейн ветке с учетом игнорирования паблик


![Submodule!](image/image11.png)


git pushнул


![git push](image/image12.png)


САЙТЁ!!!!!!!!!!


![САЙТБИЛНСАТЙ МОЙСАЙТИК](image/image13.png)



# Выводы

Сделал локальный сайт объеденный с репозиториями, научился этому)))))))

# Список литературы{.unnumbered}

::: {#refs}
:::
