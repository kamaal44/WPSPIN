# WPSPIN.sh
27 октября 2014 года, человеком под ником hacker404 был опубликован скрипт, позволяющий проводить тестирование WIFI роутеров с включенным WPS. Скрипт включал в себя встроенный генератор и базу дефолтных WPS-Pin для некоторых моделей беспроводных роутеров.
Скрипт прекрасно работал и показывал хорошие результаты до выхода релиза Kali Linux 2.
С выходом нового релиза Kali, скрипт перестал работать, т.к. изменился формат вывода обновленного airmon-ng...

Пришло время вдохнуть новую жизнь в скрипт ;-)

Внес изменения в код для корректной работы на Kali Linux 2. Добавил автоматический перевод беспроводного адаптера из режима Monitor в режим Managed и запуск службы network-manager при нажатии EXIT, Restart и перерыванием работы Reaver по нажатии CTRL+C.
Теперь нет необходимости вручную менять режим адаптера после завершения работы скрипта. 
Весь остальной функционал остался без изменения.

WPSPIN.sh for KaliLinux 2
