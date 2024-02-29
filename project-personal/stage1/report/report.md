---
## Front matter
title: "Отчёт по этапу №1"
subtitle: "Дисциплина: Основы информационной безопасности"
author: "Мишина Анастасия Алексеевна"

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

Получение практических навыков установки ОС на виртуальную машину. Установка дистрибутива Kali Linux [@infosec].

# Выполнение лабораторной работы

Для начала скачиваем образ ОС с официального сайта. Приступаем к созданию виртуальной машины, работа ведется в UTM. Выбираем нужный образ (рис. [-@fig:001]), указываем число оперативной памяти 4096 и ядер процессора (рис. [-@fig:002]), выделяем место под виртуальный жесткий диск 32 гб (рис. [-@fig:003]), даем имя виртуальной машине и сохраняем ее (рис. [-@fig:004]).

![Выбор образа](image/1.png){#fig:001 width=70%}

![Память и процессор](image/2.png){#fig:002 width=70%}

![Виртуальный жесткий диск](image/3.png){#fig:003 width=70%}

![Имя машины](image/4.png){#fig:004 width=70%}

Затем переходим в настройки и в разделе devices добавляем serial (рис. [-@fig:005]).

![Добавление девайса](image/5.png){#fig:005 width=70%}

Запускаем виртуальную машину и переходим к установке без графического интерфейса. Выбираем английский язык (рис. [-@fig:006]), выбираем местонахождение (рис. [-@fig:007]), настраиваем клавиатуру (рис. [-@fig:008]), вводим имя хоста (рис. [-@fig:009]), создаем пользователя (рис. [-@fig:010]) и вводим пароль (рис. [-@fig:011]).

![Выбор языка](image/6.png){#fig:006 width=70%}

![Выбор местонахождения](image/7.png){#fig:007 width=70%}

![Клавиатура](image/8.png){#fig:008 width=70%}

![Имя хоста](image/9.png){#fig:009 width=70%}

![Имя пользователя](image/10.png){#fig:010 width=70%}

![Создание пароля](image/11.png){#fig:011 width=70%}

Переходим к разбиению диска, выбираем использование всего диска (рис. [-@fig:012]), также выбираем наш виртуальный жесткий диск (рис. [-@fig:013]).

![Разбиение диска](image/12.png){#fig:012 width=70%}

![Выбор виртуального жесткого диска](image/13.png){#fig:013 width=70%}

Выбираем разбиение для новых пользователей (рис. [-@fig:014]), заканчиваем его (рис. [-@fig:015]) и записываем изменения на диск (рис. [-@fig:016]).

![Разбиение диска](image/14.png){#fig:014 width=70%}

![Разбиение диска](image/15.png){#fig:015 width=70%}

![Разбиение диска](image/16.png){#fig:016 width=70%}

Выбираем стандартное программное обеспечение для Kali Linux, предложенное системой (рис. [-@fig:017]) и завершаем установку (рис. [-@fig:018]).

![Программное обеспечение](image/17.png){#fig:017 width=70%}

![Завершение установки](image/18.png){#fig:018 width=70%}

Затем выключаем виртуальную машину (рис. [-@fig:019]), отключаем образ (рис. [-@fig:020]) и удаляем девайс serial (рис. [-@fig:021]).

![Выключение виртуальной машины](image/19.png){#fig:019 width=70%}

![Отключение образа](image/20.png){#fig:020 width=70%}

![Удаление девайса](image/21.png){#fig:021 width=70%}

Запускаем виртуальную машину, после загрузки вводим данные пользователя - логин и пароль (рис. [-@fig:022]).

![Ввод логина и пароля](image/22.png){#fig:022 width=70%}

Открываем терминал и убеждаемся, что система установлена успешно (рис. [-@fig:023]).

![Проверка имени пользователя и хоста](image/23.jpg){#fig:023 width=70%}

# Выводы

В ходе выполнения данной лабораторной работы, я приобрела практические навыки установки операционной системы Kali Linux на виртуальную машину UTM. В ходе работы были настроены минимально необходимые для дальнейшей работы сервисы, установлено необходимое ПО. 

# Список литературы{.unnumbered}

::: {#refs}
:::
