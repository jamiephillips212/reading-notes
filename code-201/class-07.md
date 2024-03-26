# HTML Tables and JS Constructor Functions

## Explain why we need domain modeling

## Domain modeling is a way to think through a problem without diving in code first. It can save time and money by validating ideas and allowing clear communication throughout various teams.

## Why should tables not be used for page layouts?

According to MDN you should not use tables to layout web pages because:

- It reduces accessibility.
- It produces tag soup which is essentially a bunch of nested elements that are hard to follow.
- They are not responsive automatically.
- List and describe 3 different semantic HTML elements used in an HTML `<table>`

`<td>`- Table data which contains the data for the row/column of the data.

`<tr>` - The rows of data. Each of these elements will name a particular row of data.

`<th>` - The table header. It allows the user and search engines to quickly identifty the data in columns.

## What is a constructor and what are some advantages to using it?

A constructor is just another functions; however it is meant to create a new object when called and then return that object. The main advantage to using a constructor is to keep your code DRY.

## How does the term this differ when used in an object literal versus when used in a constructor?

An object literal refers to that object. Where the constructors use of this can refers to the object the constructor created. A constructor can make virtually unlimited objects.

## Explain prototypes and inheritance via an analogy from your previous work experience

Prototypes are a way to add a method to an object in a more simplified way than specifying the method in the object itself. This eliminates needing to copy the methods into memory for each object it instead is shared between all the objects of the same type.  Inheritance is what an object knows about itself when it is created. For example: If you create a new object named person which has a name of Tim and weight of 190lbs from the person object each object created of person would have those characteristics. We have now inherited those properties from the original object.

I do not know a good analogy because I have no previous work experience.
