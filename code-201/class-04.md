# Links, Layouts, and Functions

## To create a basic link, we wrap text or other content inside what element?

`<a></a>`

## The href attribute contains what information?

The address to which the element links.

What are some ways we can ensure links on our pages are accessible to all readers?
According to Mozilla

- Use clear link wording
- Use keywords in link text
- Understand that some readers skim and will be drawn to links and other page features

## What is meant by “normal flow”?

- Normal flow is the default way that elements lay themselves out without modification.

## What are a few differences between block-level and inline elements?

As found on [Mozilla](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Positioning)

Block-level elements are laid out vertically. Block-level always starts on a new line, and the vertical space is equal to its content. Inline-level content is aligned either vertically or horizontally depending on their text. Inline-level elements can be changed with CSS.

## ___ positioning is the default for every html element

Normal flow

## Name a few advantages to using absolute positioning on an element

Absolutely positioned, sits on it's own layer seperate from other things. This makes it useful for UI features, pop-ups, and more.

## What is a key difference between fixed positioning and absolute positioning?

Fixed positioning positions itself relative to the viewport where absolute positioning positions itself to it's nearest ancestor.

## Describe the difference between a function declaration and a function invocation

function helloWorld() {} <--- This is the declaration

helloWorld(); <--- This is the invocation

The difference is the function contains the logic and code to be executed, however, the invocation is what tells the program to execute the function.

For example:

function helloWorld(){
  console.log('Hello World!');
}

// The above code will never execute until it is invoked.

helloWorld(); // Note the (); this indicates a function is being called/invoked.
What is the difference between a parameter and an argument?
Building on the above example and making it more awesome...

function helloWorld(parameter1, parameter2){
  console.log('Hello ' + parameter1 + ' you\'re the most awesome person on ' + parameter2 + '!');
}

// The above code will never execute until it is invoked.
// Note the (); this indicates a function is being called/invoked.

helloWorld('mochi', 'Earth'); // Now note the invocation using arguments.

// You can also pass variables as arguments...
let coolPerson = 'mochi';
let planetHeLives = 'Earth';

// This invocation will produce the exact same console.log as the prior.
helloWorld(coolestPersonEverOfAllTime, planetHeLives);

// In addition you can also pass other things like arrays or functions themselves as arguments.

## Pick 2 benefits to pair programming and reflect on how these benefits could help you on your coding journey

Social skills - I am super anti-social.
Engaged Collaboration - I want to be able to talk to my programming partner and make sure we're both on task and not procrastinating.
