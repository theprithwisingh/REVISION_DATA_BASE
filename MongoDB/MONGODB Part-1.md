# MONGODB

| RDBMS | MONGODB |
| --- | --- |
| Database | Database |
| Tables | Collection |
| Rows | Document |
| columns | Fields or keys |

### **How to create database in MongoDB**

**Step1**: `show db_name` and here Practicing name of database is `latest_db`

**How to create collections/table in MongoDB**

**step2**:  `db.students.insertOne()`  or Only first create collection `db.createCollection(collection_name)`

`students` is collections.

### **How to add data in collection or table in MongoDB**

**step3:**

```json
db.students.insertOne(key1:"value1",key2:"value2",key3:"value3"...)
```

![Screenshot 2024-04-21 172139.jpg](MONGODB%201595eb0e97d845c792956a6fca48b5fd/Screenshot_2024-04-21_172139.jpg)

### **How to show database  collection or table ,which is insert above  in MongoDB**

**Step4**: `db.students.find()`

![Screenshot 2024-04-21 172608.jpg](MONGODB%201595eb0e97d845c792956a6fca48b5fd/Screenshot_2024-04-21_172608.jpg)

### **How to update  database>collection or table with Nesting document limit MongoDB**

**Step5:** `db.students.updateOne({name:"Ram"},`

`{$set:{idCards:{`

`hasPanCard:false,hasAadharCard:true`

`}}})`

What is `$set`

`$set` is an update operator in MongoDB that modifies the value of a field in a document. It allows you to update specific fields within a document without overwriting the entire document.

For example-

 if you have a document with fields **`name`**, **`age`**, and **`address`**, and you want to update only the **`address`** field, you can use **`$set`** to modify just that field while leaving the other fields unchanged.

how you would use **`$set`** in an update operation : CLI

```json
db.collection.updateOne(
   { <query> },
   { $set: { <field1>: <value1>, <field2>: <value2>, ... } }
)
```

![Screenshot 2024-04-21 195949.jpg](MONGODB%201595eb0e97d845c792956a6fca48b5fd/Screenshot_2024-04-21_195949.jpg)

### **How to find updated collection’s field’s value ??**

**Step6:**`db.students.findOne({name:'ram'})`

![Screenshot 2024-04-21 202915.jpg](MONGODB%201595eb0e97d845c792956a6fca48b5fd/Screenshot_2024-04-21_202915.jpg)

### **How to update collection’s all field’s value ??**

**Step7:**