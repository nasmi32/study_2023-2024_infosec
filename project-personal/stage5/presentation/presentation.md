---
## Front matter
lang: ru-RU
title: Презентация по этапу №5
subtitle: Основы информационной безопасности
author:
  - Мишина Анастасия Алексеевна
date: 9 мая 2024

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

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Мишина Анастасия Алексеевна
  * НПИбд-02-22
  
:::
::: {.column width="30%"}

:::
::::::::::::::

## Цель работы

- Научиться использовать Burp Suite для демонстрации реальных возможностей злоумышленников.

# Выполнение работы

## Burp Suite

![Включение перехвата в прокси](image/1.png){#fig:001 width=60%}

## Firefox

![Настройка прокси-сервера](image/2.png){#fig:002 width=50%}

## Полученные данные

![Перехват данных веб-приложения](image/3.png){#fig:003 width=70%}

## Ввод логина и пароля

![Запрос для входа в веб-приложение](image/4.png){#fig:004 width=70%}

## Попытка входа

![HTTP history](image/5.png){#fig:005 width=70%}

## Intruder

![Выбор позиций в Intruder](image/6.png){#fig:006 width=70%}


## Возможные логины

![Заполнение нагрузки username](image/7.png){#fig:007 width=30%}

## Возможные пароли

![Заполнение нагрузки password](image/8.png){#fig:008 width=30%}

## Результаты атаки

![Результаты атаки](image/9.png){#fig:009 width=70%}

## Ретранслятор

![Использование Repeater](image/10.png){#fig:010 width=70%}

## Ретранслятор

![Использование Repeater](image/11.png){#fig:011 width=70%}

## Выводы

- В ходе выполнения данной работы, я научилась использовать набор инструментов Burp Suite. Данный набор инструментов безопасности приложений является мощной платформой для атаки веб-приложений.


