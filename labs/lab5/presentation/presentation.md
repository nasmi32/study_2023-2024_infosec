---
## Front matter
lang: ru-RU
title: Лабораторная работа №5
subtitle: Основы информационной безопасности
author:
  - Мишина А. А.
date: 11 апреля 2024

## i18n babel
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

## Докладчик

- Мишина Анастасия Алексеевна
- НПИбд-02-22

# Выполнение лабораторной работы

## Цель работы

- Изучение механизмов изменения идентификаторов, применения SetUID- и Sticky-битов. Получение практических навыков работы в кон- соли с дополнительными атрибутами. Рассмотрение работы механизма смены идентификатора процессов пользователей, а также влияние бита Sticky на запись и удаление файлов.

## Файл simpleid.c

![Создание файла simpleid.c](image/1.png){#fig:001 width=70%}

## Файл simpleid.c

![Программа в файле simpleid.c](image/2.png){#fig:002 width=70%}

## Проверка

![Выполнение программы simpleid и команды id](image/3.png){#fig:003 width=70%}

## Усложнение

![Добавление вывода действительных идентификаторов](image/4.png){#fig:004 width=70%}

## Проверка

![Компиляция и запуск simpleid2](image/5.png){#fig:005 width=70%}

## Смена атрибута и владельца

![Запуск simpleid2 с SETUID. Сравнение результатов](image/6.png){#fig:006 width=70%}

## Смена атрибута и владельца

![Запуск simpleid2 с SETGID. Сравнение результатов](image/7.png){#fig:007 width=70%}

## Readfile.c

![Программа readfile](image/8.png){#fig:008 width=70%}

## Проверка

![Изменение прав доступа, проверка от имени пользователя guest](image/9.png){#fig:009 width=70%}

## Смена владельца и атрибута

![Установка SETUID для readfile, проверка](image/10.png){#fig:010 width=35%}

## file01.txt

![Проверка наличия атрибута Sticky на /tmp, работа с файлом file01.txt](image/11.png){#fig:011 width=50%}

## Атрибут t

![Снятие атрибута t (Sticky-бит), повторение операций](image/12.png){#fig:012 width=70%}

## Атрибут t

![Возвращение атрибута](image/13.png){#fig:013 width=70%}


## Вывод

- В ходе выполнения данной лабораторной работы, я изучила механизмы изменения идентификаторов, применения SetUID- и Sticky-битов. Получила практические навыки работы в консоли с дополнительными атрибутами. Рассмотрела работы механизма смены идентификатора процессов пользователей, а также влияние бита Sticky на запись и удаление файлов.