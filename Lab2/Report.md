University: [ITMO University](https://itmo.ru/ru/)
Faculty: [FICT](https://fict.itmo.ru)
Course: [Introduction to distributed technologies](https://github.com/itmo-ict-faculty/introduction-to-distributed-technologies)
Year: 2022/2023
Group: K4112c
Author: Бученков Евгений Евгеньевич
Lab: Lab2
Date of create: 20.09.2022
Date of finished: 13.11.2022

Создание service манифесты и разворачиваем deployment, для хостинга сервисов:
![Image text](https://github.com/eugenebuch/2022_2023-introduction_to_distributed_technologies-k4112c-buchenkov_e_e/blob/master/Lab2/2022-11-13_22-11.png)

После выполнения прошлой лабораторной необходимо было перезапустить системный сервис net, после чего запускаем созданные сервисы и видим следующую страницу:
![Image text](https://github.com/eugenebuch/2022_2023-introduction_to_distributed_technologies-k4112c-buchenkov_e_e/blob/master/Lab2/2022-11-13_22-19.png)

Диграмма сервисов, отражающая взаимодействие контейнеров (port-forward является переадресацией сервисного порта 8200 на стандартный реакт-порт 3000, который доступен снаружи):

![Image text](https://github.com/eugenebuch/2022_2023-introduction_to_distributed_technologies-k4112c-buchenkov_e_e/blob/master/Lab2/DiagramLab2.png)

Вывод:
В результате проделанной работы был запущен сервис с клиентской частью на порту 3000, в который были переданны значения переменных окружения
