## Напишіть SQL-запит, який для таблиці orders виводить на екран атрибут id, атрибут date та JSON-об’єкт {"id": <атрибут id рядка>, "date": <атрибут date рядка>}. Для створення JSON-об’єкта використайте функцію. (Рисунок-5)  

```sql
USE hw_03;

SELECT
	id
    ,date
    ,JSON_OBJECT('id', id, 'date', date)
FROM orders
```

*Рисунок-5*  
![alt text](Рисунок-5.png)  
