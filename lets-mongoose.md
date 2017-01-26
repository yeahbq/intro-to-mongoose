# Lets Mongoose

**Within your squads explore these questions**

- What is an ODM?
- What is MongooseJS?
- Why do we need MongooseJS?
- What does the word "abstraction" mean?
- How do we use mongoose?
- What are models in Mongoose?
- Define what schema means in Mongoose?
- How do we connect to our database?
- What is a "model"?
- What is data denormalization and data duplication?
- What is "built-in-typecasting" in Mongoose?
- What is the "population" feature in Mongoose?
- What does "virtual" do in Mongoose?
- Explain built-in-promises in Mongoose?
- How are documents mapped in Mongoose?
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

