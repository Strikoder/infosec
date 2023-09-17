---
# Front matter
lang: ru-RU
title: "Отчёт по лабораторной работе №1"
subtitle: "Развертывание виртуальной машины"
author: "Яссин Мохамад Аламин НКНбд-01-20"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Получение практических навыков работы в консоли с атрибутами файлов, закрепление теоретических основ дискреционного разграничения доступа в современных системах с открытым кодом на базе ОС Linux.

# Теоретическое введение

Дискреционное разграничение доступа — управление доступом субъектов к объектам на основе списков управления доступом или матрицы доступа. Также используются названия дискреционное управление доступом, контролируемое управление доступом и разграничительное управление доступом. [2]

# Выполнение лабораторной работы

1. Создаем учетную запись пользлвателя guest. 


2. Задаем пароль для новой учетной записи.(@fig:002)

![Задание пароля](image/2.png){ #fig:002 width=100%}

3. Входим в новую учетную запись. Определяем директорию в которой находимся. Она не является домашней директорией, переходим в нее. (@fig:003)

4. Уточняем имя пользователя. (@fig:003)

5. Уточняем имя пользователя и его группу. Guest ходится с командной строкой. (@fig:003)

![Уточнение пользователя](image/3.png){ #fig:003 width=100%}

6. Смотрим файл /etc/passwd. ( @fig:005)



![Запись о guest в /etc/passwd](image/5.png){ #fig:005 width=100%}

7. Определяем существующие в системе директории. (@fig:006)

![Права на директориях](image/6.png){ #fig:006 width=100%}

8. Смотрим расширенные атрибуты установлены на поддиректориях, находящихся в директории /home. (@fig:007)

![Результат работы команды lsattr](image/7.png){ #fig:007 width=100%}

9. Создаем поддиректорию dir1 и определяем права доступа и расширенные атрибуты. (@fig:008)

![Создаем директорию dir1 и смотрим ее атрибуты](image/8.png){ #fig:008 width=100%}

10. Снимаем все атрибуты поддиректории. (@fig:009)

![Снятие атрибутов поддиректории dir1](image/9.png){ #fig:009 width=100%}

11. Пытаемся создать файл, не получается из-за запрета доступа. (@fig:010)

![Попытка создания файла](image/10.png){ #fig:010 width=100%}

12. Заполняем таблицу "Установленные права и разрешённые действия".

![таблица](image/11.png){ #fig:010 width=100%}
![таблица](image/12.png){ #fig:010 width=100%}


# Вывод

В ходе выполнения лабораторной работы был создан новый пользователь, были заполнены таблицы “Установленные права и разрешённые действия” и "Минимальные права для совершения операций” и получены навыки разграничения доступа в ОС Linux.

# Библиография

1. Методические материалы курса.
2. Wikipedia: Избирательное управление доступом. (URL: https://ru.wikipedia.org/wiki/%D0%98%D0%B7%D0%B1%D0%B8%D1%80%D0%B0%D1%82%D0%B5%D0%BB%D1%8C%D0%BD%D0%BE%D0%B5_%D1%83%D0%BF%D1%80%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5_%D0%B4%D0%BE%D1%81%D1%82%D1%83%D0%BF%D0%BE%D0%BC)
