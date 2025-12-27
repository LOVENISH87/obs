mongo in node1!!
[[batman]]
[[socket.io]]
create a db -> <mark style="background: #ABF7F7A6;">use db</mark>, it will create db database 

<mark style="background: #ADCCFFA6;">show collections</mark> will show collection "json data stored in database!!"

now to create collections we use <mark style="background: #D2B3FFA6;">db.createCollection('name_of_the_collection')</mark>;

to see the collections that we just created type <mark style="background: #FF5582A6;">'show Collection'</mark>

to insert in s

to show the inside -> use<mark style="background: #FFB86CA6;"> db.Collection.find() , or better use pretty()</mark> after the function!!!


to find something use <mark style="background: #BBFABBA6;">db.Collection.find({name : "love"})</mark> , this is for searching one item1!!!

to find using condition ->> <mark style="background: #FFB8EBA6;">db.student.find({section:{$gt:20}}) and {$lt:23}</mark>


and gte ->> greatet ">="  && lte <<- "<="


to sort =>> uni> <mark style="background: #ABF7F7A6;">db.collection.find().sort({_id: 0})</mark>






some shit i did -> 
```js

]
uni>  db.student.find({section:{$gt:20}})

uni> 
(To exit, press Ctrl+C again or Ctrl+D or type .exit)
uni> db.Collection.find({name : "batman"})
[
  {
    _id: ObjectId('6932a912b026075c598de666'),
    name: 'batman',
    age: 23
  },
  {
    _id: ObjectId('6932a929b026075c598de667'),
    name: 'batman',
    age: 23
  },
  {
    _id: ObjectId('6932a93bb026075c598de668'),
    id: 0,
    name: 'batman',
    age: 23
  },
  {
    _id: ObjectId('6932a946b026075c598de669'),
    id: 0,
    name: 'batman',
    age: 23
  }
]
uni> db.Collection.find({name : "love"})
[
  {
    _id: ObjectId('6932a9f6b026075c598de66a'),
    name: 'love',
    class: 'big dih',
    section: 'goon'
  }
]
uni> db.collection.find().sort({_id: 0})
MongoInvalidArgumentError: Invalid sort direction: 0
uni> db.collection.find().sort({_id})
ReferenceError: _id is not defined
uni> db.collection.find().sort({name : "love"})
MongoInvalidArgumentError: Invalid sort direction: "love"
uni> db.COllection.updateOne({name: "batman"} , {
... $set: {city:"gotham"}})
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 0,
  modifiedCount: 0,
  upsertedCount: 0
}
uni> db.COllection.updateOne({ name: "batman" }, { $set: { age: 22 } })
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 0,
  modifiedCount: 0,
  upsertedCount: 0
}
uni> db.COllection.updateMany({ name: "batman" }, { $set: { age: 22 } })
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 0,
  modifiedCount: 0,
  upsertedCount: 0
}
uni> db.countDocuments()
TypeError: db.countDocuments is not a function
uni> db.Collections.countDocuments()
0
uni> db.Collection.countDocuments()
6
uni> db.Collection.updateMany({ name: "batman" }, { $set: { age: 22 } })
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 4,
  modifiedCount: 4,
  upsertedCount: 0
}
uni> 



```


```json

uni> db.stats()
{
  db: 'uni',
  collections: Long('2'),
  views: Long('0'),
  objects: Long('6'),
  avgObjSize: 60,
  dataSize: 360,
  storageSize: 40960,
  indexes: Long('2'),
  indexSize: 40960,
  totalSize: 81920,
  scaleFactor: Long('1'),
  fsUsedSize: 71788371968,
  fsTotalSize: 160531959808,
  ok: 1
}
uni> 

```


<mark style="background: #FF5582A6;">
db.dropDatabase() drop !!!</mark>

<mark style="background: #FFF3A3A6;">db.Collection.drop();</mark>


[[GitHub]]