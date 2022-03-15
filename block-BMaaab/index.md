writeCode

Run these shell commands in mongo shell:

- db.version() //it will show the version of  the mondoDb
- db.stats() // it will give us the stat about  the database which we are connected
- db.help() // show all the commands 

Write code to

- create a database of your country name.
```js
use india
```
- check list of databases to see newly created database.
```js
show dbs
//But  the database is not shown becasue we need to add some  documents inside it the database is empty that,s why it is not showing
```
- check which database you are currently connected to ?
// currenlty we are connected to the database which we have created now named as india.