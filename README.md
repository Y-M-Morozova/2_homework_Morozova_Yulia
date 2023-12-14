# Морозова Юлия, OTUS, группа Postgre-DBA-2023-11

## Домашнее задание №2 по теме: «Установка PostgreSQL»

<br/><br/>

1. Создаю в яндекс облаке ВМ с Ubuntu /22.04 и устанавливаю докер:
    ![1](https://github.com/Y-M-Morozova/2_homework_Morozova_Yulia/assets/153178571/e3fdc6b3-6bf9-468e-acfa-3b6a4e7728ef)

<br/><br/>

2.	Создаю docker-сеть pg-net:
    ![2](https://github.com/Y-M-Morozova/2_homework_Morozova_Yulia/assets/153178571/0b15e7ca-08d3-44c3-962d-5637c1de0fc5)

<br/><br/>


3.	Подключаю созданную сеть pg-net к контейнеру(pg-server) сервера Postgres, версия 15, порт хоста 5432, порт контейнера 5432, монтирую ЛОКАЛЬНУЮ папку для хранения данных: /var/lib/postgresql/data:

    ![3](https://github.com/Y-M-Morozova/2_homework_Morozova_Yulia/assets/153178571/18c1028a-dc40-4e27-a918-f0046f21f813)

<br/><br/>

4.	Запускаю отдельный контейнер с клиентом(pg-client) Postgres в общей сети c БД, создаю для тестов БД otus, а в ней тестовую табличку test, вставляю 2 строки:

    ![4](https://github.com/Y-M-Morozova/2_homework_Morozova_Yulia/assets/153178571/63b89f4b-fb18-4458-87cf-59501afbaec2)


<br/><br/>

5.	Проверяю наш отдельный контейнер:

   ![5](https://github.com/Y-M-Morozova/2_homework_Morozova_Yulia/assets/153178571/1a2428ba-864e-4152-8068-99c48236a39a)

   <br/><br/>

   

