# Readings

## Javascript Objects basic

In basic terms objects in Javascript are a collection of data or function. For example we can define a variable as

```js

const name = {};

```

This is an example of an object. When the code is ran through the browser nothing will appear but when *name* is typed in the console the retrun value will be {}.

One of the advantages of using object literals sending a single object with multiple data in them is much more efficiant than sending serval items individually.

Objects differ from arrays because objects can be called by the asscociated value instead of using the index number to select an item.

One example of using the bracket notation would be 

```js

person['age'];
person['name']['first']

```

### Evaluate the code below What does the term this refer to and what is the advantage to using this

```js

const dog = {
  name: 'Spot',
  age: 2,
  color: 'white with black spots',
  humanAge: function (){
    console.log(`${this.name} is ${this.age*7} in human years`);
  }
}

```

this refers to the current object the code is being written inside. In this case this would be name & age.