# Отчет по лабораторной работе №2.2
 
**Студент:** Татаринова Екатерина 
**Группа:** АДЭУ-221
**Вариант:** 15  
**Тема данных:** Real Estate (Недвижимость) — адаптировано на E-commerce (Superstore)  
**Основной фильтр:** Подкатегория "Art"  
**Доп. задание 1:** Отчет по городам  

---

## Цель работы

Получить практические навыки создания сложного ETL-процесса, включающего динамическую загрузку файлов по HTTP, нормализацию базы данных, обработку дубликатов и настройку обработки ошибок с использованием Pentaho Data Integration (PDI).

---

## Ход выполнения работы

### 1. Подготовка базы данных

Выполнен SQL-скрипт для создания таблиц:
- `orders` — таблица фактов (заказы)
- `customers` — измерение "Клиенты"
- `products` — измерение "Товары"

Настроена кодировка `utf8mb4`.

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab2/img/1_create%20table.png)

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab2/img/2_createTable.png)

### 2. Создание главного Job (CSV_to_MySQL.kjb)

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab2/img/3_job.png)

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab2/img/4Job.png)

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab2/img/5_1_job.png)




### 3. Трансформация Orders 

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab2/img/9_filterArt.png)

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab2/img/9.1_valueInOrder.png)

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab2/img/10_tableorder.png)

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab2/img/6_conection.png)


### 4. Дополнительное задание 1: Отчет по городам (city_report.ktr)

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab2/img/14_cityRep.png)

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab2/img/15_cityrep.png)

**Результат:** CSV-файл `city_report.csv` с количеством клиентов по городам.

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab2/img/16_cityrep_res.png)

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab2/img/17_cityrep_resres.png)




## Результаты работы

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab2/img/11_res.png)

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab2/img/12_res.png)

![](https://github.com/TatarinovaEM758/PP_ETL/blob/main/lab2/img/13_res.png)
