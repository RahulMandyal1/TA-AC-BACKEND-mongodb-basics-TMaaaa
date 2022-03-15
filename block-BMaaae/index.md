writeCode

Write code to:-

- create a database named `sports`.
```js
use sports 
```
- list all databases present in local mongod server.
```js
show dbs
```

- create 3 collections named `cricket`, `football`, `TT` in sports databse.
```js
db.createCollections('cricket');
db.createCollections('football');
db.createCollections('TT');
```

- add multiple players in those collections which should have fields like `name`, `age` and `email` and `bid_price`.
```js
db.cricket.insert({name : "Rahul Thakur" , age: 19 , email : 'iamrahu;079@gmail.com',bid_price : '1cr'})
db.football.insert({name : "Rahul Thakur" , age: 19 , email : 'iamrahu;079@gmail.com',bid_price : '1cr'})
db.TT.insert({name : "Rahul Thakur" , age: 19 , email : 'iamrahu;079@gmail.com',bid_price : '1cr'})
```

- list all collections in sports database.
show collections
- rename `TT` collection to `tennis`.
```js
db.renameCollection('tennis');
```
- create a capped collection called `khokho` which should have max 3 documents.

```js
db.createCollection('khokho',{capped: true , size:500 , max:3})
```
  Try inserting more than 3 and see what happens?
- check whether a collection is capped or not?
```js
db.khokho.isCapped();//true
```
- drop all documents from `football` collection.
```js
db.football.remove()
```
- delete cricket collection completely.
```js
db.cricket.drop()
```
- delete sports database.
```js
db.dropDatabase()
```
- check which database you are connected to ?
```js
still connected to sports databas
```
- connect to test database
```js
use test
```