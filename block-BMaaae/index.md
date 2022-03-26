writeCode

Write code to:-

- create a database named `sports`.
use sports
- list all databases present in local mongod server.
show dbs
- create 3 collections named `cricket`, `football`, `TT` in sports databse.
db.createCollection('cricket')
db.createCollection('football')
db.createCollection('TT')
- add multiple players in those collections which should have fields like `name`, `age` and `email` and `bid_price`.
db.cricket.insert({"name":"Kohli","age":29,"email":"xyz@gmail.com","bid_price":25000})
db.football.insert({"name":"Ronaldo","age":40,"email":"xyz@gmail.com","bid_price":35000})
db.TT.insert({"name":"Vishwa","age":22,"email":"xyz@gmail.com","bid_price":55000})
- list all collections in sports database.
show collections
- rename `TT` collection to `tennis`.
db.TT.find()
- create a capped collection called `khokho` which should have max 3 documents.
db.createCollection('khokho',{capped:true,size:100000,max:3})
db.khokho.insert({name:"raju"})
db.khokho.insert({name:"sagar"})
db.khokho.insert({name:"sameer"})
db.khokho.insert({name:"siva"})

  Try inserting more than 3 and see what happens?
- check whether a collection is capped or not?
db.khokho.isCapped()
- drop all documents from `football` collection.
db.football.remove()
- delete cricket collection completely.
db.football.drop()
- delete sports database.
db.dropDatabase()
- check which database you are connected to ?
db
- connect to test database
use test
