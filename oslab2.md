---
# Front matter
title: "Лабораторная работа 2"
subtitle: "Отчёт"
author: "Новосельцев Данила Сергеевич"

# Generic otions
lang: ru-RU
toc-title: "Содержание"

# Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

# Pdf output format
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
### Fonts
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
## Misc options
indent: true
header-includes:
  - \linepenalty=10 
  - \interlinepenalty=0 
  - \hyphenpenalty=50 
  - \exhyphenpenalty=50 
  - \binoppenalty=700 
  - \relpenalty=500 
  - \clubpenalty=150 
  - \widowpenalty=150 
  - \displaywidowpenalty=50 
  - \brokenpenalty=100 
  - \predisplaypenalty=10000 
  - \postdisplaypenalty=0 
  - \floatingpenalty = 20000 
  - \raggedbottom 
  - \usepackage{float} 
  - \floatplacement{figure}{H} 
---

# Лабораторная работа 2
 Новосельцев.Д.С. 
 НФИбд-02-20

---

# Цель работы

Изучить идеологию и применение средств контроля версий.

---

# Ход работы

Для начала работы я создал учетную запись в github.

--- 

Для работы с сервером репозиториев я создал ssh-ключ с помощью команды ssh-keygen. После я скопировал его данные и через github вставил их в поле 'key'

![](https://imgur.com/eRV1exN.png)
![](https://imgur.com/gwkv4jm.png)
![](https://imgur.com/PdhhANo.png)

---

Я создал пустой репозиторий lab2 для дальнейшей работы с ним.

![](https://imgur.com/VJvJ7m7.png)

---

Для подключения репозитория к github я действовал по инструкции, предоставленной самим GitHub

![](https://imgur.com/YkpLord.png)

---

Первичной конфигурацией я использовал создание файла лицензии.

![](https://imgur.com/ZvV0nqb.png)

---

![](https://imgur.com/kUBNVky.png)

---
После добавления шаблонов конфигурируемых файлов я выполнил коммит и отправил на гитхаб.

![](https://imgur.com/hqovU9C.pdf)

---

Я инициализировал git flow и создал новый релиз, указав версию и дбавив индекс.

![](https://imgur.com/KTl4kYb.png)

---

После чего я залил релиз на github.

![](https://imgur.com/DHPID8H.png)

---

Изначально программа мне не позволила сделать релиз, так как не доверяла моему ключу. Я вручную доверился этому ключу.
![](https://imgur.com/xnHBiFI.png)

Итог
![](https://imgur.com/A1EGByY.png)

# Вывод:
Я изучил идеологию и применение средств контроля версий.


---

# Ответы на контрольные вопросы:
1. система контроля версий позволяет их фиксировать, совмещать изменения,
произведённые разными участниками проекта, производить откат к любой более
ранней версии проекта, если это требуется.
2. • некоторое место, где хранятся файлы
• commit - отдельная версия программы
• история - информация о всех изменениях в проекте
• рабочая копия - текущее состояние файлов проекта
3. децентрализованные хранятся на многих устройствах и передаются многим
устройствам(Mercurial), централизованные - файлы хранятся в одном устройства(CVS)
4. изменяем, делаем коммиты, закидываем на репозиторий, если необходимо делаеи
релизы.
5. делаем пул нынешних изменений, изменяем, добавляем свои изменения в ветку,
коммиты и т.д.
6. контроль версиями, одновременная работа нескольких людей над 1 проектом и многое
другое
7. -init = инициализация локального репозитория -status = показ всех измененных и
добавленных в коммит файлов -add = добавление файлов
8. проект с закрытым исходным кодом используют локальные репозитории, проекты с
открытым исходным кодом, проекты выполняемые несколькими людьми, удаленно -
удаленные репозитории
9. ветки используются для удобства работы с версиями и изминениями программы
10. многие конфигурационные файлы с личными или важными файлами не должны бытб
доступны, а также есть примеры папок/файлов, которые создаются для кэширования,
которые независимы от проекта и от которых проект не зависит.