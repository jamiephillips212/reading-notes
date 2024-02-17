# Basics of HTML, CSS, and JS

# Why is it important to use semantic elements in our HTML?

- They contain extra information for the browsers, search engines, and accessiblity devices than their non-semantic counterparts.

# How many levels of headings are there in HTML?

- There are six levels of headings in HTML. `<h1>-<h6>`

# What are some uses for the `<sup>` and `<sub>` elements?

- `<sup>` is used for superscript and `<sub>` for subscript.

> Think of the use as expressing mathmatical, engineering, chemical equations, or for dates. Super is on top like superman, and sub is on the bottom like a submarine.

# When using the `<abbr>` element, what attribute must be added to provide the full expansion of the term?

- When creating a abbreviation element you must add the `title=""` attribute to expand the term.

# What are ways we can apply CSS to our HTML?

- You can include your styling in a style element.
- You can add a CSS source file attribute to a style element.
- You can use inline styling.

# Why should we avoid using inline styles?

- Inline styles should be avoided because its easy to overlook them if you're refactoring your website. You have to change the style in EVERY HTML file to do a site wide change. It also overrides the styles in your CSS file.

# Describe the CSS code:

> `h2` {
  color: black;
  padding: 5px;
}

> h2 is the selector, color and padding are the properties, and the brackets `{}` are the declaration.

# JavaScript Basics

# What data type is a sequence of text enclosed in a single quote marks?

- String

### List 4 types of JavaScript operators?

- Not/Does not `!, !==`
- Strict euqality `===`
- Assignment `=`
- Addition `+`

# Describe a real world problem you could solve with a function?

- A function is a way to reuse code. Anytime you're going to repeat code, use functions. Write it once and call/invoke it unlimited times.

# An `if statement checks a _ and if it evaluates to _,` then the code block will excute?

- Condition true

# What is the use of an `else if`

- You'd use an `else if` to continue checking a condition until one or the `else` is executed.

# List 3 different types of comparison operators?

- `==` tests if a value is the same as one another.
- `<` compares if one value is less than another.
- `>=` compares if a value is greater than or equal to another.

# What is the difference between the logical operator && and ||?

- By using `&&` you are checking if multiple statements both evaulate to true.

> if (imTired === true && isItBedtime === true) [
  // I am tired and it is bedtime..
  goToBed();
]

By using || also known as pipes, you are comparing mulitple statements and executing code if one condition returns true.

> if(imTired === false || imSick === true){

  Even though imTired is false, imSick is true, and so we are going to bed.
}

## Things I want to know more about:

-How to use boolean correctly.
