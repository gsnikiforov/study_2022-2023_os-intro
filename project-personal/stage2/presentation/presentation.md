---
## Front matter
lang: ru-RU
title: Индивидуальный Проект
subtitle: Этап 1
author:
  - Никифоров Г.С.
institute:
  - Российский университет дружбы народов, Москва, Россия

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---

# Информация

## Докладчик


  * Никифоров Георгий Сергеевич
  * Студент НММбд02-22
  * Российский университет дружбы народов
  * <https://github.com/gsnikiforov/gsnikiforov.github.io>

# Целеустремленность

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

## Заключение
Цель работы была достигнута: в результате выполнения данной работы была добавлена персональная информация и написаны две пробные публикации.

