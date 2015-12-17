---
layout: page
title:  Программное обеспечение
categories: software
permalink: /software/
---

## Вступление

Выбор базовой ОС определяет всё. Все реальные и потенциальные возможности.
Выбор специализированной _сборки_ определяет только удобства на старте и геморрой на финише. - **Krey**

На реальном/виртуальном железе пособирайте разные варианты NAS.
Возьмите три диска (хватит для RAID5), настройте каждый NAS до: 

* каталоги видны по SMB c нужными правами 
* качаются торренты 
* настроен бэкап на четвертый диск. 

Уйдет пара дней, зато все станет понятно. - **ewizard**

## Примерный алгоритм выбора софта для домашнего NAS

[![Выбор ПО для NAS](/files/soft4nas_choosing.svg)](/files/soft4nas_choosing.svg)

## Готовые популярные сборки

### Выбор

__Q.__ Если у меня атом и один диск, где скорость по сети выше будет? Надежность не нужна
(не то что бы совсем не нужна, но скорость важнее)<br />
__A.__ Посмотрите Linux, из сборок - OMV. В конференции были сообщения о полной утилизации 
гигабита под OMV на атоме. **MikeMac**

__Q.__ В чем плюсы и минусы ZFS?<br />
__A.__ [Зачем ZFS дома](http://2gusia.livejournal.com/7545.html)

__Q.__ C программированием не знаком, а \*nix никогда и не видел, хочется что-то простое<br />
__A.__ Покупные NAS, все роутеры и т.д. и т.п. работают на юникс/линукс.
Общее представление по этим системам не помешает. **Сергей789**<br />
Поставьте на основной комп виртуалку. Попробуйте в ней nas4free и/или omv.
[Это предельно просто](http://2gusia.livejournal.com/22902.html) **MikeMac**

### Nas4free (развитие FreeNAS 0.7.x)

*   [Официальный сайт](http://www.nas4free.org/) (англ.)
*   [nas4free wiki](http://wiki.nas4free.org/doku.php) (англ.)
*   [nas4free forum](http://forums.nas4free.org/index.php) (англ.)
*   [русскоязычный форум](http://forums.nas4free.org/viewforum.php?f=44&sid=603e23082349bac63b5d8c9e50a5580a)
*   [Русскоязычная инфа - установка, настройка, железо...](http://2gusia.livejournal.com/30360.html)
*   [Тюнинг NAS4Free](http://forum.ixbt.com/topic.cgi?id=4:127822:3686#3686) от **Sergei V. Sh** Прим. **MikeMac** loader.conf с 847 версии правится через вебгуй аналогично rc.conf
*   [Подробнее про тюнинг](http://forum.ixbt.com/topic.cgi?id=4:127864:2353#2353) от **thedix**
*   [rc.conf Cheat Sheet](http://forums.nas4free.org/viewtopic.php?f=75&t=204)
*   [перенаправление log](http://wiki.nas4free.org/doku.php?id=faq:0134)
*   [Установка collectd на nas4free](http://forum.ixbt.com/topic.cgi?id=4:127822:2815#2815) от **jenci**
*   [безопасный доступ снаружи к NAS](http://forum.ixbt.com/topic.cgi?id=4:127819-137#4076) от **Sergei V. Sh**
*   [внешний доступ к серверу FTP+TLS на nas4free](http://forum.ixbt.com/topic.cgi?id=109:82:2637#2637) от **Krutilator**

__Q.__ На Самбе при включении Max Protocol SMB2 происходят обрывы передачи.<br />
__A.__ Из-за бага в samba 3.6.x SMB2 совместо с AIO не работает. Отключите AIO или замените SMB2 на NT1.

__Q.__ Можно ли импортировать zfs пул, например, созданный во FreeNAS.<br />
__A.__ Да. ```Disks|ZFS|Configuration|Synchronize```

__Q.__ Подключил диск, названия (ada1, ada2...) дисков поехали.<br />
__A.__ Сохраняем конфиг на всякий случай, идём в ```Disks|Management```,
кнопки ```Import Disks``` или ```Clear Config``` and ```Import disks```.
При необходимости затем ```Disks|ZFS|Configuration|Synchronize```

### OMV - OpenMediaVault

*   [Официальный сайт](http://openmediavault.org/) (англ.)
*   [OMV wiki](http://wiki.openmediavault.org/index.php?title=Main_Page) (англ.)
*   [Русское пошаговое руководство по установке](http://macrodmin.blogspot.com/2012/03/openmediavault-nas.html)
*   [Ветка на форуме ixbt.com](http://forum.ixbt.com/topic.cgi?id=11:44112)

### FreeNAS (бесплатный вариант TrueNAS от IX Systems)

*   [Официальный сайт](http://www.freenas.org/) (англ.)
*   [Документация](http://doc.freenas.org) (англ.)

#### Отзывы о версии 8.3 (устаревшая версия)

От FreeNAS пришлось отказаться.

1. SMART демон не запустился, причём продиагностировать ошибку по скупому «failed» оказалось невозможно.
На официальном форуме ничего внятного поиском не нашёл.
2. Температуру HDD в гуе не показывает, предполагается, что ты можешь получать только нотификации о
критических значениях по SMART (который не заработал).
3. Концепция jail изначально показалась интересной. В реальности надо назначать ip вручную
(я предпочитаю дома ip раздавать по dhcp), примонтировать датасет в jail - это очень длинная
многоходовка (которая мне так и не далась).

В целом, управление дисками, zfs, шарами во FreeNAS гораздо удобнее, всё остальное в Nas4Free сделано удобнее.
Хотя главное, из-за чего отказался, это из-за неработающего SMAR - **Alex M. Jake**

«Я тоже не смог SMART запустить на FreeNAS. Последствия Вы все знаете - посыпавшиеся винты, а я ни сном, ни духом»
- **Dimonizer**

## OC общего назначения

По результатам голосования в теме чуть более 50% используют BSD,
~ по 20% Windows и Linux и около 8% - Solaris

### Windows

* [Информация по Windows вынесена сюда](/software/windows/)
* [Soft RAID1 под Windows7](http://winitpro.ru/index.php/2011/04/30/kak-sozdat-programmnyj-raid-v-windows-7/)

### Unix-семейство

*   [Настройка прав на сетевую SAMBA папку из под Windows](http://forum.ixbt.com/topic.cgi?id=4:127822:3556#3556)
    _How to_ от **kostya_1983**
*   [Сборник скриптов от участников темы](https://github.com/Shesternin/NAS-HandMade)
*   [Шифрование файлов в Linux и FreeBSD](http://ramzess.ru/shifrovanie-fajlov-v-linux-i-freebsd/)
*   [Насколько сильно Transmission грузит процессор?](http://forum.ixbt.com/topic.cgi?id=4:127819-106#3120)
*   [Transmission качает медленно на широком канале](http://forum.ixbt.com/topic.cgi?id=4:127805-76#2316)
ответ от **RU_Taurus** и результат - см далее по ветке
*   [Шпаргалка: Active Directory, CIFS/SMB](http://forum.ixbt.com/topic.cgi?id=109:4-42#1240) от **Mikluhamaklay**

#### Linux

Проект, посвященный портированию ZFS на Linux - [ZfsOnLinux](http://zfsonlinux.org/) (кратко **ZoL**).
При этом работу ведут отнюдь не любители-энтузиасты, а известнейшие в узких кругах программисты под
крылом _Lawrence Livermore National Laboratory_.

При этом ZFS в лаборатории используется как back-end файловая система для популярной кластерной
системы Lustre. ZoL в данный момент вполне стабилен и работоспособен, как минимум, в домашнем NAS.

#### BSD-семейство (FreeBSD, PC-BSD...)

* [Установка FreeBSD на zfs пул](https://wiki.freebsd.org/RootOnZFS/GPTZFSBoot/9.0-RELEASE)
* [Установка FreeBSD на зашифрованный USB-носитель](http://forum.ixbt.com/topic.cgi?id=4:127864-166#4807) от __RU_Taurus__
* [Перемещение интенсивных на запись каталогов FreeBSD в пространство zfs-пула.](
http://forum.ixbt.com/topic.cgi?id=4:127864-7#190) от __RU_Taurus__
* [Защищенный шифрованием удалённый backup NAS](http://forum.ixbt.com/topic.cgi?id=4:127819-130#3826) от __Oleg__
* [О настройке transmission](http://forum.ixbt.com/topic.cgi?id=109:4:2495#2495) от __RU_Taurus__
* О разграничении прав доступа от __RU_Taurus__
  * [NAS своими руками (часть 5), #3067](http://forum.ixbt.com/topic.cgi?id=11:43718:3067#3067)
  * [NAS своими руками (часть 5), #3330](http://forum.ixbt.com/topic.cgi?id=11:43718:3330#3330)
* [Защита от переборщиков паролей](http://forum.ixbt.com/topic.cgi?id=4:127805-94#2797) от **WearWolf**
* [Баг в AHCI-стеке FreeBSD 10.1 и лечение](http://forum.ixbt.com/topic.cgi?id=4:127805-94#2800)
от **MethroGnome**. См также пост **RU_Taurus** там же чуть ниже

#### Solaris (Illumos, OpenIndiana, Nexenta, SmartOS...)

Т.к. использование Solaris требует заметной квалификации, мы попросили пользователей ответить на вопросы.

##### Вопросы

1.  какие преимущества дает Солярка
2.  что на ней сделать нельзя или весьма затруднительно
3.  что советуете изучать желающим двигаться в эту сторону

А более детального <abbr title="Frequently Asked Questions">FAQ</abbr> тут мы избежим.
Новичку с парой вечеров свободных тут делать нечего, а продвинутые со временем - разберутся.

##### Ответы

* **#term** [NAS своими руками (часть 6), #2203](http://forum.ixbt.com/topic.cgi?id=4:127822:2203#2203)
* **archa** [NAS своими руками (часть 6), #2263](http://forum.ixbt.com/topic.cgi?id=4:127822:2263#2263)
* [Установка deluge-1.3.3 на Solaris](http://forum.ixbt.com/topic.cgi?id=4:127822:2438#2438) от **Brainstem**
* [Cборка свежего transmission-daemon на Solaris 11](http://forum.ixbt.com/topic.cgi?id=11:43718:3540#3540) от **Archer13**

## Мультиплатформное ПО

### transmisson-remote-gui

[Программа](http://sourceforge.net/projects/transgui/) для управления Transmission,
существенно превосходящая по функциональности встроенный веб интерфейс.

### iozone

Команда на тестирование

```sh
iozone -i0 -i1 -i2 -s10g -r128k -f /mnt/storage
```
где  
i0 - тестировать линейное чтение  
i1 - тестировать линейную запись  
i2 - тестировать случайные операции  
s - объем тестового паттерна (должен быть более объема RAM)  
r - размер блока (128К для zfs)  
f - каталог для теста (без указания тестирует в текущем) **RU_Taurus**

## Виртуализация NAS  

### VMware vSphere ESXI

* [Корректное завершение работы AiO: Esxi и ИБП APC Back-UPS USB](http://forum.ixbt.com/topic.cgi?id=4:127805-91#2712)
от **student81**
