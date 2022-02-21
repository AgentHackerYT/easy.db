# easy.db
<div align="center">
<img src="easy.db.png" heigh="400" width="400"/>
</div>

- A Simple Database Which Uses JSON Files to store your data

- Alternative for Quick.db

- Uses No 3rd Party Dependencies

- No Complex Sqlite3 like Tool Installations

- Easy To Transfer data

# How To Use?

- Creating A Database 

```js

const { Database } = require('easy.db')

const db = new Database("path as written in fs")

// example

new Database("database.json")

```
- Add and Subtracting Values
```js 
db.add('key', 10)

db.subtract(`key`, 10)
```
- Setting Values
```js
db.set('key', "hello world")
```
- Getting Values
```js
db.get('key')
```
- Pushing Values

```js

    db.push(`key`, {some: "data"}) || db.push(`key`, ["some_data"])

```
- Deleting A Key
```js
db.delete('key')
```
- Clearing The Database
```js
db.clear()
//or
db.deleteAll()
```
- Check if the value exists or not
```js
db.has('key')
```
- All The Keys and Values
```js
db.all()
```
- Load And Save Data are Uses Less as the database automatically loads and save the keys and values
