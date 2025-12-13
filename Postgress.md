<span style="color:rgb(0, 176, 80)"><br><br><span style="color:rgb(0, 176, 80)">\l => list all the dbs</span> <br>\c => connect to the sdata base that we created!</span> 
**for creating**  
```sql
create a table
CREATE TABLE products( 
id SERIAL PRIMARY KEY,
name VARCHAR(100),
price VARCHAR(30),
category VARCHAR(40),
stockleft INT
);
```


inserting into table =

```sql
INSERT INTO products(name, price, category, stockleft) VALUES 
('Laptop' . 23, 'electroics',12).
('Laptop' . 23, 'electroics',12).
('Laptop' . 23, 'electroics',12).
('batman' . 23, 'great',1).
('Laptop' . 23, 'electroics',12).
```

```sql | copy
SELECT * FROM products;
```


filter something!!!

```sql
SELECT * FROM product WHERE price > 400;
```

update =>

```sql
UPDATE products set stockleft=10 WHERE id=2;
```

delete =>
```sql
DELETE FROM products WHERE id=3;
```

drop table =>

``` sql

DROP TABLE  'tableName'

```


drop database => 

```sql

DROP DATABASE databaseName
example >>> DROP DATABASE  online_store

```

