# Морозова Юлия, OTUS, группа Postgre-DBA-2023-11

## Домашнее задание №2 по теме: «Установка PostgreSQL»

<br/><br/>

1. Создаю в яндекс облаке ВМ с Ubuntu /22.04 и устанавливаю докер:

    ![1](https://github.com/Y-M-Morozova/2_homework_Morozova_Yulia/assets/153178571/b9216a02-aede-4882-baf0-dfbbcc8838d3)
 

<br/><br/>

2.	Создаю docker-сеть pg-net:

    ![2](https://github.com/Y-M-Morozova/2_homework_Morozova_Yulia/assets/153178571/c45b2e71-11f7-463c-92c8-c36391c1ab5d)


<br/><br/>


3.	Подключаю созданную сеть pg-net к контейнеру(pg-server) сервера Postgres, версия 15, порт хоста 5432, порт контейнера 5432, монтирую ЛОКАЛЬНУЮ папку для хранения данных: /var/lib/postgresql/data:

    ![3](https://github.com/Y-M-Morozova/2_homework_Morozova_Yulia/assets/153178571/a8699bfe-809f-4c87-ad00-16245ce1bdfd)

<br/><br/>

4.	Запускаю отдельный контейнер с клиентом(pg-client) Postgres в общей сети c БД:

    ![4_5](https://github.com/Y-M-Morozova/2_homework_Morozova_Yulia/assets/153178571/99435e84-2bc7-4a23-9849-32fb8de69729)
      
<br/><br/>

5.	Cоздаю для тестов БД otus, а в ней тестовую табличку test, вставляю 2 строки:

    ![5](https://github.com/Y-M-Morozova/2_homework_Morozova_Yulia/assets/153178571/1a2428ba-864e-4152-8068-99c48236a39a)

   <br/><br/>

   
6.	Теперь подключаюсь к контейнеру с сервером с домашнего ноутбука(НЕ из яндекс облака!) , для этого беру публичный адрес моей ВМ в ЯО и настройки контейнера, для подключения пользуюсь DBeaver’ом (установлен локально - на моем ноутбуке). Проверяю: БД otus, таблица test и две строки – все ок!

    ![6](https://github.com/Y-M-Morozova/2_homework_Morozova_Yulia/assets/153178571/8e1a1480-b430-45ee-9421-612fa8c16991)

<br/><br/>
