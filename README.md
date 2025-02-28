*   **Однострочный INSERT:** `INSERT INTO table (column1, column2) VALUES (value1, value2);` (Вставка одной записи в таблицу).
*   **Многострочный INSERT:** `INSERT INTO table (column1, column2) VALUES (value11, value12), (value21, value22), ...` (Вставка нескольких записей в таблицу одним запросом).
*   **INSERT ... SELECT:** `INSERT INTO table1 (column1, column2) SELECT (col1, col2) FROM table2;` (Вставка данных, полученных из другой таблицы с помощью запроса SELECT).
*   **Глобальное обновление (UPDATE):** `UPDATE table1 SET column1 = new value;` (Обновление значения указанного столбца для всех записей в таблице).
*   **Условное обновление (UPDATE ... WHERE):** `UPDATE table1 SET column1=new_value, column2=new_value WHERE condition;` (Обновление значений указанных столбцов для записей, удовлетворяющих заданному условию).
*   **Полное удаление (DELETE):** `DELETE FROM table;` (Удаление всех записей из таблицы).
*   **Условное удаление (DELETE ... WHERE):** `DELETE FROM table WHERE condition;` (Удаление записей из таблицы, удовлетворяющих заданному условию).