Татаринова Екатерина, группа АДЭУ-221

Вариант 15
-----------------------------------------------------------------------------------------

Лабораторная работа 1.1 Установка и настройка ETL-инструмента. Создание конвейеров данных


Бизнес-задача: Выявить сегменты клиентов с высоким риском оттока (Churn=Yes), чтобы разработать меры удержания

Запуск Пентахо

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab_1/img/1%20etl.png)
  
Загрузка данных
 
![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab_1/img/2%20etl.png)
  
![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab_1/img/3%20etl.png)

Загрузка файла  (Csv file input)

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab_1/img/4%20etl.png)

Проводим проверку названий (select values) столбцов для базы данных (snake-case):

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab_1/img/5%20etl.png)

Проводим отбор столбцов (Memory group by):

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab_1/img/6%20etl.png)

Заполнение полей Value mapper

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab_1/img/7%20etl.png)

Вкладка Table order

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab_1/img/8%20etl.png)

Результат

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab_1/img/9%20etl.png)

Результат в phpMyAdmin

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab_1/img/res.png)



