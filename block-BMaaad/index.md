writeCode

Write command to

- List collections from a database.
```js
show nothing because there is no more collection in the database
```
- create a new collection in your country database which you created recently.
```js
db.createCollections('HimacalPradesh')
```
Write code to:-

- crate a database named `weather`
- create a capped collection named `temperature` with maximum of 3 documents and try inserting more than 3 to see the result.
```js
db.createCollection(`temperature`,{capped:true,size:500 max:3})

```
- create a simple collection named `humidity`
db.createCollection( `humidity`)
- check whether `temperature` collection is capped or not ?
```js
db.collection.isCapped()

``
- Delete `humidity` collection and then the entire database(weather).
db.temperature.drop()
db.dropDatabase()
```

