# javascript course summary

## table of Contents

- [javascript course summary](#javascript-course-summary)
  - [table of Contents](#table-of-contents)
  - [1- work with chrome develope tools](#1--work-with-chrome-develope-tools)
  - [2- where to put the code](#2--where-to-put-the-code)
  - [3- comments](#3--comments)
  - [4- Data types \& typeOf operator](#4--data-types--typeof-operator)
  - [Variables](#variables)
  - [compare between var, let, and const](#compare-between-var-let-and-const)
    - [var](#var)
    - [let](#let)
    - [const](#const)
  - [concatenation strings](#concatenation-strings)
    - [templates literals and template strings](#templates-literals-and-template-strings)
      - [ecma script and \`\`](#ecma-script-and-)

## 1- work with chrome develope tools

we can write js code in console any things we can write it in js also we can write it in console

there are some ways for that. when we want to some warnings or message

```javascript
console.log("write any things"); // it will appear in console
console.wrong("write any wrongs"); // it will appear in console with red color and false
```

we can create items in console and we can select them then we change them by change their color or size like these examples

```javascript
document.write(<h1> learning JS</h1>);
document.querySelector("h1").style.color = "red";
```

## 2- where to put the code

we have to put the script tag in the ending of the page because JS order read the lines line by line

```HTML
<body>
    <h1> learning JS </h1>
<script src="main.js"> </script>
</body>
```

when the code be after the script tag that means it is unavailable

```HTML
<head>
    <script src="main.js"></script>
    </head>
<body>
    <h1> learning JS </h1>
</body>
```

## 3- comments

by comments we can write notes about codes or use them to prevent the codes from running
there are two types of comments

1- single line comment

```javascript
// write comments on the same line
```

2- most line comments

```javascript
/* 
1- here we can write a lot of points
2- make lists 
3- explain or write information
 */
```

## 4- Data types & typeOf operator

1- **strings**

```javascript
console.log(typeof "learning JS");
```

2- **number**

```javascript
console.log(typeof 5000);
```

3- **boolean**

```javascript
console.log(typeof true);
console.log(typeof false);
```

4- **object**

```javascript
console.log(typeof ["Ali", "Mohammed", "Osama"]); // this is called "array" but its kind from object
console.log(typeof null); // if the variable is empty it called null
console.log(typeof { name: "Sabri", age: 17, country: "Yemen" }); // this is called object and its kind from object
```

5- **undefined**

```javascript
console.log(typeof undefined);
```

## Variables

- what is the variable?

  Variables are containers for storing information

- why do we use the variables in JS ?

  to store and manage data within a program. They act as containers that hold different types of information

- how to we write the variables ?
  like this ways
```javascript 
var user = "Sabri";
console.log(user);
```
if we use the variable before declare it it will be undefined like this code
```javascript 
console.log(user);
var user = "Sabri";
```

## compare between var, let, and const

### var 
we can redeclare it and if we use it before we declare the value will be undefined 
```javascript 
var age = 1; // here we redeclare it the value in it will be "2"
var age = 2;

console.log(user);
var user = "Sabri";
```
### let 
we can not redeclare it and if we use it before we declare there is wrong
```javascript 
var age = 1; // here we can not redeclare if we do that it will be a wrong
var age = 2;

console.log(user);
var user = "Sabri";
```
### const
we can not redeclare it and if we use it before we declare there is wrong
```javascript 
var age = 1; // here we can not redeclare if we do that it will be a wrong
var age = 2;

console.log(user);
var user = "Sabri";
```
finally when we create var we can find it in the window
but let and const can not be there.

## concatenation strings 
here we have some example
```javascript
let firstName = "Mohammed";
let lastName = "Ali"
console.log(firstName + lastName); // we contact both by this way 
// if we want to make a gap between them use this 
console.log(firstName + " " lastName); // here it will be a gap
console.log(firstName,lastName); // this day it considers them to messages then it prints them beside each others it means there is a automatic gap.
```
### templates literals and template strings
when we want to make gaps between the variables we use this ways 
```javascript 
console.log(a + " " + b + " " + c)
```
and if we have any strings an we want make on of them under of them we use "`\n`"
```javascript 
console.log(a + " " + b + "/n" + c);  // a it will be under them
```
#### ecma script and ``
 but ecma scrip make it easy without `/n` and without `" "` we can male gaps by this ways
 put the variables between `` then use put the variable into `{}` with $
```javascript 
console.log(`${a} ${b} ${c}`); // we do not need to use the last methods
// we can write any things between them and if we want make them in two more we can 
console.log(`${a} hello ${b} 
 ${c}`); // just by click enter 
```
- example 
  ```javascript
  // write some variables
  let title 
  ```