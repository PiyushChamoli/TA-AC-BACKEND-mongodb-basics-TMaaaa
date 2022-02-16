writeCode

Write code to:-

- create a database named `mountains`
- a collection inside that database named `himalayas`
- insert 1 document into that collection `{name: 'Dhauldhar range', height: '4000 mtrs'}`

- insert multiple document using insertMany command
- find all documents from mountains
- find a single document using name

[
    {
        name: 'Dhauldhar range 2', height: '5000 mtrs'
    },
    {
        name: 'Dhauldhar range 3', height: '6000 mtrs'
    },
    {
        name: 'Dhauldhar range 4', height: '7000 mtrs'
    }
]


```
use mountains
db.himalayas.find({height: "4000 mtrs"})
db.himalayas.update({height: "4000 mtrs"},{$set:{name:"Dhauldhar range 1}})
```