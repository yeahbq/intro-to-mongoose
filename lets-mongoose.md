# Lets Mongoose

**Within your squads explore these questions**

##- What is an ODM?
Mongoose is to MongoDB as ActiveRecord is to a SQL database. However, because it maps code to
Mongo's documents, it is referred to as an Object Document Mapper (ODM) instead of an ORM, but 
their general purpose is the same.

##- What is MongooseJS?
"Mongoose provides a straight-forward, schema-based solution to model your application data"

##- Why do we need MongooseJS?
Mongoose allows us to define schemas and ensures that documents conform.
Using the Mongoose ODM is by far the most popular way to perform CRUD on a MongoDB.

##- What does the word "abstraction" mean?
A way to remove complexity and being able to work without worrying on the details

##- How do we use mongoose?
Install mongoose driver for nodemodule locally (npm install --save mongoose).
Require it (var mongoose = require('mongoose') )

##- What are models in Mongoose?
Constructors compiled from schemas. Scehmas are the blueprints/settings and models are the instance
to be able to perform CRUD operations on mongoDB.

##- Define what schema means in Mongoose?
Everything in Mongoose starts with a Schema. Each schema maps to a MongoDB collection and
defines the shape of the documents within that collection.

##- How do we connect to our database?
var mongoose = require('mongoose');
mongoose.connect('mongodb://localhost/movies');

##- What is a "model"?
A constructor compiled from schemas definitions (1:1) from a schema. Required to perform CRUD on 
mongoDB.

##- What is data denormalization and data deduplication?
Database normalization, or simply normalization, is the process of organizing the columns 
(attributes) and tables (relations) of a relational database to reduce data redundancy and
improve data integrity.

Data deduplication -- often called intelligent compression or single-instance storage --
 is a process that eliminates redundant copies and reduces storage overhead. Data
deduplicatoin techniques ensure that only one unique instance of data is retained on
storage media. Redundant data blocks are replaced with a pointer to the unique copy data.
In that way, data duplication closely aligns with incremental backup, which copies only the data
that has changed since the precvious backup.

##- What is "built-in-typecasting" in Mongoose?
Converting data from one type to another (ie number to string). Non-destructive and only performs
on that specific transaction (a query that only hits once).

##- What is the "population" feature in Mongoose?
Population is the process of automatically replcaing the specified paths in the document
with documents from other collections.

##- What does "virtual" do in Mongoose?
Virtual properties - create properties like "fullName" that are not persisted in the database.
Is like an object.
```
user.virtual {
    fullName: firstName + lastName
}
```

##- Explain built-in-promises in Mongoose?
Mongoose async operations, like .save() and queries, return Promises/A+ conformant promises.
This means that you can do things like MyModel.findOne({}).then() and yield 
MyModel.findOne({}).exec()

##- How are documents mapped in Mongoose?
Mongoose documents represent a one-to-one mapping to documents as stored in MeongoDB. Each 
document is an instance of its Model.

##- What are custom instance methods and static methods?
Custom Instance methods which operate on the document (id 1984.findsimilar() )
Static methods which operate on the entire collection (ie db.collection.find() )

##- What are the 8 built-in types that we can specify for our properties in Mongoose?
```
*String
*Number
*Boolean
*Date
*Array - []
*mongoose.Schema.Types.ObjectId
*mongoose.Schema.Types.Buffer
*mongoose.Schema.Types.Mixed
```


**Review this code snippet from Mongoose's homepage**

```
var mongoose = require('mongoose');
mongoose.connect('mongodb://localhost/test');

var Cat = mongoose.model('Cat', { name: String });

var kitty = new Cat({ name: 'Zildjian' });
kitty.save(function (err) {
  if (err) {
    console.log(err);
  } else {
    console.log('meow');
  }
});

```

**Resources**
[Google Search Engine is your best friend](https://www.google.com/)
[Mongoose Official Doc](http://mongoosejs.com/)
[Mongoose Gist ppt](https://gist.github.com/jim-clark/85fb003f3063e6d152da8a1ab51a51ab)

