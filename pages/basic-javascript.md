# Contents

<details>
<summary> Introduction to JavaScript </summary>

-   [What is JavaScript?](#what-is-javascript)
-   [Why JavaScript in Data Structures and Algorithms?](#why-javascript-in-data-structures-and-algorithms)
-   [What is Data Structures and Algorithms?](#what-is-data-structures-and-algorithms)
</details>

<details>
<summary> JavaScript Basics</summary>

-   [Variables](#variables)
-   [Data Types](#data-types)
-   [Operators](#operators)
-   [Strings](#strings)
-   [Arrays](#arrays)
-   [Objects](#objects)
-   [Functions](#functions)
-   [Conditionals](#conditionals)
-   [Loops](#loops)
-   [Scope](#scope)

</details>

<details>
<summary> Arrays and Objects</summary>

-   [Arrays and Objects](#arrays-and-objects)

</details>

## INTRODUCTION to JavaScript

### What is JavaScript?

JavaScript is a programming language that is used to make web pages interactive. It is a lightweight, interpreted programming language with first-class functions, most known as the scripting language for Web pages, but it's used in many non-browser environments as well. JavaScript is a prototype-based, multi-paradigm, single-threaded, dynamic language, supporting object-oriented, imperative, and declarative (e.g. functional programming) styles.

### Why JavaScript in Data Structures and Algorithms?

JavaScript is a very popular programming language. It is used in web development, mobile development, desktop development, game development, and many other areas. So learn one language and you can use it in many different areas so you don't have to learn different language to separately learn DSA. It is also the only programming language that is supported by all major browsers. This makes it a very useful language to learn. It is also a very powerful language. It is a multi-paradigm language, which means that it supports object-oriented programming, functional programming, and imperative programming. It also supports functional programming, which makes it a very powerful language.

### What is Data Structures and Algorithms?

Data Structures and Algorithms are the building blocks of computer science. They are the foundation of all computer programs.

## JavaScript Basics

### Variables

Variables are used to store data values. In JavaScript, there are three types of variables:

-   `var` - This is the old way of declaring variables. It is still used in some cases, but it is not recommended to use it.
-   `let` - This is the new way of declaring variables. It is the recommended way to declare variables.
-   `const` - This is the new way of declaring variables. It is the recommended way to declare variables. It is used to declare variables that are not going to change.

```js
var x = 5;
let y = 10;
const z = 15;
```

### Data Types

JavaScript has dynamic typing, which means that the same variable can be used to store different data types. There are seven data types in JavaScript:

-   `Number` - This is used to store numbers.
-   `String` - This is used to store text.
-   `Boolean` - This is used to store `true` or `false`.
-   `Null` - This is used to store nothing.
-   `Undefined` - This is used to store nothing.
-   `Symbol` - This is used to store unique values.
-   `Object` - This is used to store collections of data.

```js
var x = 5; // Number
var y = "Hello"; // String
var z = true; // Boolean
var a = null; // Null
var b = undefined; // Undefined
var c = Symbol("Hello"); // Symbol
var d = { name: "John", age: 30 }; // Object
```

### Operators

JavaScript has the following types of operators:

-   `Arithmetic` - This is used to perform arithmetic operations.
-   `Assignment` - This is used to assign values to variables.
-   `Comparison` - This is used to compare values.
-   `Logical` - This is used to combine conditional statements.
-   `String` - This is used to concatenate strings.
-   `Ternary` - This is used to assign a value to a variable based on a condition.

```js
// Arithmetic
var x = 5;
var y = 10;
var z = x + y; // 15 (Addition)
// and many more... (Subtraction, Multiplication, Division, Modulus, Exponentiation)

// Assignment
var x = 5;
x += 10; // 15 (Addition)
// and many more... (Subtraction, Multiplication, Division, Modulus, Exponentiation)

// Comparison
var x = 5;
var y = 10;
var z = x == y; // false (Equal to)
// and many more... (Not equal to, Greater than, Greater than or equal to, Less than, Less than or equal to)

// Logical
var x = 5;
var y = 10;
var z = x < 10 && y > 10; // true (And)
// and many more... (Or, Not)

// String
var x = "Hello";
var y = "World";
var z = x + y; // "Hello World" (Concatenation)

// Ternary
var x = 5;
var y = 10;
var z = x > y ? "x is greater than y" : "x is less than or equal to y"; // "x is less than or equal to y"
```

### Strings

Strings are used to store text. Strings are created by enclosing text in quotes. There are three types of quotes:

-   `"` - Double quotes.
-   `'` - Single quotes.
-   `` ` `` - Backticks.

```js
var x = "Hello"; // Double quotes
var y = "Hello"; // Single quotes
var z = `Hello`; // Backticks
```

### Arrays

Arrays are used to store multiple values in a single variable. Arrays are created by enclosing values in square brackets.

```js
var x = [1, 2, 3, 4, 5]; // Array of numbers
var y = ["Hello", "World"]; // Array of strings
var z = [true, false]; // Array of booleans
var a = [1, "Hello", true]; // Array of different data types
```

### Objects

Objects are used to store collections of data. Objects are created by enclosing values in curly brackets.

```js
var x = { name: "John", age: 30 }; // Object
```

### Functions

Functions are used to perform a task. Functions are created by using the `function` keyword.

```js
function myFunction() {
    console.log("Hello World");
}
```

### Conditionals

Conditionals are used to perform different actions based on different conditions. JavaScript has the following types of conditionals:

-   `if` - This is used to perform a task if a condition is true.
-   `if...else` - This is used to perform a task if a condition is true, and a different task if the condition is false.
-   `if...else if...else` - This is used to perform a task if a condition is true, and a different task if another condition is true, and a different task if none of the conditions are true.
-   `switch` - This is used to perform different actions based on different conditions.

```js
// if
var x = 5;
if (x > 10) {
    console.log("x is greater than 10");
}

// if...else
var x = 5;
if (x > 10) {
    console.log("x is greater than 10");
} else {
    console.log("x is less than or equal to 10");
}

// if...else if...else
var x = 5;
if (x > 10) {
    console.log("x is greater than 10");
} else if (x > 5) {
    console.log("x is greater than 5");
} else {
    console.log("x is less than or equal to 5");
}

// switch
var x = 5;
switch (x) {
    case 1:
        console.log("x is 1");
        break;
    case 2:
        console.log("x is 2");
        break;
    case 3:
        console.log("x is 3");
        break;
    default:
        console.log("x is not 1, 2, or 3");
}
```

### Loops

Loops are used to perform a task multiple times. JavaScript has the following types of loops:

-   `for` - This is used to perform a task a specified number of times.
-   `while` - This is used to perform a task while a condition is true.
-   `do...while` - This is used to perform a task while a condition is true.

```js
// for
for (var i = 0; i < 10; i++) {
    console.log(i);
}

// while
var i = 0;
while (i < 10) {
    console.log(i);
    i++;
}

// do...while
var i = 0;
do {
    console.log(i);
    i++;
} while (i < 10);
```

### Scope

Scope is used to define where variables can be accessed or referenced. JavaScript has the following types of scope:

-   `Global` - This is used to define a variable that can be accessed by all functions.
-   `Local` - This is used to define a variable that can only be accessed by the function it is defined in.

```js
// Global
var x = 5;

function myFunction() {
    console.log(x);
}

myFunction(); // 5

// Local
function myFunction() {
    var x = 5;
    console.log(x);
}

myFunction(); // 5
```

## JavaScript Arrays and Objects

### Arrays and Objects

Arrays are used to store multiple values in a single variable. Arrays are created by enclosing values in square brackets. Read more about arrays and objects in [here](./arrays-and-objects.md).
