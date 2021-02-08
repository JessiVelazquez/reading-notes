# **Javascript**

Javascript makes web pages interative. Example are:
- Slideshows
- Forms
- Partial page reloads
- Filtering data

## **Script**

A script is a series of instructions for the computer, akin to:
- a recipe
- a handbook 
- a manual

The goal needs to be defined first.
- Tasks must be defined, then broken down into series of steps.
- remember a computer only understands commands it already knows (delete, add, open, etc), and yes/no binary questions.

## **Computers think programmatically**

- Recall that everything eventually boils down to 1's and 0's. Everything else is achieved through abstraction.

**Objects**

- Objects have properties:
    - If the object is a car, its properties could be:
        - *Make*
        - *Color*
        - *CurrentSpeed*
        - *FuelType*

- Objects have events:
    - If the object is a car, events could be:
        - *brake*
        - *accelerate*

- Objects have methods:
    - If the object is a car, methods could be:
        - changespeed() - increases or decreases the value of *currentspeed* property

**A Script puts these things together**

- **Events** can trigger **methods**
- **Methods** can retrieve or update an objects's **properties**

**The Document Object**

- Models the current webpage loaded into a browser.

    - Properties are things like the URL, title, last modified, etc

    - **Events** are things like load, click, keypress.

    - **Methods** are things like 
        - write() - adds new content to the document
        - getElementbyID() - access an element when you state its ID

**How a Browser Sees a Page**

1. Browser reveives HTML page.
2. Browser creates a model and stores it in memory.
    - Like a family tree where the head is document object, then the html object, and then branching out into various other objects, taken from the HTML structure, which are called **nodes**.
3. Browser shows the page on the screen using a **rendering engine**
    - The rendering engine uses either default stylings for HTML elements, otherwise it will use the CSS style sheet you call in your script.

**Fitting HTML, CSS, and Javascript together**
- HTML is content layer
- CSS is presentation layer 
    - Called by using the ```<link src="stylesheet.css"></link>``` element in HTML file
- Javascript behavior layer 
    - Called by using the ```<script src="javascriptfile.js"></script>``` element in HTML file

## **Parts of a Script**

Expressions
- evaluate into a single value

```
var color = 'beige';
```

or

```
var area = 3 * 2;
```

Operators
- Allow programmers to create a single value from one or more values.
- like '+', '-', or '>'

```
greeting = 'Hi" + 'Molly';
```

- Arthimethic operators, and string operators.
- String operator is '+', which concatenates, or joins two strings.

## **Functions**

- Allow you to group a series of statements together to perform a specific task.
- Can be reused in different parts of the script, or in two different scripts.
- To write a function, give it a name and then write the statements needed to achieve its task inside the curly braces. Known as **function declaration**:

```
function sayHello() {
    document.write('Hello!');
}
```

- Calling a function:
- Since you have defined (named) the function above, you can call it with just one line of code:

```
sayHello();
```

- If a function needs more info, declare like this (where **width** and **height** are known as *parameters*):

```
function getArea(width, height) {
    return width * height;
}
```

- Then, call that function (with parameters) like this:

```
getArea(3, 5);
```

- Getting a single value out of a function:

```
function calculateArea(width, height) {
    var area = width * height;
    return area;
}
var wallOne = calculateArea(3, 5);
var wallTwo - calculateArea(8, 5);
```