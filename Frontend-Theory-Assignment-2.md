# Frontend: Theory Assignment 2

## 1. What is CSS Box Model?

The CSS Box Model describes how every HTML element is represented as a rectangular box. It consists of four parts:

1. Content – The actual text or content of the element.
2. Padding – Space between the content and the border.
3. Border – A line surrounding the padding and content.
4. Margin – Space outside the border that separates the element from other elements.

Example:

```css
div {
    width: 200px;
    padding: 20px;
    border: 5px solid black;
    margin: 10px;
}
```

## 2. What is a Media Query? Explain with a sample code.

A media query is a CSS technique used to apply different styles to a webpage depending on the device or screen size. It is commonly used to make websites responsive.

Example:

```css
body {
    background-color: white;
}

@media screen and (max-width: 600px) {
    body {
        background-color: lightblue;
    }
}
```

## 3. What are the features of Bootstrap?

Bootstrap is a popular front-end framework used to create responsive and mobile-friendly websites.

Main features include:

- Responsive grid system
- Mobile-first design
- Predefined CSS classes
- Ready-made UI components
- Responsive utilities
- Buttons, forms, cards, navigation bars, and other components
- Cross-browser compatibility
- Easy and fast development

## 4. Write an example of basic grid structure in Bootstrap.

Bootstrap uses a 12-column grid system. A basic grid structure can be created using containers, rows, and columns.

Example:

```html
<div class="container">
    <div class="row">
        <div class="col">Column 1</div>
        <div class="col">Column 2</div>
        <div class="col">Column 3</div>
    </div>
</div>
```

## 5. What are CSS Selectors?

CSS selectors are patterns used to select HTML elements that we want to style.

Common types of selectors are:

- Element selector
- ID selector
- Class selector
- Universal selector
- Group selector
- Attribute selector
- Descendant selector
- Child selector

Examples:

```css
p {
    color: blue;
}

#heading {
    color: red;
}

.box {
    background-color: yellow;
}
```

## 6. What are CSS backgrounds? List the properties.

CSS background properties are used to set and control the background of an HTML element.

Important background properties include:

- `background-color`
- `background-image`
- `background-repeat`
- `background-position`
- `background-size`
- `background-attachment`
- `background-origin`
- `background-clip`

Example:

```css
body {
    background-color: lightblue;
    background-image: url("image.jpg");
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
}
```

## 7. How can we overlap elements in CSS?

Elements can be overlapped by using CSS positioning along with the `z-index` property.

Example:

```css
.box1 {
    position: absolute;
    top: 50px;
    left: 50px;
    z-index: 1;
}

.box2 {
    position: absolute;
    top: 80px;
    left: 80px;
    z-index: 2;
}
```

The element with the higher `z-index` appears in front of the element with the lower `z-index`.

## 8. What are the different positioning properties in CSS?

CSS provides the following main positioning values:

1. `static` – Default position of an element.
2. `relative` – Positions an element relative to its normal position.
3. `absolute` – Positions an element relative to its nearest positioned ancestor.
4. `fixed` – Positions an element relative to the browser viewport.
5. `sticky` – Acts like relative positioning until a specified scrolling point, then behaves like fixed positioning.

Example:

```css
.box {
    position: relative;
    top: 20px;
    left: 30px;
}
```

## 9. What is ECMAScript?

ECMAScript is a standard specification that defines the rules and features of scripting languages. JavaScript is the most widely used implementation of ECMAScript.

ECMAScript defines features such as variables, functions, objects, classes, operators, and modern JavaScript syntax.

## 10. What is the difference between var, let and const in JavaScript? Explain Temporal Dead Zone.

### Difference between var, let and const

| Feature | var | let | const |
|---|---|---|---|
| Scope | Function scoped | Block scoped | Block scoped |
| Redeclaration | Allowed | Not allowed in same scope | Not allowed in same scope |
| Reassignment | Allowed | Allowed | Not allowed |
| Hoisting | Hoisted and initialized as `undefined` | Hoisted but not initialized | Hoisted but not initialized |

Example:

```javascript
var a = 10;
a = 20;

let b = 10;
b = 20;

const c = 10;
// c = 20; // Error
```

### Temporal Dead Zone (TDZ)

The Temporal Dead Zone is the period between entering a block and the point where a `let` or `const` variable is declared. During this period, the variable cannot be accessed.

Example:

```javascript
console.log(x); // ReferenceError
let x = 10;
```

The error occurs because `x` is in the Temporal Dead Zone until its declaration is reached.
