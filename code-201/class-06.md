# Domain Modeling, Intro to the DOM, and Object Literal Notion

## How would you describe an object to a non-technical friend you grew up with?

An Object is a collection of things relating to a thing. Such as a person may be an object and this object has a name, height, weight, and functions as in maybe they can code or play soccer.

## What are some advantages to creating object literals?

 Object literals are already written and ready to go objects. They can be added to or changed, however, for the most part it is literal and great for structured data.

## How do objects differ from arrays?

You refer to elements in an array by index and by name in objects.

## Give an example for when you would need to use bracket notation to access an object's property instead of dot notation

If you needed to access a property of an object that is in a variable name.

## Evaluate the code below. What does the term this refer to and what is the advantage to using this?

> const dog = {
 > name: 'Spot',
  > age: 2,
  > color: 'white with black spots',
  > humanAge: function (){
    > console.log(`${this.name} is ${this.age*7} in human years`);
  }
}
 `this` refer to this instance of dog or this object. The use of this is good for scoping, multiple instances of an object, and for the use with constructors[https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics]

## What is the DOM?

 The document object model or the DOM is a representation of objects that compromise the structure and content of a document on the web[https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction]. This allows Javascript to manipulate and work with the web page.
