writeCode

Write command to

- List collections from a database.

```mongodb
show collections
```

- create a new collection in your country database which you created recently.

```mongodb
db.createCollection()

```

Write code to:-

- crate a database named `weather`
- create a capped collection named `temperature` with maximum of 3 documents and try inserting more than 3 to see the result.
- create a simple collection named `humidity`
- check whether `temperature` collection is capped or not ?
- Delete `humidity` collection and then the entire database(weather).

```mongodb
use weather
db.createCollection('temperature', {capped:true,size:4096,max:3})
db.temperature.insert({mumbai:25})
db.temperature.insert({delhi:15})
db.temperature.insert({dehradun:8})
db.temperature.insert({ladakh:5})
db.temperature.isCapped()
db.dropDatabase()

```