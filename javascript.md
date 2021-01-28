# Javascript

Javascript makes web pages interative. Example are:
- Slideshows
- Forms
- Partial page reloads
- Filtering data

## Script

A script is a series of instructions for the computer, akin to:
- a recipe
- a handbook 
- a manual

The goal needs to be defined first.
- Tasks must be defined, then broken down into series of steps.
- remember a computer only understands commands it already knows (delete, add, open, etc), and yes/no binary questions.

## Parts of a Script

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

## Functions

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