# Lets Mongoose

**Within your squads explore these questions**

- What is an ODM?
- What is MongooseJS?
- Why do we need MongooseJS?
- What does the word "abstraction" mean?
- How do we use mongoose?
- What are models in Mongoose?

- Define what schema means in Mongoose?
>>Everything in Mongoose starts with a Schema. Each schema maps to a MongoDB collection and
>>defines the shape of the documents within that collection.

- How do we connect to our database?

- What is a "model"?
>>A constructor compiled from schemas definitions (1:1) from a schema

- What is data denormalization and data deduplication?
>>Database normalization, or simply normalization, is the process of organizing the columns 
>>(attributes) and tables (relations) of a relational database to reduce data redundancy and
>>improve data integrity.

>>Data deduplication -- often called intelligent compression or single-instance storage --
>> is a process that eliminates redundant copies and reduces storage overhead. Data
>>deduplicatoin techniques ensure that only one unique instance of data is retained on
>>storage media. Redundant data blocks are replaced with a pointer to the unique copy data.
>>In that way, data duplication closely aligns with incremental backup, which copies only the data
>>that has changed since the precvious backup.

- What is "built-in-typecasting" in Mongoose?

- What is the "population" feature in Mongoose?
>>Population is the process of automatically replcaing the specified paths in the document
>>with documents from other collections.

- What does "virtual" do in Mongoose?

- Explain built-in-promises in Mongoose?
>>Mongoose async operations, like .save() and queries, return Promises/A+ conformant promises.
>>This means that you can do things like MyModel.findOne({}).then() and yield 
>>MyModel.findOne({}).exec()

- How are documents mapped in Mongoose?
>>Mongoose documents represent a one-to-one mapping to documents as stored in MeongoDB. Each 
>>document is an instance of its Model.

- What are custom instance methods and static methods?


- What are the 8 built-in types that we can specify for our properties in Mongoose?

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

