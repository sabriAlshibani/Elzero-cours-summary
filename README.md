# javascript course summary

## table of Contents

- [javascript course summary](#javascript-course-summary)
  - [table of Contents](#table-of-contents)
  - [1- work with chrome develope tools](#1--work-with-chrome-develope-tools)
  - [2- where to put the code](#2--where-to-put-the-code)
  - [3- comments](#3--comments)
  - [4- Data types \& typeOf operator](#4--data-types--typeof-operator)
    - [output](#output)
    - [output](#output-1)
    - [output](#output-2)
    - [output](#output-3)
    - [output](#output-4)
  - [Variables](#variables)
  - [compare between var, let, and const](#compare-between-var-let-and-const)
    - [var](#var)
    - [let](#let)
    - [const](#const)
  - [concatenation strings](#concatenation-strings)
    - [templates literals and template strings](#templates-literals-and-template-strings)
      - [ecma script and \`\`](#ecma-script-and-)
  - [arithmetic operator](#arithmetic-operator)
  - [unary operator](#unary-operator)
    - [plus operator`(+)`](#plus-operator)
      - [output](#output-5)
    - [negative operator `(-)`](#negative-operator--)
      - [output](#output-6)
  - [Number](#number)
    - [Number methods](#number-methods)

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
### output
```
string
```

2- **number**

```javascript
console.log(typeof 5000);
```
### output
```
number
```

3- **boolean**

```javascript
console.log(typeof true);
console.log(typeof false);
```
### output
```
boolean
boolean
```

4- **object**

```javascript
console.log(typeof ["Ali", "Mohammed", "Osama"]); // this is called "array" but its kind from object
console.log(typeof null); // if the variable is empty it called null
console.log(typeof { name: "Sabri", age: 17, country: "Yemen" }); // this is called object and its kind from object
```
### output
```
object
object
object
```

5- **undefined**

```javascript
console.log(typeof undefined);
```
### output
```
undefined
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
```
Sabri
```

if we use the variable before declare it it will be undefined like this code
```javascript 
console.log(user);
var user = "Sabri";
```
```
undefined
```

## compare between var, let, and const

### var 
we can redeclare it and if we use it before we declare the value will be undefined 
```javascript 
var age = 1; // here we redeclare it the value in it will be "2"
var age = 2;
console.log(age);

console.log(user);
var user = "Sabri";
```
```
2

undefined
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
- an example 
  ```javascript
  //here are some variables in one line
  let title = " learning js",
   description = " we learning js from Elzero web school", 
   date = "2023/ 11/ 23";
  // we created HTML in a variable
  let card = `
  <div class="card">
  <h3 class="title"> ${title} </h3>
  <p class="title"> ${description} </p>
  <span class="title"> ${date} </span>
  `
  // now we writing "HTML" in JS 
  document.write(card); // it will apear on the page  
  ```

  ## arithmetic operator 
| operator | description  | the job |
|:--------:|----------|----------|
|  +       | addition |  it adds tow numbers or strings or variables or more together |
|   -      | subtraction |  it subtracts the numbers we cant just  |
|   *      | multiplication |  it  multiplies numbers  |
|   **      | Exponentiation |  it  multiplies numbers  |
|   /      |  	Division |  it divides numbers  |
|   %      |  	Modulus (Remainder) |  it returns the division remainder  |
|   ++     |    Increment |  it increments numbers |
|  --     |  	decrement |  it decrements numbers  |

## unary operator
### plus operator`(+)` 
  
  it convert the number into the string to number
  if we use it ito the string it will be NAN 



  ```javascript
  let str1 = "12"; 
//using unary plus to covert  string to number
let num = +str1; 
console.log(num); 

// Here we are using typeof operator 
console.log(typeof (num)) 

// "Geeks" cannot be converted to a number 
let str2 = +"Geeks"; 
console.log(str2);

  ```
  #### output
  ```
  12 

number

NAN
  ```

  ### negative operator `(-)` 
  it covert string to number also, but when we use it with string witch not a number
  the result will be NAN 

```javascript
  let str1 = "12"; 
//using unary plus to covert  string to number
let num = -str1; 
console.log(num); 

// Here we are using typeof operator 
console.log(typeof (num)) 

// "Geeks" cannot be converted to a number 
let str2 = -"Geeks"; 
console.log(str2);

  ```

  #### output
  ```
  -12 

number

NAN
  ```

## Number 
here are different methods to type number 

```javascript 
console.log(1000000);
console.log(1000-000); 
console.log(10e6); // type after " e " how many zeros do want to it be 
console.log(10 ** 6);
console.log(10 * 10 * 10 * 10 * 10 * 10);
// all those methods get the same result or value 

```

### Number methods
we have some methods of Number methods 

```javascript 
console.log( (100).toString()); // it convert number to string put the number into () or type two (.) after number like way below if the number with out Fractions

console.log( 100.55555.toFixed());  // it fixes the number from Fractions just type how many numbers do you want be after the main number 

console.log(Number("100")); // convert string to number 
// but if we type  (100 Ahmed) what will happen ?
console.log(Number("100 Ahmed")); // the result will be NAN 
// and also using unary operator 

```











