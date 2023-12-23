# What is Javascript?

Javascript adds an *interactive* element to websites.

> Known as the scripting language for Web pages. [^1]

> Do not confuse JavaScript with the Java programming language — JavaScript is not "Interpreted Java". Both "Java" and "JavaScript" are trademarks or registered trademarks of Oracle in the U.S and other countries. However, the two programming languages have very different syntax, semantics, and use. [^1]

JavaScript documentation of core languages:

- [JavaScript Guide](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide)
- [JavaScript Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide)

> We can distingush 3 major parts of what we usually refer to as "JavaScript".

1. **The Language itself.** This is fairly standard among the various environments, both the various browsers and in the various server-side environments.
2. **The DOM API** - How the language can interact with the various parts of a web page while in the browser. While in this respect the various browsers are getting closer to each other they still differ. Several libraries, most prominently JQurey, is trying to provide a unified API.
3. *The Server **API** (API for short)* provided by Node.js or one of the other server-side systems. [^2]

When applying JavaScript to HTML, preffered to **include** an external file within the HTML similar to CSS. Another option: *Embed JavaScript directly into a line in HTML.*

- Simple example of embedded JavaScript is the **alert** function. It creates a pop-up in the browser with the text.

> `examples/js/alert.html`
`<script language="javascript"> alert ("Hello World"); </script>` [^2]

## Ways to Use JavaScript

### Embed

- Similar to inline CSS
- `<script>code>/script>`

>- A simple example of JavaScript is the **alert** function. This creates a pop-up in browser with text.

- `example/js/alert.html`
`<script language=javascript"> alert("Hello World"); </script>` [^2]

#### Include

- An external `app.js` file that should be linked in the `<head>` section tag using `app.js` attribute.
-Ex: `script src="app.js></script>`

## Variables

- let *can change*
- `declaration: let myAge: =21`
- `declaration:      myAge: =22`

- `const will never change`
- Declaration: `cost myName =Jamie`

## Data types

- Strings: text with single (`) before and after
- Numbers: any number but without quotes
- Boolean: true or false

~Note~ 

- To `comment out` on javascript, use // to start your notes.

## Conditions

- if, else, and else if
- if example:
-`const userName = prompt("What is your name?");`
- `if (userName: "Chris"){alert("Hi Instructor")}`

- else
-`else {alert("Glad you're here!);}`

- else if
- `const userName = prompt ("What is your name?");`
- `if (userName == "Chris){alert("Hi Instructor");} else if (userName == "Molly){"Hey Molly!"};{else {alert("Glad you're here!);}}`

# References:

- [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- [Introduction to JavaScript - Basic Output](https://code-maven.com/introduction-to-javascript)
- [JavaScript Input with Prompt and Confirm](https://code-maven.com/javascript-input-with-prompt-and-confirm)
- [JavaScript Variables](https://www.w3schools.com/js/js_variables.asp)

Additional References

1. [How Computers work](https://www.youtube.com/playlist?list=PLzdnOPI1iJNcsRwJhvksEo1tJqjIqWbN-)

# Answers

1. Container for storing information
2. Creates container or "variable" to store information
3. (=) is an assignment operator. Assigns the value to the variable.
4. User input.
