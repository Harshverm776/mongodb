# MongoDB

## Commands

* **Log-**  
`mongo -u <username> -p <password> --authenticationDatabase <dbname>`  

* **Show All Databases-**  
`show dbs`  

* **Select DB-**  
`use databaseName`  

* **Authenticate-**  
`db.auth("username", "password")`  

* **Logout-**  
`db.logout()`  

* **List collections-**  
`show collections;`  
`db.getCollectionNames();`  

* **List Users-**  
`show users;`  
`db.getUsers();`  

* **List roles-**  
`show roles`  

* **Create collection-**  
`db.createCollection("collectionName");`  

* **Insert document-**  
`db.<collectionName>.insert({field1: "value", field2: "value"})`  
`db.<collectionName>.insert([{field1: "value1"}, {field1: "value2"}])`  
`db.<collectionName>.insertMany([{field1: "value1"}, {field1: "value2"}])`  

* **Save or Update-**  
`db.<collectionName>.save({"_id": new ObjectId("jhgsdjhgdsf"), field1: "value", field2: "value"});`  

* **Display records-**  
`db.<collectionName>.find();`  
`db.<collectionName>.find().limit(10);`  
`db.<collectionName>.find({"_id": ObjectId("someid")});`  
`db.<collectionName>.find({"_id": ObjectId("someid")}, {field1: 1, field2: 1});`
`db.<collectionName>.find({"_id": ObjectId("someid")}, {field1: 0});`  
`db.<collectionName>.count();`
