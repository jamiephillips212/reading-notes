# Design Web Pages with CSS

What is CSS?

- CSS or "Cascading Style Sheets" used to manipulate HTML from its default styling.

- Example:
`Selector {
    property: value:
}`

## Good Practice

- Keep HTML and CSS in seperate files.

### How to start

- In working repository and alongside your **index.html** file, create a **style.css** file.
- `<link>` the two files by adding `<link rel="stylesheet" href"style.css"` in the `<head>` section  below the `<title>` element in the HTML file.
- This will link the HTML and CSS files.

### Applying CSS

#### Selectors

- When using CSS, the selector indentifies the location in the HTML code where the style will be applied. This allows the style to be applied specifically or broadly.
- Options are a path, id, and class.
- Path: `<nav>` <ul> <li>
- Unique ID:

- HTML
- CSS

- Class
- `.class-name { property: value; }`

### Property and Value

- The property can be font, size, color, etc
- The value is what you want to change the property to
- EX: `header {background-color : purple; font-size: 6em; }`

> Note that the colon seperates the property and value, while the semi-colon seperates sets of properties and values

- To apply the above styles, that would be written in the style. css file, insert `style background-color: purple; font-size: 6em;` as an attribute to the appropriate element in the HTML. This case, it would be inserted  one space after the `"header"` in the opening tag.
- EX: `<header style="background-color: purple; font-size 6em;>Heading Number One Text</header>`

### Answers

- A style language used to alter/manipulate apperance of HTML's standard structure
- Three ways to add CSS into project:

- External CSS
- Achieved by adding a reference to a style sheet in the `<head>` section of the HTML page(s). Must be saved in a .css extension and is housed in the working repository with the HTML file.

- Internal CSS
- Refers to a style sheet being added into the HTML file instead of  external CSS file.

- Inline CSS
- Used to apply desired style to a single element.

- `p { color: red;}`
