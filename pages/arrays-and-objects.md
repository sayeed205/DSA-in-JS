# Arrays and Objects

## Contents

<details>
<summary>Arrays</summary>

-   [Creating Arrays](#creating-arrays)
-   [Accessing Array Elements](#accessing-array-elements)
-   [Changing Array Elements](#changing-array-elements)
-   [Array Length](#array-length)
-   [Looping Array Elements](#looping-array-elements)
-   [Adding Array Elements](#adding-array-elements)
-   [Removing Array Elements](#removing-array-elements)

</details>

<details>
<summary>Objects</summary>

-   [Creating Objects](#creating-objects)
-   [Accessing Object Properties](#accessing-object-properties)
-   [Changing Object Properties](#changing-object-properties)
-   [Object Methods](#object-methods)
-   [Looping Object Properties](#looping-object-properties)
-   [Adding Object Properties](#adding-object-properties)
-   [Removing Object Properties](#removing-object-properties)

</details>

<details>
<summary>Array Methods</summary>

-   [concat()](#concat)
-   [copyWithin()](#copywithin)
-   [entries()](#entries)
-   [every()](#every)
-   [fill()](#fill)
-   [filter()](#filter)
-   [find()](#find)
-   [findIndex()](#findindex)
-   [forEach()](#foreach)
-   [from()](#from)
-   [includes()](#includes)
-   [indexOf()](#indexof)
-   [isArray()](#isarray)
-   [join()](#join)
-   [keys()](#keys)
-   [lastIndexOf()](#lastindexof)
-   [map()](#map)
-   [pop()](#pop)
-   [push()](#push)
-   [reduce()](#reduce)
-   [reduceRight()](#reduceright)
-   [reverse()](#reverse)
-   [shift()](#shift)
-   [slice()](#slice)
-   [some()](#some)
-   [sort()](#sort)
-   [splice()](#splice)
-   [toString()](#tostring)
-   [unshift()](#unshift)

</details>

<details>
<summary>Object Methods</summary>

-   [assign()](#assign)
-   [create()](#create)
-   [entries()](#entries-1)
-   [freeze()](#freeze)
-   [is()](#is)
-   [isExtensible()](#isextensible)
-   [isFrozen()](#isfrozen)
-   [isSealed()](#issealed)
-   [keys()](#keys-1)
-   [seal()](#seal)
-   [values()](#values-1)

</details>

<details>
<summary>Array Properties</summary>

-   [Array.length](#arraylength)

</details>

<details>
<summary>Looping through and Objects</summary>

-   [for...in](#forin)
-   [Object.keys()](#objectkeys)
-   [Object.values()](#objectvalues)
-   [Object.entries()](#objectentries)

</details>

### Arrays

Arrays are used to store multiple values in a single variable. Arrays are created by enclosing values in square brackets.

```js
var x = [1, 2, 3, 4, 5]; // Array of numbers
var y = ["Hello", "World"]; // Array of strings
var z = [true, false]; // Array of booleans
var a = [1, "Hello", true]; // Array of different data types
```

#### Creating Arrays

Arrays can be created using the `Array` constructor.

```js
var x = new Array(1, 2, 3, 4, 5);
console.log(x); // [1, 2, 3, 4, 5]
```

#### Accessing Array Elements

Array elements can be accessed by referring to the index number.

```js
var x = [1, 2, 3, 4, 5];
console.log(x[0]); // 1
console.log(x[1]); // 2

var y = ["Hello", "World"];
console.log(y[0]); // "Hello"

var z = [true, false];
console.log(z[0]); // true
```

#### Changing Array Elements

Array elements can be changed by referring to the index number.

```js
var x = [1, 2, 3, 4, 5];
x[0] = 10;
console.log(x[0]); // 10
```

#### Array Length

The length property returns the number of elements in an array.

```js
var x = [1, 2, 3, 4, 5];
console.log(x.length); // 5
```

#### Looping Array Elements

Array elements can be looped through using the `for` loop.

```js
var x = [1, 2, 3, 4, 5];
for (var i = 0; i < x.length; i++) {
    console.log(x[i]);
}
```

#### Adding Array Elements

Array elements can be added using the `push` method.

```js
var x = [1, 2, 3, 4, 5];
x.push(6);
console.log(x); // [1, 2, 3, 4, 5, 6]
```

#### Removing Array Elements

Array elements can be removed using the `pop` method.

```js
var x = [1, 2, 3, 4, 5];
x.pop();
console.log(x); // [1, 2, 3, 4]
```

### Objects

Objects are used to store collections of data. Objects are created by enclosing values in curly brackets.

```js
var x = { name: "John", age: 30 }; // Object
```

#### Creating Objects

Objects can be created using the `Object` constructor.

```js
var x = new Object();
x.name = "John";
x.age = 30;
console.log(x); // { name: "John", age: 30 }
```

#### Accessing Object Properties

Object properties can be accessed by referring to the property name.

```js
var x = { name: "John", age: 30 };
console.log(x.name); // "John"
console.log(x.age); // 30
```

#### Changing Object Properties

Object properties can be changed by referring to the property name.

```js
var x = { name: "John", age: 30 };
x.name = "Jane";
console.log(x.name); // "Jane"
```

#### Looping Object Properties

Object properties can be looped through using the `for...in` loop.

```js
var x = { name: "John", age: 30 };
for (var key in x) {
    console.log(x[key]);
}
```

#### Adding Object Properties

Object properties can be added using the `newProperty` method.

```js
var x = { name: "John", age: 30 };
x.email = "john@doe.com";
console.log(x); // { name: "John", age: 30, email: "john@doe.com" }
```

#### Removing Object Properties

Object properties can be removed using the `delete` keyword.

```js
var x = { name: "John", age: 30 };
delete x.age;
console.log(x); // { name: "John" }
```

### Array Methods

-   #### `concat()`

    The `concat()` method is used to join two or more arrays.

        ```js
        var x = [1, 2, 3];
        var y = [4, 5, 6];
        var z = x.concat(y);
        console.log(z); // [1, 2, 3, 4, 5, 6]
        ```

-   #### `copyWithin()`

    The `copyWithin()` method is used to copy array elements within the array.

        ```js
        var x = [1, 2, 3, 4, 5];
        x.copyWithin(0, 3);
        console.log(x); // [4, 5, 3, 4, 5]
        ```

-   #### `entries()`

    The `entries()` method is used to return a key/value pair Array Iteration Object.

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.entries();
        console.log(y.next().value); // [0, 1]
        console.log(y.next().value); // [1, 2]
        console.log(y.next().value); // [2, 3]
        ```

-   #### `every()`

    The `every()` method is used to check if all array values pass a test.

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.every(function (value) {
            return value > 0;
        });
        console.log(y); // true
        ```

-   #### `fill()`

    The `fill()` method is used to fill the elements in an array with a static value.

        ```js
        var x = [1, 2, 3, 4, 5];
        x.fill(0);
        console.log(x); // [0, 0, 0, 0, 0]
        ```

-   #### `filter()`

    The `filter()` method is used to create a new array with array elements that passes a test.

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.filter(function (value) {
            return value > 3;
        });
        console.log(y); // [4, 5]
        ```

-   #### `find()`

    The `find()` method is used to return the value of the first array element that passes a test.

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.find(function (value) {
            return value > 3;
        });
        console.log(y); // 4
        ```

-   #### `findIndex()`

    The `findIndex()` method is used to return the index of the first array element that passes a test.

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.findIndex(function (value) {
            return value > 3;
        });
        console.log(y); // 3
        ```

-   #### `forEach()`

    The `forEach()` method is used to call a function for each array element.

        ```js
        var x = [1, 2, 3, 4, 5];
        x.forEach(function (value) {
            console.log(value);
        });
        ```

-   #### `from()`

    The `from()` method is used to create an array from an object or string.

        ```js
        var x = Array.from("John");
        console.log(x); // ["J", "o", "h", "n"]
        ```

-   #### `includes()`

    The `includes()` method is used to check if an array contains the specified element.

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.includes(3);
        console.log(y); // true
        ```

-   #### `indexOf()`

    The `indexOf()` method is used to search the array for an element and returns its position.

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.indexOf(3);
        console.log(y); // 2
        ```

-   #### `isArray()`

    The `isArray()` method is used to check whether an object is an array.

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = Array.isArray(x);
        console.log(y); // true
        ```

-   #### `join()`

    The `join()` method is used to join all elements of an array into a string.

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.join("-");
        console.log(y); // "1-2-3-4-5"
        ```

-   #### `keys()`

    The `keys()` method is used to return a Array Iteration Object, containing the keys of the original array.

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.keys();
        console.log(y.next().value); // 0
        console.log(y.next().value); // 1
        console.log(y.next().value); // 2
        ```

-   #### `lastIndexOf()`

    The `lastIndexOf()` method is used to search the array for an element, starting at the end, and returns its position.

        ```js
        var x = [1, 2, 3, 4, 5, 3];
        var y = x.lastIndexOf(3);
        console.log(y); // 5
        ```

-   #### `map()`

    The `map()` method is used to create a new array with the result of calling a function for each array element.

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.map(function (value) {
            return value * 2;
        });
        console.log(y); // [2, 4, 6, 8, 10]
        ```

-   #### `pop()`

    The `pop()` method is used to remove the last element of an array, and returns that element.

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.pop();
        console.log(y); // 5
        console.log(x); // [1, 2, 3, 4]
        ```

-   #### `push()`

    The `push()` method is used to add new elements to the end of an array, and returns the new length.

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.push(6);
        console.log(y); // 6
        console.log(x); // [1, 2, 3, 4, 5, 6]
        ```

-   #### `reduce()`

    The `reduce()` method is used to reduce the values of an array to a single value (going left-to-right).

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.reduce(function (total, value) {
            return total + value;
        });
        console.log(y); // 15
        ```

-   #### `reduceRight()`

    The `reduceRight()` method is used to reduce the values of an array to a single value (going right-to-left).

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.reduceRight(function (total, value) {
            return total + value;
        });
        console.log(y); // 15
        ```

-   #### `reverse()`

    The `reverse()` method is used to reverse the elements in an array.

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.reverse();
        console.log(y); // [5, 4, 3, 2, 1]
        ```

-   #### `shift()`

    The `shift()` method is used to remove the first element of an array, and returns that element.

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.shift();
        console.log(y); // 1
        console.log(x); // [2, 3, 4, 5]
        ```

-   #### `slice()`

    The `slice()` method is used to select a part of an array, and returns the new array.

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.slice(2, 4);
        console.log(y); // [3, 4]
        ```

-   #### `some()`

    The `some()` method is used to check if any of the array elements pass a test.

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.some(function (value) {
            return value > 3;
        });
        console.log(y); // true
        ```

-   #### `sort()`

    The `sort()` method is used to sort the elements of an array.

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.sort(function (a, b) {
            return b - a;
        });
        console.log(y); // [5, 4, 3, 2, 1]
        ```

-   #### `splice()`

    The `splice()` method is used to add/remove items to/from an array, and returns the removed item(s).

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.splice(2, 0, 6, 7);
        console.log(y); // []
        console.log(x); // [1, 2, 6, 7, 3, 4, 5]
        ```

-   #### `toString()`

    The `toString()` method is used to convert an array to a string of (comma separated) array values.

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.toString();
        console.log(y); // "1,2,3,4,5"
        ```

-   #### `unshift()`

    The `unshift()` method is used to add new elements to the beginning of an array, and returns the new length.

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.unshift(6);
        console.log(y); // 6
        console.log(x); // [6, 1, 2, 3, 4, 5]
        ```

### Array Properties

-   #### `arraylength`

    The `length` property sets or returns the number of elements in an array.

        ```js
        var x = [1, 2, 3, 4, 5];
        var y = x.length;
        console.log(y); // 5
        ```

### Looping through Objects

-   #### `for...in`

    The `for...in` loop loops through the properties of an object.

        ```js
        var x = { a: 1, b: 2, c: 3 };
        for (var y in x) {
            console.log(y); // a, b, c
        }
        ```

-   #### `Object.keys()`

    The `Object.keys()` method returns an array of a given object's own enumerable properties.

        ```js
        var x = { a: 1, b: 2, c: 3 };
        var y = Object.keys(x);
        console.log(y); // ["a", "b", "c"]
        ```

-   #### `Object.values()`

    The `Object.values()` method returns an array of a given object's own enumerable property values.

        ```js
        var x = { a: 1, b: 2, c: 3 };
        var y = Object.values(x);
        console.log(y); // [1, 2, 3]
        ```

-   #### `Object.entries()`

    The `Object.entries()` method returns an array of a given object's own enumerable string-keyed property [key, value] pairs.

        ```js
        var x = { a: 1, b: 2, c: 3 };
        var y = Object.entries(x);
        console.log(y); // [["a", 1], ["b", 2], ["c", 3]]
        ```

<!-- Here ends the content of basic-javascript.md -->
