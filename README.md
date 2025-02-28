1. INSERT INTO table (column1, column2) VALUES (value1, value2);

INSERT INTO: Эта команда говорит базе данных, что мы хотим добавить новую запись (строку) в таблицу.
 table: Здесь нужно указать имя таблицы, в которую ты хочешь добавить данные. Например, customers, products, orders и т.д.
(column1, column2): Это список столбцов, в которые мы будем вставлять данные. Каждый столбец должен существовать в указанной таблице (table). Например, если таблица customers содержит столбцы id, name, email, ты можешь указать (name, email). Важно перечислить столбцы в правильном порядке.
 VALUES: Эта команда говорит базе данных, что дальше идут значения для вставки.
(value1, value2): Это значения, которые ты хочешь вставить в соответствующие столбцы. value1 будет вставлено в column1, value2 будет вставлено в column2. Важно, чтобы тип данных значения соответствовал типу данных столбца (например, число в числовой столбец, текст в текстовый столбец). Значения указываются в том же порядке, что и столбцы.
Пример:
INSERT INTO customers (name, email) VALUES ('Иван Иванов', 'ivan@example.com');

2. INSERT INTO table (column1, column2) VALUES (value11, value12), (value21, value22), ...;

Это расширенная версия предыдущего запроса, позволяющая добавить сразу несколько записей в таблицу.
Пример: INSERT INTO products (name, price) VALUES ('Яблоко', 50), ('Банан', 70), ('Апельсин', 90);

3. INSERT INTO table1 (column1, column2) SELECT (col1, col2) FROM table2;

Этот запрос позволяет добавить данные в одну таблицу (table1) из другой таблицы (table2).

•  INSERT INTO table1 (column1, column2): Как и ранее, указывает, в какую таблицу и в какие столбцы мы хотим добавить данные.
•  SELECT (col1, col2) FROM table2: Это SELECT запрос, который выбирает данные из таблицы table2. col1 и col2 - это столбцы из table2, которые мы хотим вставить в column1 и column2 в table1 соответственно. Важно, чтобы типы данных col1 и col2 были совместимы с типами данных column1 и column2.

Пример: INSERT INTO employees (name, department_id) SELECT full_name, dept_id FROM new_employees;

4. UPDATE table1 SET column1 = new_value;

Эта команда позволяет изменить существующие данные в таблице.

•  UPDATE table1: Указывает, какую таблицу мы хотим обновить.
•  SET column1 = new_value: Устанавливает новое значение (new_value) для столбца column1. Все записи в таблице table1 будут изменены! Это очень важно помнить.

Пример: UPDATE products SET price = 100;

5. UPDATE table1 SET column1 = new_value, column2 = new_value WHERE condition;

Это более безопасная и полезная версия команды UPDATE. Она позволяет изменить данные только для тех записей, которые соответствуют определенному условию.

•  UPDATE table1 и SET column1 = new_value, column2 = new_value: Работают так же, как и раньше. Можно обновлять значения нескольких столбцов, разделяя их запятыми.
•  WHERE condition: Это условие, которое определяет, какие записи будут обновлены. Условие может быть любым логическим выражением, которое возвращает TRUE или FALSE. Например, id = 5, price > 100, name = 'Иван', и т.д.

Пример:UPDATE customers SET email = 'new_email@example.com' WHERE id = 123;

6. DELETE FROM table;

Эта команда удаляет все записи из таблицы.

•  DELETE FROM: Указывает, что мы хотим удалить данные.
•  table: Указывает имя таблицы, из которой мы хотим удалить данные.

Пример: DELETE FROM products;

7. DELETE FROM table WHERE condition;

Это более безопасная версия команды DELETE. Она позволяет удалить только те записи, которые соответствуют определенному условию.

•  DELETE FROM table: Работает так же, как и раньше.
•  WHERE condition: Условие, которое определяет, какие записи будут удалены.

Пример:DELETE FROM orders WHERE status = 'cancelled';
