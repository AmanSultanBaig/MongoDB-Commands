## Basic Of MongoDB Commands

In MongoDB if you want to see all databases so write command `> show dbs` & if you want to see all collections so write command `> show collections`

If you want to get search something in your collection/Table so write `db.mycollection.find({})`, this command will execute like 
```ruby 
select * from Table
``` 
in Sql Server / MySQL [RDMS]

### 1. Create Database

In MongoDB use, DATABASE_NAME is used to create a database. If this name database doesn’t exist, it will get created, else it will return the existed one.

`> use databaseName`

To check the current database now:

`> db`

### 2. Drop Database
`> databaseName.dropDatabase()`

If the database is not specified, then it will delete the default database that is “test”.

### 3. Create Collection

To create collection, the MongoDB command used is:  **db.createCollection(name, options).** 

Here, the name is the name of the collection & options is a document which is used to specify the configuration of the collection. Though “Options” parameter is optional, it’s good to provide it.

### 4. Drop Collection
`db.mycollection.drop()`

### Insert Document
Inserts a document or documents into a collection.
The **insert()** method has the following syntax:
```ruby
// with json objects
db.collectionName.insert({name:"Aman Sultan",postion:"JS Developer"})
```


