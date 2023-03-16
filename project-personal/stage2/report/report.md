---
## Front matter
title: "Отчёт по выполнению индивидуального проекта"
subtitle: "Этап 2"
author: "Никифоров Георгий Сергеевич"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
## bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: false # List of tables
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

## Цель работы
Цель настоящей работы - Добавить информацию о себе и написать тестовый пост. Репозитории проекта размещёны по адресам [https://github.com/gsnikiforov/wine-tyan](https://github.com/gsnikiforov/wine-tyan) и [https://github.com/gsnikiforov/gsnikiforov.github.io](https://github.com/gsnikiforov/gsnikiforov.github.io).

# Выполнение этапа 2

## Предварительная настройка

Чтобы видеть изменения в реальном времени, мы, находясь в директории персонального сайта, ввели команду

``` bash
~/bin/hugo server
```

В конце вывода она напечатала в консоль адрес запущенного локального сервера:
Копируя его и вставляя в строку поиска браузера, мы попадаем на локальный сервер. При любом сохранённом изменении он перезагрузит своё содержимое, что крайне удобно.

## Добавление информации о себе

Редактируя файл `content/authors/admin/_index.md`, мы изменили информацию о себе. Заменяя файл `content/authors/admin/avatar.jpg` на любое другое изображение с названием _avatar_, мы смогли изменить персональное фото:

![Изменение персональной информации](image/Рис.%202.png "Изменение персональной информации")

## Добавление первого поста

Далее мы скопировали папку `post/getting-started` с любым другим именем (в моём случае это `post/Week 0`). Далее поменяли изображение `post/Week 0/featured.jpg` на любое другое (важно, чтобы оно нзывалось _featured_) и файл `post/Week 0/_index.jpg`:

![Первый пост](image/Рис.%203.png "Первый пост")

## Добавление второго поста

Аналогичной процедурой создали второй пост о системе контроля версий Git:

![Второй пост](image/Рис.%204.png "Второй пост")

# Заключение
Цель работы была достигнута: в результате выполнения данной работы была добавлена персональная информация и написаны две пробные публикации.
