---
## Front matter
lang: ru-RU
title: Лабораторная работа №6
subtitle: Основы информационной безопасности
author:
  - Мишина А. А.
date: 25 апреля 2024

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

- Развить навыки администрирования ОС Linux. Получить первое прак- тическое знакомство с технологией SELinux1. Проверить работу SELinx на практике совместно с веб-сервером Apache.

## SELinux, веб-сервер Apache

![Проверка режима SELinux, запуск веб-сервера](image/1.png){#fig:001 width=50%}

## SELinux, веб-сервер Apache

![Контекст безопасности веб-сервера и состояние переключателей SELinux](image/2.png){#fig:002 width=50%}

## Статистика

![Статистика по политике](image/3.png){#fig:003 width=40%}

## /var/www и /var/www/html

![Определение типов файлов и поддиректорий www и html. Создание файла test.html](image/4.png){#fig:004 width=70%}

## test.html

![Файл test.html](image/5.png){#fig:005 width=70%}

## Контекст test.html

![Контекст файла test.html](image/6.png){#fig:006 width=70%}

## Браузер

![Запуск файла в браузере](image/7.png){#fig:007 width=70%}

## Man и контекст файла

![Изучение справок, контекст файла test.html](image/8.png){#fig:008 width=70%}

## Смена контекста

![Смена контекста файла, проверка](image/9.png){#fig:009 width=70%}

## Браузер

![Попытка просмотра](image/10.png){#fig:010 width=70%}

## Права доступа, лог-файл

![Права доступа, системный log-файл](image/11.png){#fig:011 width=50%}

## httpd.conf

- Смена TCP-порта на 81

![Файл httpd.conf](image/12.png){#fig:012 width=70%}

## Сервер apache

![Перезапуск веб-сервера Apache](image/13.png){#fig:013 width=70%}

## Браузер

![Сбой веб-сервера](image/14.png){#fig:014 width=30%}

## Лог-файлы

![Просмотр лог-файлов](image/15.png){#fig:015 width=70%}

## Лог-файлы

![Просмотр лог-файлов](image/16.png){#fig:016 width=70%}


## Порты

![Проверка списка портов, перезагрука сервера, возвращение контекста](image/17.png){#fig:017 width=70%}

## Браузер

![Просмотр файла через сервер](image/18.png){#fig:018 width=70%}


## httpd.conf

![Файл httpd.conf](image/19.png){#fig:019 width=70%}


## Удаление

![Удаляем привязку http_port_t к 81, выполняем проверку, удаляем файл test.html](image/20.png){#fig:020 width=70%}


## Вывод

- В ходе выполнения данной лабораторной работы, я развила навыки администрирования ОС Linux, получила первое практическое знакомство с технологией SELinux1, а также проверила работу SELinx на практике совместно с веб-сервером Apache.