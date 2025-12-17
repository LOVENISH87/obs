

its a relatinoal data base1!!!!
#keys
#primary_key

<span style="color:rgb(0, 176, 80)"><br><br><span style="color:rgb(0, 176, 80)">\l => list all the dbs</span> <br>\c => connect to the sdata base that we created!</span> 
\du -> select rows
\dn  => database schema 
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



### row and cols -> tuple and 


~ ❯❯❯ function post
          pgcli -U batman -d postgres -h localhost 
      end
~ ❯❯❯ funcsave post

fish function for postgres



insert into postgres man- >>>"

```sql

CREATE TABLE student(
    name VARCHAR(23),
    age INT ,
    city VARCHAR(23)
)


INSERT INTO student(name, age, city) VALUES ('batman', 34,'saving goth');
```


)<span style="color:rgb(0, 176, 80)">pg lib in node or express</span> 


``` sql

async function createUser() {

const rest = await pool.query(

"INSERT INTO student (name, age, city) VALUES ($1, $2, $3)",

['Robin' , 34, 'gotham']

)

console.log("student inserted", rest.rows[0]);

  

}

  

async function readUser() {

const rest = await pool.query(

"select * from student"

)

console.log("All students" , rest.rows)

}


```

