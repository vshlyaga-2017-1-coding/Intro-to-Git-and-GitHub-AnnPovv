# Введение в систему контроля версий Git и систему для совместной разработки GitHub

**На проработку материала и выполнение заданий у вас есть 2 недели.**

## О контроле версий

Что такое контроль версий, и зачем он вам нужен? Система контроля версий — это система, регистрирующая изменения в одном или нескольких файлах с тем, чтобы в дальнейшем была возможность вернуться к определённым старым версиям этих файлов. Чаще всего в системах контроля версий хранятся исходные коды программ, но на самом деле под версионный контроль можно поместить файлы практически любого типа.

Система контроля версий даёт возможность возвращать отдельные файлы к прежнему виду, возвращать к прежнему состоянию весь проект, просматривать происходящие со временем изменения, определять, кто последним вносил изменения во внезапно переставший работать модуль, кто и когда внёс в код какую-то ошибку, и многое другое. Вообще, если, пользуясь системой контроля версий, вы всё испортите или потеряете файлы, всё можно будет легко восстановить. Вдобавок, накладные расходы за всё, что вы получаете, будут очень маленькими.

## Git

Git (произносится «гит») — распределённая система контроля версий. Проект был создан Линусом Торвальдсом для управления разработкой ядра Linux, первая версия выпущена 7 апреля 2005 года. Основные требования к новой системе были следующими:

* Скорость
* Простота дизайна
* Поддержка нелинейной разработки (тысячи параллельных веток)
* Полная распределённость
* Возможность эффективной работы с такими большими проектами, как ядро Linux (как по скорости, так и по размеру данных)

С момента рождения Git развивался и эволюционировал, становясь проще и удобнее в использовании, сохраняя при этом свои первоначальные качества. Он невероятно быстр, очень эффективен для больших проектов, а также обладает превосходной системой ветвления для нелинейной разработки

## GitHub

GitHub (произносится «гитхаб») — крупнейший веб-сервис для хостинга IT-проектов и их совместной разработки. Основан на системе контроля версий Git и разработан на Ruby on Rails и Erlang. Сервис абсолютно бесплатен для проектов с открытым исходным кодом и предоставляет им все возможности (включая SSL), а для частных проектов предлагаются различные платные тарифные планы.

Создатели сайта называют GitHub «социальной сетью для разработчиков». Кроме размещения кода, участники могут общаться, комментировать правки друг друга, а также следить за новостями знакомых. С помощью широких возможностей Git программисты могут объединять свои репозитории — GitHub предлагает удобный интерфейс для этого и может отображать вклад каждого участника в виде дерева.

Первый частный репозиторий был создан 12 января 2008. К концу 2011 года в проекте уже было зарегистрировано более миллиона пользователей и более двух миллионов репозиториев. По состоянию на март 2017 года на сайте существовало более 58 миллионов репозиториев.

## Интересные факты про Git и GitHub

*Этот раздел будет дополняться студентами в процессе выполнения заданий*

* Автор Git, Линус Торвальдс, со своей командой при работе над ядром Linux бесплатно использовали коммерческую распределённую систему контроля версий BitKeeper. В 2005 году отношения между сообществом разработчиков ядра и компанией, разрабатывавшей BitKeeper, испортились, и право бесплатного пользования продуктом было отменено. Это и подтолкнуло разработчиков Linux разработать собственную систему, основываясь на опыте, полученном за время использования BitKeeper. Так и появился на свет Git.

## Задания для самостоятельной работы

1. Установить Git на компьютер, используя помощь из разделов 1.4 и 1.5 книги «Pro Git» (https://git-scm.com/book/ru/v1)
2. Прочитать раздел 2 книги «Pro Git» (https://git-scm.com/book/ru/v1)
3. Выполнить задания интерактивного урока «Try Git» (https://try.github.io)
4. Добавить в этот репозиторий новый файл, в котором разместить исходный текст программы на выбранном вами языке программирования, которая выводит на экран надпись `Hello, World!`.
5. Создать дополнительную ветку `refactoring`, в которой надпись заменена на текущую дату.
6. В основной ветке `master` заменить надпись `Hello, World!` на надпись `Hello, User!`.
7. Выполнить слияние ветки `refactoring` в ветку `master`. При слиянии заменить вывод на строчку `Hello, User! Today is {ТЕКУЩАЯ ДАТА}`.
8. Удалить ветку `refactoring`.
9. Добавить в репозиторий задачу (Issue), в которой указать необходимость добавить в программу комментарий о появлении вывода текущей даты.
10. Посмотреть через терминал историю изменений файла. Определить SHA-1 хеш коммита, в котором в программу в дополнительной ветке был добавлен вывод текущей даты.
11. Найти в справочном сайте GitHub (https://help.github.com) форматы инструкций, которая будучи добавлена в описание коммита позволяет управлять состоянием задач.
12. Добавить в программу комментарий с 7-значной версией хеша соответствующего коммита. При добавлении коммита с комментарием в репозиторий, добавить в описание коммита специальную инструкцию, которая позволит автоматически пометить созданную ранее задачу как выполненную.
13. В случае ошибки выполнить шаги 9–12 заново. Успешным выполнением считается задача, которая была создана вручную, а закрыта с помощью специальным образом оформленного описания коммита.
14. Найти интересный для себя факт о системе контроля версий Git или сервисе GitHub и добавить его в репозиторий  https://github.com/storkvist/Intro-to-Git-and-GitHub в раздел «Интересные факты о Git и GitHub» с помощью пулл-реквеста.

## Источники информации

1. Электронная книга «Pro Git» (по-русски) — https://git-scm.com/book/ru/v1
2. Справочный сайт сервиса GitHub (по-английски) — https://help.github.com
