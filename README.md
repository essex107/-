
 Лабораторная работа №1

Здесь приведены задачи по взаимодействию с таблицей orders.

Получение всех заказов: Нужно получить все данные из таблицы orders.

![VirtualBox_kiryanova21212121212112121212121212112_27_02_2025_23_08_09](https://github.com/user-attachments/assets/6d928aca-629c-4ccd-86d5-aa53168a7a33)

Исключение новых заказов: Нужно выбрать все заказы, за исключением тех, у которых статус "new". Используется оператор IN.
https://github.com/essex107/-/blob/main/VirtualBox_kiryanova21212121212112121212121212112_27_02_2025_23_09_54.png?raw=true

Выбор новых и отмененных заказов: Необходимо получить список заказов со статусом "new" или "cancelled".

![VirtualBox_kiryanova21212121212112121212121212112_27_02_2025_23_10_00](https://github.com/user-attachments/assets/6d3c79ee-e1ee-4e60-8533-0618946f5674)



Заказы с большим количеством товаров: Выбираются заказы, где количество товаров (products_count) больше 3. Выводятся только идентификатор заказа (id) и общая стоимость (sum).
![VirtualBox_kiryanova21212121212112121212121212112_27_02_2025_23_10_09](https://github.com/user-attachments/assets/3a04615d-ea9d-4ad7-8a08-c0014b86cfa7)

Лабораторная работа №2

Задачи по работе с таблицами orders и products.

Три самых дешевых заказа: Необходимо найти три заказа с самой низкой стоимостью. Результаты сортируются по убыванию цены. Отмененные заказы не учитываются.

![VirtualBox_kiryanova21212121212112121212121212112_27_02_2025_23_16_02](https://github.com/user-attachments/assets/8aba39a0-6240-4997-baa5-d8664f5554e2)

Два самых дорогих заказа: Нужно получить два заказа с максимальной стоимостью. Данные сортируются по убыванию цены, отмененные заказы исключаются.
![VirtualBox_kiryanova21212121212112121212121212112_27_02_2025_23_16_06](https://github.com/user-attachments/assets/f693bc76-9930-4f17-94d9-21ac11efb4c9)


Добавление нового заказа: В таблицу orders добавляется информация о новом заказе на сумму 8000 рублей, состоящем из 4 товаров (products).
![VirtualBox_kiryanova21212121212112121212121212112_27_02_2025_23_37_16](https://github.com/user-attachments/assets/f6cf47ca-0586-4cdd-b511-435ad35d7d54)


Добавление нового товара: В таблицу products вносятся данные о новом товаре: "VR-очки" стоимостью 70000 рублей, в количестве 2 штук (count).

![VirtualBox_kiryanova21212121212112121212121212112_27_02_2025_23_44_17](https://github.com/user-attachments/assets/1aacd50f-83c6-4c19-9975-ef5c8932e28c)


Исправление ошибки в названии товара: В таблице products название товара "IMAC" исправляется на "PS5".

![VirtualBox_kiryanova21212121212112121212121212112_27_02_2025_23_49_36](https://github.com/user-attachments/assets/4a05294a-9bed-4d2e-82f3-3085d7ca997e)

Лабораторная работа №3
Создание таблицы users:
![VirtualBox_Kiryanovafffffffffffffff_01_03_2025_10_43_40](https://github.com/user-attachments/assets/5b49dd32-f7eb-4b12-ac63-53a8990ab5d7)

![VirtualBox_Kiryanovafffffffffffffff_01_03_2025_10_16_04](https://github.com/user-attachments/assets/d968877f-08e4-4995-b98f-980537b521d9)

Полезные команды (шпаргалки)
*   **Однострочный INSERT:** `INSERT INTO table (column1, column2) VALUES (value1, value2);` (Вставка одной записи в таблицу).
*   **Многострочный INSERT:** `INSERT INTO table (column1, column2) VALUES (value11, value12), (value21, value22), ...` (Вставка нескольких записей в таблицу одним запросом).
*   **INSERT ... SELECT:** `INSERT INTO table1 (column1, column2) SELECT (col1, col2) FROM table2;` (Вставка данных, полученных из другой таблицы с помощью запроса SELECT).
*   **Глобальное обновление (UPDATE):** `UPDATE table1 SET column1 = new value;` (Обновление значения указанного столбца для всех записей в таблице).
*   **Условное обновление (UPDATE ... WHERE):** `UPDATE table1 SET column1=new_value, column2=new_value WHERE condition;` (Обновление значений указанных столбцов для записей, удовлетворяющих заданному условию).
*   **Полное удаление (DELETE):** `DELETE FROM table;` (Удаление всех записей из таблицы).
*   **Условное удаление (DELETE ... WHERE):** `DELETE FROM table WHERE condition;` (Удаление записей из таблицы, удовлетворяющих заданному условию).

