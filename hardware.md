---
layout: page
title:  Аппаратное обеспечение
categories: hardware
permalink: /hardware/
---

## Примеры конфигураций

* [180TB of Good Vibrations – Storage Pod 3.0](http://blog.backblaze.com/2013/02/20/180tb-of-good-vibrations-storage-pod-3-0/) 
  описание  (англ) системы на 45 HDD. тем не менее использованные компоненты и глава "выученные уроки" интересны и для менее масштабных NAS. 
  [фоторепортаж](http://www.45drives.com/wiki/index.php/Screenshot_assembly_tour)
* [NAS своими руками (часть 4), #2015](http://forum.ixbt.com/topic.cgi?id=11:43009:2015#2004) от **Padavan** Pentium G840, 8GB, 6 шт 
  3.5 дисков +1 шт 2.5\. Ссылка на [фото](http://forum.ixbt.com/post.cgi?id=attach:11:43009:770:1) - весьма компактно. 
  К сожалению, использованную мать Asus P8H67-I, которая с 6 SATA(!) в отличие от более поздних - уже весьма трудно найти
* [NAS своими руками (часть 6), #2004](http://forum.ixbt.com/topic.cgi?id=11:44215:2004#2004) от **ZanZag** 
  Pentium G860, 16Gb, CF 4gb, zfs raidz2 of 6x3Tb, много фото
* [NAS своими руками (часть 6), #2012](http://forum.ixbt.com/topic.cgi?id=11:44215:2012#2012) от **ZanZag** 
  Dual-Core E5400, 8Gb, zfs raidz1 6×1.5Tb, и ещё много места. Обильно сфотографировано и существенно доработано напильником.
*   [NAS своими руками (часть 6), #2019](http://forum.ixbt.com/topic.cgi?id=11:44215:2019#2019)
от **RU_Taurus** Pentium E6700 3200, 8Гб, LSI SAS 3081E-R, 12 HDD + 1 системный. Весьма основательная сборка, но еще на LGA775
*   [NAS своими руками (часть 6), #1650](http://forum.ixbt.com/topic.cgi?id=11:44215:1650#1650)
от **half\_moon\_bay** Впаянный процессор, 16Gb.
Замер скоростей автором [NAS своими руками (часть 6), #1320](http://forum.ixbt.com/topic.cgi?id=11:44215:1320#1320).
Его коммент: "могу только добавить, что в этот конфиг отлично встаёт дешёвый четырёхпортовый контроллер ST-Lab 370
и в коробке таким образом можно вместить до 10 дисков 3.5". freenas 8.3
*   [NAS своими руками (часть 6), #2031](http://forum.ixbt.com/topic.cgi?id=11:44215:2031#2031)
от **shale** G530, 4Gb, 3 HDD, SSD под систему. Конфиг недорогой (кроме дисков).
*   [Конфигурация Mini-ITX для домашнего компьютера / сервера., #172](http://forum.ixbt.com/topic.cgi?id=4:99861:172#172)
от **Krey** сервер, а не чисто НАС [тут фотки](http://forum.ixbt.com/topic.cgi?id=4:99861:174#174)
*   [NAS своими руками (часть 6), #2043](http://forum.ixbt.com/topic.cgi?id=11:44215:2043#2043)
пара конфигураций от **axel77** - небольшая на атоме и развернутая на ксеоне.
*   [NAS своими руками (часть 6), #2124](http://forum.ixbt.com/topic.cgi?id=11:44215:2124#2124)
от **TPAKTOP**. Возможно, самая развернутая конфигурация в нашей ветке. Xeon, 18 дисков данных + системный. Фотографии.
*   [NAS своими руками (часть 6), #2277](http://forum.ixbt.com/topic.cgi?id=11:44215:2277#2277)
подробно изложенная конфигурация от **AvtoUser** с фото. Место для 12 HDD
*   [NAS своими руками (часть 6), #2436](http://forum.ixbt.com/topic.cgi?id=11:44215:2436#2436)
от **Brainstem** Solaris на Atom
*   [NAS своими руками (часть 6), #2432](http://forum.ixbt.com/topic.cgi?id=11:44215:2432#2432)
от **rsergio** Win, mITX, 2 диска данных стоят, до 6 всего влезает
*   [NAS своими руками (часть 6), #2633](http://forum.ixbt.com/topic.cgi?id=11:44215:2633#2633)
от **falstaff** Win на ssd, 6 HDD, Установлен FlexRAID, «снапшот рейд».
[Мнение автора о достоинствах и недостатках](http://forum.ixbt.com/topic.cgi?id=11:44215:2645#2645)
пару сообщений вниз - обсуждение.
*   [NAS своими руками (часть 6), #3423](http://forum.ixbt.com/topic.cgi?id=11:44215:3423#3423)
от **fatfree** Xeon E3-1230, 32Gb ECC RAM
*   [NAS своими руками (часть 6), #3677](http://forum.ixbt.com/topic.cgi?id=11:44215:3677#3677)
от **ewizard** i5-2500, аппаратный рейд 5 и 10, всего 12 HDD, Windows Home Server 2011
*   [http://lundman.net/wiki/index.php/ZFS_RAID](http://lundman.net/wiki/index.php/ZFS_RAID)
Небезызвестный lundman сделал себе 5-дисковый NAS под Solaris (всё на английском,
для квалифицированного читателя, с фотогаллереей)
*   [NAS своими руками (часть 6), #4785](http://forum.ixbt.com/topic.cgi?id=11:44215:4785#4785)
недорогой вариант с ECC памятью за счет использования процессора AMD
*   [NAS своими руками (часть 7), #1100](http://forum.ixbt.com/topic.cgi?id=11:44629-35#1100)
от **mkbth** miniITX с ECC памятью и Xeon
*   [NAS своими руками (часть 7), #1310](http://forum.ixbt.com/topic.cgi?id=11:44629-42#1310)
от **jenci** NAS на AMD с памятью ECC
*   [Географически распределённый вариант](http://forum.ixbt.com/topic.cgi?id=11:45199-126#3638)
от **Oleg Pyzhov**

## Выбор железа
### Процессор
*   Рабочая конфигурация [Pentium G2120 + ECC память](http://forum.ixbt.com/topic.cgi?id=11:44215:4668#4668) от **dim-soft**
*   [список процессоров и производительность в попугаях](http://www.cpubenchmark.net/cpu_list.php)
*   **Q.** Какой процессор посоветуете?<br />
    **A.** Зависит от задач. Обычно младший Sandy Bridge или Ivy Bridge, например Pentium G2120.
    Или что-то Atom-подобное.<br />
    **RU_Taurus**: приличный «холодный» Ivy Bridge будет и производительнее и энергоэффективнее
    какого-нибудь Атома или E-процессора AMD.

    **Q**. Стоит брать _T_ процессор, например i3-2100T? <br />
    **A.** Покупать Т-процы - бессмысленная трата денег.
    Посмотрите сравнение [i3-2100T и i3-2100](http://ark.intel.com/compare/53423,53422) <br />
    Отличий совсем немного:
    * Частота (2.5ГГц против 3.1ГГц) за счет разных множителей (25 против 31).
    * Частота графического чипа (650МГц против 850МГц).
    * TDP (35Вт против 65Вт).
    * Рекомендуемая цена ($132 против $120), реальная разница обычно больше.

    Как уж неоднократно тут говорилось - TDP это не потребление процессора, а нижняя граница рассеиваемой
    системой охлаждения мощности. При этом из i3-2100 всегда можно сделать i3-2100Т просто уменьшив
    множитель до 25 в BIOS. **AvtoUser**

    **Q.** Как оцениь энергопотребление процесора? По TDP?<br />
    **A.** TDP отношения к потребляемой мощности не имеет, это требование к системе охлаждения быть способной
    рассеивать не менее указанного кол-ва ватт тепловой энергии. Реальное энергопотребление некоторы
    современных процессоров можно посмотреть
    [здесь](http://www.fcenter.ru/online.shtml?articles/hardware/processors/31753#08).
    **RU_Taurus**

    **Q.** В каких процессорах AMD есть поддержка ECC памяти?<br />
    **A.** Cаппорт AMD про FX'ы: _"It takes some time to check the technical files.
    The result is: All the FX series, Phenom II, Athlon II (Socket AM3 or AM3+) support the unbuffered ECC memory.
    Best regards, AMD Global Customer Care."_ <br />
    Уточнение про Sempron (regor & sargas):
    _"Sorry I miss the Sempron, my falut.
    The Sempron is not included in Athlon II family but it also supports unbuffered ECC memory.
    Best regards, AMD Global Customer Care"_
    **scream_r**

### Материнская плата

**Q.** Какую LGA 1155 посоветуете?<br />
**A.** Зависит от потребностей. Обычно в нашей конференции рекомендуют mATX формфактор.
Ср. ASRock B75 Pro3-M и ASUS P8H77-M PRO.

**Q**. Насколько ценен аппаратный <abbr title="Redundant Array of Inexpensive Disks">RAID</abbr>,
рекламируемый на ряде материнских плат десктоп класса?<br />
**A**. Аппаратного <abbr title="Redundant Array of Inexpensive Disks">RAID</abbr> на этих устройствах
не бывает в принципе. Поэтому дома только два варианта - софтрейд или вообще без рейда,
просто отдельные диски.
Аппаратный <abbr title="Redundant Array of Inexpensive Disks">RAID</abbr>-контроллер с батарейкой?
Был бы, конечно, вариант, если бы не цена и ограниченная аппаратная совместимость с десктопным железом.
**RU_Taurus**

Ср также негативный [опыт](http://forum.ixbt.com/topic.cgi?id=11:45199-4#102) использования набортного
"RAID"от **WearWolf**

**Q**. А что же тогда там за <abbr title="Redundant Array of Inexpensive Disks">RAID</abbr>?  
**A**. Fake <abbr title="Redundant Array of Inexpensive Disks">RAID</abbr>.
Подробнее см англоязычную статью
[Differences between Hardware RAID, HBAs, and Software RAID](http://www.servethehome.com/difference-hardware-raid-hbas-software-raid/)

**Q**. Выбрал miniITX материнскую плату. Всё, что надо, есть, зачем её мне расширять?  
**A**. Рассмотрите и вариант mATX. Это вам сейчас кажется, что незачем. А потом захочется
поставить приличный HBA для увеличения SATA-портов, приличную сетевушку от Интел,
чтоб при 100МБайт/сек входящего по <abbr title="File Transfer Protocol">FTP</abbr>
поменьше процессор грузила и т.д. Зачем себя изначально загонять в какие-то рамки. **RU_Taurus**

### Корпуса

**RU_Taurus** о [Procase EB306S](http://forum.ixbt.com/topic.cgi?id=11:44629-94#2758)

**AlexIII** подробно описывает [Bitfenix Prodigy](http://forum.ixbt.com/topic.cgi?id=11:44629-110#3225),
[фотогалерея](http://imageshack.us/g/1/10035210/) [автора](http://forum.ixbt.com/topic.cgi?id=11:44629-94#2758)

### Блоки питания  

Если вам нужны ваши данные и/или железо, использование UPS необходимо.

Так как NAS работает в автоматическом режиме, без постоянного контроля со стороны человека,
необходимо и управляющее подключение NAS к UPS (обычно по USB).
Это позволит в случае проблем по питанию автоматически штатно выключить NAS.

Обратите внимание на [Проблемы совместной работы UPS и блоков питания с APFC](http://forum.ixbt.com/topic.cgi?id=49:7243).

[Обзоры блоков питания](http://www.fcenter.ru/online.shtml?articles/hardware/tower)

**Q.** Какой БП посоветуете?<br />
**A.** [Пример №1](http://forum.ixbt.com/topic.cgi?id=11:44215:4054#4054).
       [Пример №2](http://forum.ixbt.com/topic.cgi?id=11:44215:4060#4060).

[«Приглушение» корпусных вентиляторов](http://forum.ixbt.com/topic.cgi?id=11:44629-8#207)
в rackmount корпусах от **axel77**

[Аномальное поведение HDD при нехватке питания по 5В](http://forum.ixbt.com/topic.cgi?id=11:45199-15#405) опыт **archa**

### UPS

#### Реально работающие у форумчан

*   APC Back-UPS BX650CI-RS, nas4free 9.x/FreeBSD 9.x, nut, USB, работает из коробки, __saint_sergius__
*   APC Back-UPS CS 650, Ubuntu, nut, USB, usbhid-ups, зевелся без проблем, __bormental__
*   APC Back-UPS ES 700G, nas4free 9.x/FreeBSD 9.x, nut, USB, работает из коробки, __MikeMac__
*   [APC Back-UPS Pro 1200](http://www.apc.com/products/resource/include/techspec_index.cfm?base_sku=BR1200GI&total_watts=200),
FreeBSD 8.2-RELEASE/FreeBSD 9.0-RELEASE, apcupsd, USB/net, работает из коробки. __axel77__
[подробности](http://forum.ixbt.com/topic.cgi?id=11:44215:3668#3668)
*   APC Back-UPS RS1500i, FreeBSD 9.x, nut, USB, работает из коробки, __kostya_1983__
*   APC Smart-UPS 1500 (SUA1500I), nas4free 9.x/FreeBSD 9.x, nut, USB, usbhid-ups, работает из коробки, __Bedwere__
*   APC Smart-UPS 620 (SU620INET), nas4free 9.x/FreeBSD 9.x, nut, COM, apcsmart, работает из коробки, __ZanZag__
*   APC Smart-UPS SC420, nas4free 9.x/FreeBSD 9.x, nut, COM, apcsmart, работает из коробки, __ZanZag__
*   CyberPower CP1500EAVRLCD, 1500ВA, nut, __AvtoUser__
*   CyberPower Value 1200ELCD, nut, __cream_r__
*   Ippon Back Comfo Pro 400, nas4free 9.x/FreeBSD 9.x, nut, USB, работает из коробки, __mac_bear__
*   Ippon Back Power Pro 600, Nas4Free 9.x, nut, USB, blazer\_usb, работает из коробки, __SciNef__
*   MGE (Eaton) Ellipse 1000, Linux, nut, USB, usbhid-ups, работает, __bormental__
*   [Powercom Black Knight Pro BNT-1000AP](http://market.yandex.ru/model.xml?modelid=985692&hid=91082),
http://forum.pcm.ru/viewtopic.php?f=3&t=9169,
OMV 0.4.19, USB, NUT, usbhid-ups, работает из коробки, __hobot-bobot__
*   Powercom BNT600-AP и Powercom BNT1000-AP, Debian, nut, USB.
По поводу этих упсов: http://forum.pcm.ru/viewtopic.php?f=3&t=9169
__knyshow__

#### UPS, которые НЕ удалось заставить работать

*   Powerex VI 1000,Nas4Free, nut, USB
[определяется, и работает. Минут десять.](http://forum.ixbt.com/topic.cgi?id=11:44215:3710#3710),
После чего - _Error: Driver not connected_ __Linn__

#### UPS, вызывающие смешанные чувства

*   APC 525VA Back ES, nas4free 9.x/FreeBSD 9.x, nut, USB, не прижился у **gokvo,** <br />
[нормально работает](http://forum.ixbt.com/topic.cgi?id=11:46201-64#1942) у **CrashX** FreeNAS 9.2/9.3
*   Sven Power Smart 1000 от __RU_Taurus__ [тут](http://forum.ixbt.com/topic.cgi?id=11:44215:3666#3666)
и следующее сообщение

#### Отключение UPS после отключения нагрузки  

*   Решение для [NAS4FREE, MGE Ellipse ASR 600 USBS](http://forum.ixbt.com/topic.cgi?id=11:45837-143#4212),
(вероятно подобным образом и для других UPS) **GrayWolf**

### Жесткие диски

#### Гугловское исследование

[Failure Trends in a Large Disk Drive Population](http://static.googleusercontent.com/external_content/untrusted_dlcp/research.google.com/en/us/archive/disk_failures.pdf)
fig 4 свидетельствует о том, что оптимальная для длительной работы жесткого диска температура - где-то 36-45С.
При температуре 25С вероятность выхода из строя удваивается, при 20С - возрастает в 5 раз.
Критики отмечают, что материал опубликован в 2007 г и с тех пор конструкции дисков изменились.
Решайте сами - доверять или нет.

#### "Зеленые" WD

- с трудом переваривают глубину очереди запросов в 10 единиц и которую поэтому нужно уменьшать до 5-6.
 **RU_Taurus** [подробнее](http://forum.ixbt.com/topic.cgi?id=11:44215:4819#4819)
- при использовании под \*nix настоятельно рекомендуется отключить парковку головок или выставить
длительный интервал **MikeMac** [подробнее](http://2gusia.livejournal.com/27695.html)

#### Значение параметров S.M.A.R.T.  

[Оцениваем состояние жёстких дисков при помощи S.M.A.R.T.](http://www.ixbt.com/storage/hdd-smart-testing.shtml) -
статья на ixbt.com

#### Аномальное поведение HDD

[Аномальное поведение HDD при нехватке питания по 5В](http://forum.ixbt.com/topic.cgi?id=11:45199-15#405) опыт **archa**  

#### Cкрипт проверки SMART c отчетом на почту

[Скрипт проверки дисков на Reallocated c отправкой отчета на почту]
(http://forum.ixbt.com/topic.cgi?id=11:46201:1835#1835) от **Oleg Pyzhov**

### SATA и SAS контроллеры

**Q.** посоветуйте контроллер на n портов <br />
**A.** Профильная тема [SATA/SAS/RAID-контроллеры для дома и офиса.](http://forum.ixbt.com/topic.cgi?id=11:43801)
См. также  [From 32 to 2 ports: Ideal SATA/SAS Controllers for ZFS & Linux MD RAID](http://blog.zorinaq.com/?e=10)
Наиболее популярен в нашей ветке Dell H200A, [IBM m1015](http://www.servethehome.com/ibm-m1015-part-1-started-lsi-92208i/),
причём [перешитый в IT.](http://forum.ixbt.com/topic.cgi?id=11:43801:1425#1425) <br />
Ср. также [достался мне Dell Perc H310](http://forum.ixbt.com/topic.cgi?id=11:46201-166#4860)
от **sagem830**

**Q**. Хочу добавить SATA портов, использовав SATA мультипликатор (SATA Port Multiplier).
Скорость упадёт? <br />
**A.** на SATAII мультипликаторе портов 3Gb/s делится на всех. На 5 дисках каждому достанется 600 мегабит/c
(грубо 60 мбайт/с с учётом накладных расходов). Что в полтора, а то и два раза хуже ,
чем могут дать современные недорогие диски.
А SATA мультипликаторов на SATAIII (aka 6Gb/s) пока в природе не обнаружено (_устарело?_). **MikeMac**

**Q**. Нужен относительно простой SATA-контроллер (PCI-e x4 и без RAID) на 8 дисков<br />
**A.** Я так понимаю, речь всеж идет о PCI-E 2.0? Если да, то:

1. LSI SAS HBA 9211-8i
2. Под OEM-вариантом LSI SAS HBA 9210-8i выпускаются след. брендированные контроллеры:
    * IBM M1015
    * Intel RS2WC080
    * DELL PERC H200
    * Fujitsu D2607-A21
Все они с разной степенью успешности перешиваются в любой из вариантов LSI - HBA (IT/IR) или RAID.
3. HighPoint Rocket 2720SGL.
**RU_Taurus**

### Видеокарта и её удаление

**Q.** nas4free 10.2. Мать Asus P7P55D без встроенного видео - как запуститься без видеокарты?
Устанавливал систему с дискретной. Думал что после установки выдерну карту, включу комп
и все завертится, ан нет. Мамка мигает лампочками по мере загрузки: память, видео, загрузочное
устройство (лампочка у SATA портов), затем зажигается огонек на флешке с которой идет загрузка.
После выдергивания видяхи происходит следующее: мигает память, мигает лампочка рядом с видео-слотом,
далее звуковой сигнал об отсутствии карты, снова мигает память, далее мигает загрузочная лампочка и
начинает мигать лампочка на флешке! Однако, после 5-10 минут ожидания интерфейс недоступен, сервер
не виден в сети.<br />
**A.** У вас ведь новый NAS4Free, который уже на 10-ой версии FreeBSD? Попробуйте в loader.conf прописать строки:

```sh
kern.vty=vt  
hw.vga.textmode=1  
```
**RU_Taurus**

Результат положительный.  

### Сеть
**Q.** Думаю посадить NAS на беспроводное соединение.<br />
**A.** Подключение по WiFi не рекомендуется,
см. [NAS своими руками (часть 6), #4076](http://forum.ixbt.com/topic.cgi?id=11:44215:4076#4076)
и обсуждение ниже.

Рекомендации **padavan** по настройкам WiFi для просмотра HD видео на медиаплеере см.
[Dune HD Base 1.0/2.0/3.0 и Dune BD Prime 1.0/3.0 Обсуждаем и делимся опытом (часть 3), #1618]
(http://forum.ixbt.com/topic.cgi?id=60:8:1618#1618)
Касается не только Дюны.
__NB__ это всё может работать, если на этом канале идёт отдача видео и всё.
Если там же планшеты-смартфоны - канал делится на всех.

**Q.** Хочу использовать NAS в роли роутера, раздавать интернет. А то роутер позволяет только 100 мбит,
хотелось бы гигабит иметь, По сути только сетевую карту докупить и настроить.<br />
**A.** Подключаете к роутеру гигабитный свитч и все устройства включаете в него - получаете гигабитную локалку.
Или у вас канал до провайдера больше 100Мбит/с? **AvtoUser**

### Колхоз

[Размещение 2.5 HDD в PCI слот](http://kom.aau.dk/%7Epmr/StumbleUpon/HD-on-PCI/)

[SATA backplane for Fractal Design Define R3](http://kom.aau.dk/%7Epmr/StumbleUpon/SATA-backplane/)

[Корпус на 14 дисков](http://forum.ixbt.com/topic.cgi?id=11:45199-167#4820) от **lepon**, фото

[Одержание кулера и всё-всё](http://forum.ixbt.com/topic.cgi?id=11:45837-51#1519) от **markus912**, фото  

[  
](http://kom.aau.dk/%7Epmr/StumbleUpon/SATA-backplane/)

### Платформы помимо x32/x64  

[Установка FreeBSD на Netgear Stora с поддержкой ZFS](http://forum.netgear.ru/viewtopic.php?id=7170) от **Oddentity**

[Openmediavault 0.6 kralizec on Netgear Stora]
(http://chrislamothe.blogspot.ru/2014/08/openmediavault-06-kralizec-on-netgear.html) от **Chris LaMothe**

[SATA backplane for Fractal Design Define R3](http://kom.aau.dk/%7Epmr/StumbleUpon/SATA-backplane/)
