writeCode

Write code to:-

- create a database named `sports`.
- list all databases present in local mongod server.
- create 3 collections named `cricket`, `football`, `TT` in sports databse.
- add multiple players in those collections which should have fields like `name`, `age` and `email` and `bid_price`.
- list all collections in sports database.
- rename `TT` collection to `tennis`.
- create a capped collection called `khokho` which should have max 3 documents.
  Try inserting more than 3 and see what happens?
- check whether a collection is capped or not?
- drop all documents from `football` collection.
- delete cricket collection completely.
- delete sports database.
- check which database you are connected to ?
- connect to test database


Answers:
```
use sports
show dbs
db.cricket.insertMany(players)
db.football.insertMany(players)
db.TT.insertMany(players)
show collections
db.TT.renameCollection('tennis')
db.createCollection('khokho', {capped:true,size:4096,max:3})
db.khokho.insertMany(players)
db.khokho.isCapped()
db.football.remove({})
db.cricket.drop()
use test
```