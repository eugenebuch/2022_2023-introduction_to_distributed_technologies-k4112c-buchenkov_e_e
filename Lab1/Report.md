University: [ITMO University](https://itmo.ru/ru/)
Faculty: [FICT](https://fict.itmo.ru)
Course: [Introduction to distributed technologies](https://github.com/itmo-ict-faculty/introduction-to-distributed-technologies)
Year: 2022/2023
Group: K4112c
Author: Бученков Евгений Евгеньевич
Lab: Lab1
Date of create: 20.09.2022
Date of finished: 13.11.2022

Ответы на вопросы:

1. Что сейчас произошло и что сделали команды указанные ранее? 
minikube kubectl -- expose pod vault --type=NodePort --port=8200: создает сервис типа NodePort (доступного клиентам из вне) с портом 8200

kubectl port-forward service/vault 8200:8200: перевод контейнера на порт 8200
![Image text](https://github.com/eugenebuch/2022_2023-introduction_to_distributed_technologies-k4112c-buchenkov_e_e/blob/master/Lab1/2022-11-13_18-27.png)

После этого хостится веб-морда
![Image text](https://github.com/eugenebuch/2022_2023-introduction_to_distributed_technologies-k4112c-buchenkov_e_e/blob/master/Lab1/2022-11-13_18-27_1.png)

minikube stop: останавливает выполнение minikube

2. Где взять токен для входа в Vault?
Токен можно взять, если посмотреть в логи контейнера десктоп версии докера, либо если ввести команду "kubectl logs vault"

![Image text](https://github.com/eugenebuch/2022_2023-introduction_to_distributed_technologies-k4112c-buchenkov_e_e/blob/master/Lab1/2022-11-13_18-29.png)

При вводе валидного токена видим хранилище секретов
![Image text](https://github.com/eugenebuch/2022_2023-introduction_to_distributed_technologies-k4112c-buchenkov_e_e/blob/master/Lab1/2022-11-13_18-29_1.png)
