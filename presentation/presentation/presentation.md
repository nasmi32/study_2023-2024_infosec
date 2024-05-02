---
## Front matter
lang: ru-RU
title: Система PGP
subtitle: Основы информационной безопасности
author:
  - Мишина А. А. НПИбд-02-22
date: 02 мая 2024

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

## Введение

:::::::::::::: {.columns align=center}
::: {.column width="50%"}

PGP (Pretty Good Privacy) - 1991 г. 

* Секретность
* Установление подлинности
* Удобство

:::
::: {.column width="50%"}

![Филипп Циммерман](image/1.jpeg){width=60%}

:::
::::::::::::::

## Основные принципы PGP

- Наличие открытого и закрытого ключа.
- Возможность кодирования и подписи файлов.
- Сертификат ключа - индентификатор пользователя, ключ, дата создания.
- Keyring - хранилище пар ключей, сертификатов.

## PGP в Ubuntu

:::::::::::::: {.columns align=center}
::: {.column width="50%"}

- GPG – GNU Privacy Guard
- Бесплатный аналог PGP

:::
::: {.column width="50%"}

![Общая схема шифрования и дешифрования](image/2.png){width=90%}

:::
::::::::::::::

## Установка GPG

![Установка GPG](image/3.png){width=60%}

## Основные опции GPG

![Опции gpg](image/4.png){width=60%}

## Генерация ключей

![Создание пары ключей](image/5.png){width=45%}

## Состав ключа

![Состав ключа](image/6.png){width=70%}

## Экспорт

![Экспорт ключа](image/7.png){width=45%}

## Импорт

![Передача ключа](image/8.png){width=70%}

![Импорт ключа](image/9.png){width=70%}

## Файл

![Создание секретного файла](image/10.png){width=70%}

![Файл secret_file.txt](image/11.png){width=60%}

## Шифрование

![Создание подписи файла, шифрование файла](image/12.png){#fig:013 width=70%}

## Результаты

![Файл цифровой подписи](image/13.png){#fig:014 width=70%}

![Зашифрованный файл с текстом](image/14.png){#fig:015 width=70%}

## Дешифрование

![Дешифровка и проверка подписи](image/15.png){#fig:016 width=70%}

![Просмотр дешифрованного файла](image/16.png){#fig:017 width=70%}

## Выводы

- PGP эффективен.
- Применение: защита личной переписки, шифрование дисков, безопасность бизнеса, обмен файлами, работа с github.
- Свободный доступ системы PGP.