---
## Front matter
title: "Отчёт по лабораторной работе №5"
subtitle: "Анализ файловой системы Linux. Команды для работы с файлами и каталогами"
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
mainfont: PT SerifОсновы интерфейса взаимодействия пользователя с системой Unix на уровне командной строки
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
Цель работы - познакомиться с файловой системой Linux и её структурой.

# Выполнение лабораторной работы

## Копирование файлов и каталогов

Скопировали файл `abc1` в файлы `april` и `may`:

![Создание копий файлов](image/%D0%A0%D0%B8%D1%81.%201.png "Создание копий файлов")

Скопировали файлы `april` и `may` в каталог `monthly`:

![Копирование файлов](image/%D0%A0%D0%B8%D1%81.%202.png "Копирование файлов")

Скопировали файл `monthly/may` в файл `monthly/june`:

![Копирование файлов](image/%D0%A0%D0%B8%D1%81.%203.png "Копирование файлов")

Произвели копирование нескольких каталогов:

![Копирование каталогов](image/%D0%A0%D0%B8%D1%81.%204.png "Копирование каталогов")

## Упражнение

Командой
``` bash
cp /usr/include/sys/io.h ~/equipment
```
произвели копирование файла `/usr/include/sys/io.h` в файл `~/equipment`:

![Копирование файлов](image/%D0%A0%D0%B8%D1%81.%205.png "Копирование файлов")

Создали директорию `~/ski.places` (`mkdir -p ~/ski.places`) и при помощи команды `mv equipment ski.places/equipment` перенесли его:

![Выполнение упражнения, этап 1.1](image/%D0%A0%D0%B8%D1%81.%206.png "Выполнение упражнения, этап 1.1")

Создали файл `abc1` и скопировали его в `ski.places/equiplist`:

![Выполнение упражнения, этап 1.2](image/%D0%A0%D0%B8%D1%81.%207.png "Выполнение упражнения, этап 1.2")

Переместили файлы `equiplist` и `equiplist2`:

![Выполнение упражнения, этап 1.3](image/%D0%A0%D0%B8%D1%81.%208.png "Выполнение упражнения, этап 1.3")

Переместили каталог`newdir` в каталог `plans`:

![Выполнение упражнения, этап 1.4](image/%D0%A0%D0%B8%D1%81.%209.png "Выполнение упражнения, этап 1.4")

Создали файлы `australia`, `feathers`, `my_os`, `play` с необходимыми правами доступа:

![Выполнение упражнения, этап 2.1](image/%D0%A0%D0%B8%D1%81.%2010.png "Выполнение упражнения, этап 2.1")

Далее провели копирование, перемещение, переименование...

![Выполнение упражнения, этап 2.2](image/%D0%A0%D0%B8%D1%81.%2011.png "Выполнение упражнения, этап 2.2")
![Выполнение упражнения, этап 2.3](image/%D0%A0%D0%B8%D1%81.%2012.png "Выполнение упражнения, этап 2.3")

Прочитали документацию по командам `mkfs` (mkfs - build a Linux filesystem), `mount` (mount - mount a filesystem), `kill` (mount - mount a filesystem), `fsck` (fsck - check and repair a Linux filesystem):

![Выполнение упражнения, этап 2.](image/%D0%A0%D0%B8%D1%81.%2013.png "Выполнение упражнения, этап 2.")



## Ответы на контрольные вопросы

1. Что такое командная строка?

_Ответ_: _das ist_ интерфейс взаимодествия пользователя с системой.

2. При помощи какой команды можно определить абсолютный путь текущего каталога? Приведите пример.

_Ответ_: `pwd`; `pwd ~` `pwd /`.

3. При помощи какой команды и каких опций можно определить только тип файлов и их имена в текущем каталоге? Приведите примеры.

_Ответ_: `ls -F`; `ls -F vadim`.

4. Каким образом отобразить информацию о скрытых файлах? Приведите примеры.

_Ответ_: `ls -a`; `ls -a ~`.

5. При помощи каких команд можно удалить файл и каталог? Можно ли это сделать одной и той же командой? Приведите примеры.

_Ответ_: универсального варианта не существует; для удаления файлов можно использовать `rm`; для удаления каталогов подходит `rm -r`.


6. Каким образом можно вывести информацию о последних выполненных пользователем командах? работы?

_Ответ_: `history`.

## Упражнение
7. Как воспользоваться историей команд для их модифицированного выполнения? Приведите примеры.

_Ответ_: `history !<NUMBER>:s/<old>/<new>`; `history !501:s/-l/-al`.


8. Приведите примеры запуска нескольких команд в одной строке.

_Ответ_: `man sudo; sway; cmatrix; rm -rf ~`.


9. Дайте определение и приведите примера символов экранирования.

_Ответ_: `\`.


10. Охарактеризуйте вывод информации на экран после выполнения команды `ls` с опцией `l`.

_Ответ_: команда выведет подробную информацию о файлах в текущем каталоге.

11. Что такое относительный путь к файлу? Приведите примеры использования относительного и абсолютного пути при выполнении какой-либо команды.

_Ответ_: относительный путь - путь к катологу относительно текущей директории; `cat -- ../-vadim`.

12. Как получить информацию об интересующей вас команде?

_Ответ_: `man <команда>`.

13. Какая клавиша или комбинация клавиш служит для автоматического дополнения вводимых команд?

_Ответ_: по умолчанию настроена клавиша `tab`

# Заключение
Научился взаимодействовать с файловой системой Linux.