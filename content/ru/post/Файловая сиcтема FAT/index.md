---
title: Файловая Система FAT
subtitle: Сегодня мы поговорим о файловой системе FAT
# Link this post with a project
projects: []

# Date published
date: '2022-05-25T00:00:00Z'

# Date updated
lastmod: '2022-05-25T00:00:00Z'

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'Image credit: []()'
  focal_point: ''
  placement: 2
  preview_only: false

authors:
  - admin

tags:
  - 5 неделя

categories:
  - пост 5

---
Файловая система – это инструмент, позволяющий операционной системе и программам обращаться к нужным файлам и работать с ними. При этом программы оперируют только названием файла, его размером и датой созданий. Все остальные функции по поиску необходимого файла в хранилище и работе с ним берет на себя файловая система накопителя



## **Что за файловая система?**

Сокращенная аббревиатура «FAT» расшифровывается как «таблица размещения файлов». Это простая классическая архитектура файловой системы, изначально предназначенная для небольших дисков и простых структур папок. Инымисловами, файловая система «FAT» представляет собой групповой метод организации, в котором таблица размещения файлов выделена в отдельную логическую область и находится в начале тома. Для исключения непреднамеренных или случайных ошибок, способных повлиять на корректное отображение таблицы, система, в целях безопасности, хранит копию массива индексных указателей. Файловая система FAT используется ОС MS DOS и ОС Windows для упорядочения файлов и управления ими.

Разработана Биллом Гейтсом и Марком МакДональдом (англ.) в 1976—1977 годах. Использовалась в качестве основной файловой системы в операционных системах семейств MS-DOS и Windows 9x.


## **Какие бывают файловые системы FAT?**
Существует несколько версий файловой системы FAT, среди которых наибольшее применение нашли файловые системы FAT 16 и FAT 32. Отличие этих файловых систем состоит в разрядности чисел, используемых в таблицах размещения файлов.

Однако упоминаю еще две файловые системы :FAT12 и FAT64 или другое ее название exFAT. Дальше мы разберем их различия.

## **Файловая Система FAT12**

Файловая система, широко применяемая на гибких магнитных дисках. Является первой популярной файловой системой на IBM PC - совместимых компьютерах.

Самое последнее устройство накопления информации, которое использовало файловую систему FAT12 были гибкий диск диаметром 3.5 дюйма и емкостью 1,44 МБ. Были еще дискеты размером 2,88, но они не получили большого распространения.

Все пространство файловой системы FAT12 разделено на блоки, кратные размеру сектора дискеты (512 байт). В применении к дискетами размер кластера обычно выбирается равным одному сектору. Каждый непустой файл занимает минимум 1 кластер. Поэтому если на дискете будет много маленьких файлов, то много места будет пропадать зря. Максимальный размер кластера для файловой системы FAT12 составляет 8192 байта.

Достоинствами ее является то, что она занимает мало места на диске, требует мало оперативной памяти для ее кэширования. Недостатком - то, что при использовании на разделах больше 64 Mб размер кластера становится максимальным, что приводит к неизбежным потерям свободного места на диске в конечном кластере каждого файла.

## **Файловая Система FAT16**

Файловая система FAT 16 поддерживается ОС MS DOS, Windows 95, Windows 98, Windows 2000, а также некоторыми версиями ОС UNIX.Цифра 16 в названии файловой системы указывает на число бит (двоичных разрядов), необходимых
для хранения информации о номерах кластеров, используемых файлом, т. е. в таблице размещения файлов можно разместить не более 65536 записей Операционная система использует Таблицу размещения файлов для поиска файла и определения кластеров, которые этот файл занимает на жестком диске. Кроме того, в Таблице фиксируются сведения о свободных и дефектных кластерах. Чтобы легче было осмыслить файловую систему FAT16 представьте
себе оглавление книги и как вы работаете с этим оглавлением, вот именно также операционная система работает с FAT 16.

Максимальный размер разделов или дисков в FAT16 составляет 4,2 гигабайта.

Однако в наше время FAT 16 использование неэффективно. Но она полностью удовлетворяла требованиям старых компьютеров.

Современные НЖМД имеют объем памяти несколько десятков гигабайт, поэтому применение файловой системы FAT16 для них неэффективно.

Второй недостаток заключается в том, что для хранения всех файловых атрибутов система FAT использует всего 1 байт. Поэтому просто не представляется возможности хранить данные о правах доступа к файлу, его владельце и т. д.

## **Файловая Система FAT32**

Файловая система FAT32 является расширенной версией файловой системы FAT16, поддержка которой была впервые реализована в Windows 95В . Файловая система FAT32 поддерживается также ОС Windows 98, Windows 2000 и Windows ХР.

Основное отличие файловой системы FAT32 от FAT16 заключается в том, что в таблице размещения файлов FAT можно разместить не 65 536 записей о номерах кластерах, а 268.435.445.

Одна из основных причин создания FAT32 состояла в необходимости более эффективно использовать дисковое пространство. В этой файловой системе используются кластеры меньшего размера для накопителей, емкость которых не превышает 8 Гбайт (размер кластеров при этом составляет 4 Кбайт), что позволяет на 10–15 % повысить эффективность использования дискового пространства накопителя по сравнению с накопителем в файловой системе FAT16. Кроме того, в файловой системе FAT32 увеличивается максимальный размер тома (раздела) диска.

## **Файловая Система FAT64 или exFAT**

«exFAT» – это сокращенное обозначение от полного английского названия «Extended File Allocation Table» («расширенная таблица размещения файлов»). Стандарт является обновленной версией файловой системы «FAT32»,созданный корпорацией «Microsoft».Система exFAT чрезвычайно похожа на FAT32. Но главным отличием является устранение ограничений, присутствующих в файловой системе FAT32, что позволяет пользователям хранить файлы намного большего размера, чем четыре гигабайта.

Также в файловой системе «exFAT» значительно снижено число перезаписей секторов, ответственных за непосредственное хранение информации, что особенно важно для флэш-накопителей, ввиду необратимого изнашивания ячеек после определённого количества операций записи, и улучшен механизм распределения свободного места.

## **Достоинства и Недостатки файловой системы FAT**

Конечно, файловая система FAT уже устарела и используется все больше в флэшкартах, чем в операционных системах. Однако также у нее остался и плюсы:
-  Файловая система FAT лучше всего работает для дисков и/или разделов примерно в 200 МБ, так как FAT начинается с очень мало накладных расходов.
-  Поддерживается большинством устройств.

Но также существуют и минусы FAT:
-  Желательно, чтобы при использовании дисков или разделов более 200 МБ файловая система FAT не должна использоваться. Это потому, что по мере увеличения размера тома производительность с FAT быстро снижается.
-  Низкая устойчивость с мягким сбоям;
-  "Потерянные кластеры“
-  Отсутствуют механизмы разграничения доступа
-  Невозможно установить разрешения на файлы, которые являются разделамиFAT.
















