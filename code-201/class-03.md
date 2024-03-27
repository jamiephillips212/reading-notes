# Lists, The Box Model, and Loops

## When should you use an unordered list your HTML document?

- Inverse of the ordered list is the unordered list and it should be used when the order of your items do not matter. Such as a list of your favorite artists in no particular order, or a shopping list.

## How do you change the bullet style of unordered list items?

- Use CSS to change the list-style-type. The attribute has been deprecated.

## When should you use an ordered list vs unordered list in your HTML document?

- Use an ordered list when it contains items where order matters. I.E, the steps to build furniture, how to bake a cake, or your top 20 songs in order.
- Inverse of the ordered list is the unordered list and it should be used when the order of your items do not matter. Such as a list of your favorite artists in no particular order, or a shopping list.

## Describe two ways you can change the numbers on list items provided by an ordered list?

- To change the numbers on an unordered list, you can use either CSS or an attribute tag to style it.

## Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled: "The Box Model?"

- The margin is the outermost box in the box model. Padding is the white space between the margin and the content. Now to create the story. Disclaimer: I haven't written in ages.

- Once upon a time, a brave knight, whose name was Margin, protected his princess, princess padding, from the harms of the outside world. The knight, built walls around the castle, but princess padding told him that the walls were not enough to protect her. Princess Padding ordered a new castle to be built, where she would safely be in the middle, with her younger sister, named Content.

## List and describe the four parts of an HTML elements box as referred to by the box model

> Quoted from [Mozilla](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model)

- Content Box
- Padding Box
- Border Box
- Margin Box

- The content box is where your content will go, and is the innermost square. The padding box creates the white space between the content and margin. The border box, which can be styled, surrounds the padding box. The margin box is the outermost layer of the box model and determines the overall size of the box

## What data types can you store inside of an array?

- You can store arrays in arrays, strings, numbers, and objects.

## Is the people array a vaild JavaScript array? If so, how can I access the values stored? If not, why?

The people array is vaild JavaScript, and can be accessed in several ways.

> const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];

## List five shorthand operators for assignment in JavaScript and describe what they do

1. `x += f()` - used for additon and can be used to increase an int or even add to an array.
2. `x ?? = f()` - Nullish coalescing assignment.
3. `x *= f()` - used for mulitplication. Will multiply x by f() in this scenario.
4. `<<=` - left shift assignment, this will move the 1's in binary left by what you indicate. Such as `x <<= 2;`.
5. `x -= f()` - used for subtraction and can be used to remove items from an array or decrease an int.

## Read the code below and evaluate the last expression and explain what the result would be be and why

- without running the code, i'd assume:
dog

> let a = 10;
 let b = 'dog';
 let c = false;

 // evaluate this
 (a + c) + b;

 When excuted, it returns 10dog.

 Some dynamically typed trickery seems present here

 1. The first code adds 10 + false
 2. the false boolean and is a 0.

 It works as:
 `(10 + 0) + dog` <--- int + int + string
 `(10 + dog)` <--- int + string
`10dog` <--- JavaScript converts the int into a string when cocatenating them so this is a string.

## Describe a real world example of when a conditional statement should be used in a JavaScript program

- Simply broken down, if it's about to rain, bring an umbrella.

A conditional statement in JavaScript should be used when you have the logic requirement. If you need to evaluate and then execute on a condition.

## Give an example of when a loop is useful in JavaScript

- [ArrayPlay](<https://replit.com/@jamiep212/ArrayPlay#index.js). This example is useful when you need to ierate through an array of things.
