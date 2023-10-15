---
## Front matter
lang: ru-RU
title: Защита лабораторной работы №6. Мандатное разграничение прав в Linux.
author: Яссин Мохамад Аламин
group: NI-402
institute: RUDN University, Moscow, Russian Federation
date: 14 октября 2023

## Formatting
toc: false
slide_level: 2
theme: metropolis
header-includes: 
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
aspectratio: 43
section-titles: true
---

# Прагматика выполнения лабораторной работы

- навыки работы с SELinux и Apache
- знакомство с файлами html

# Цель выполнения лабораторной работы

- развить навыки администрирования ОС Linux
- получить первое практическое знакомство с технологией SELinux
- проверить работу SELinux на практике совместно с веб-сервером Apache

#  Выполнение лабораторной работы

## Создание программы

- подготовили лабораторный стенд
- проверили режим и политику SELinux
- запустили Apache
- определяли тип файлов в /var/www
- создали файл test.html
- открыли его через веб-браузер
- сменили контекст
- сменили прослушиваемый TCP-порт с 80 на 81
- добавили порт 81 в список
- открыли файл через веб-браузер
- вернули порт с 81 на 80
- удалили 81 порт из списка
- удалили файл test.html

# Результаты выполнения лабораторной работы

- были развиты навыки администрирования ОС Linux
- была проверена работа SELinux на практике совместно с веб-сервером Apache
