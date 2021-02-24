# Javascript

 ### Use of comments  
* For one line comment - ** `//this is a comment` **
* For multiple ines - ** `/* this is multi line comment */` **

### Datatypes
* the different data types are: 
     * number
     * bigint
     * boolean
     * String
     * null
     * undefined
     * symbol
     * object
 * Variables are declared using `var`, `let`,`const`.
 
 ### Assignment operator
 * `=` is used to assign a value to variable
 * ```js
   let myName = 'Shreyasi';
   ```
 ### Assigning one variable to another
 * ```js
   var a;
   a = 7;
   var b;
   b=a;
   ```
### Unintialized variables
* When JavaScript variables are declared, they have an initial value of `undefined`. If you do a mathematical operation on an undefined variable your result will be `NaN` which means "Not a Number"

### Case sensitivity of variables
* Javascript variables follow `camel case`
* ` myVar, inMyCity , iDontGiveAFuck;`

### Adding numbers
* `let a = 10+ 20;`

### Subtracting numbers
* ` let a = 20-10;`

### Multiplying numbers
* `let a = 8*8; `

### Dividing numbers
* `let a = 18/2 ;`

### Incrementing number
* `i++` i.e `i=i+1`

### Decrementing number
* `i--` i.e `i=i-1`

### Storing decimals
* decimal numbers can also be stored in variabbles
* `let a = 6.8; `
* `let b = 2.0 * 2.5 //5.0`
* `let c = 4.4 / 2.0 //2.2`

### Finding Remainder
* `let a = 5%2 //1`
* `let b = Math.floor(5 / 2) //2 is the quotient

### Compound assignment with augmented addition
* myVar = myVar + 5;
can be written as
` myVar+=5`

### Compound assignment with augmented subtraction
* myVar = myVar - 3;
can be written as
`myVar -= 3`

### Compound assignment with augmented multiplication
* myVar = myVar * 6;
can be written as
` myVar*=6`

### Compound assignment with augmented didvision
* myVar =  myVar / 8;
can be written as 
`myVar/= 8;`

### Declaring string variables
* `let myName = "Shreyasi Patil";`

### Escaping literal quotes in string
* use of " and ' in string - if using same " in two places - 
```js
var string = "Alan said \"Petter is learning javascript"\.";
```

### Quoting Strings with Single Quotes Passed
* `let stringOfMyOwn = 'Jake asks Finn "Hey, let\'s go on a adventure?"'`

### Escape sequences in string
* \'	single quote
*  \"	double quote
*  \\	backslash
*  \n	newline
*  \r	carriage return
*  \t	tab
*  \b	word boundary
*  \f	form feed

### Concatinate strings with Plus Operator
```js
let myString = "My name is "+ "Shreyasi Patil";
```

### Concatenating Strings with the Plus Equals Operator
```js
let ourString = "I come first.";
ourString += "I come last."; //I come first.I come last.
```

### Constructing strings using variables
```js
var ourName = "freeCodeCamp";
var ourStr = "Hello, our name is " + ourName + ", how are you?";
// ourStr is now "Hello, our name is freeCodeCamp, how are you?"
```
### Find length of String
* `.length` is used.
* `let string = "length"`
*  `string.length // 6`

### Use Bracket Notation to Find the First Character in a String
* Bracket notation is a way to get a character at a specific index within a string
* 
```js
    var firstName = "Charles";
    var firstLetter = firstName[0]; // firstLetter is "C"
 ```
### Understand String Immutability Passed
* ***In JavaScript, String values are immutable, which means that they cannot be altered once created.***

### Finding last character of string
* 
```js
let firstName = "Shreyasi";
let lastCharacter = firstName[firstName.length - 1];
```
### Javascript Arrays
* 
```js
   var sandwich = ["peanut butter", "jelly", "bread"]
   ```
   
### Multidimensional Array(nesting arrays)
*
```js
[["Bulls", 23], ["White Sox", 45]]
```
### Access array data with index
* 
```js
var array = [50,60,70];
array[0]; // equals 50
var data = array[1];  // equals 60
```
### Modify Array data with index
*
```js
var ourArray = [50,40,30];
ourArray[0] = 15; // equals [15,40,30]
```
### Access Multi-Dimensional Arrays With Indexes Passed
* 
```js
var arr = [
  [1,2,3],
  [4,5,6],
  [7,8,9],
  [[10,11,12], 13, 14]
];
arr[3]; // equals [[10,11,12], 13, 14]
arr[3][0]; // equals [10,11,12]
arr[3][0][1]; // equals 11
```
### Manipulate Arrays with push()
* An easy way to append data to the end of an array is via the `push()` function.

* `push()` takes one or more parameters and "pushes" them onto the end of the array.
* 
```js
var arr1 = [1,2,3];
arr1.push(4);
// arr1 is now [1,2,3,4]

var arr2 = ["Stimpson", "J", "cat"];
arr2.push(["happy", "joy"]);
// arr2 now equals ["Stimpson", "J", "cat", ["happy", "joy"]]
```
### Manipulate Arrays with pop()
* `pop()` is used to "pop" a value off of the end of an array. We can store this "popped off" value by assigning it to a variable. 
* In other words, `pop()` removes the last element from an array and returns that element.
* 
```js
var threeArr = [1, 4, 6];
var oneDown = threeArr.pop();
console.log(oneDown); // Returns 6
console.log(threeArr); // Returns [1, 4]
```
### Manipulate Arrays with shift()
* That's where `shift()` comes in. It works just like .pop(), except it **removes the first element instead of the last**
* 
```js
var ourArray = ["Stimpson", "J", ["cat"]];
var removedFromOurArray = ourArray.shift();
// removedFromOurArray now equals "Stimpson" and ourArray now equals ["J", ["cat"]].

Use the .shift() function to remove the first item from myArray, assigning the "shifted off" value to removedFromMyArray.

myArray should now equal [["dog", 3]].

removedFromMyArray should contain ["John", 23].
```
### Manipulate Arrays with unshift()
* Not only can you `shift` elements off of the beginning of an array, you can also `unshift` elements to the beginning of an array i.e. add elements in front of the array.

* `unshift()` works exactly like `.push()`, but instead of adding the element at the end of the array, `unshift()` adds the element at the beginning of the array.
*
```js
var ourArray = ["Stimpson", "J", "cat"];
ourArray.shift(); // ourArray now equals ["J", "cat"]
ourArray.unshift("Happy");
// ourArray now equals ["Happy", "J", "cat"]
```
### Javascript Functions
*
```js
function functionName() {
  console.log("Hello World");
}
```
### Passing values to functions using parameter
*
```js
function testFun(param1, param2) {
  console.log(param1, param2);
}
```
### Global Scope and Functions
* In JavaScript, scope refers to the visibility of variables. Variables which are defined outside of a function block have Global scope. This means, they can be seen everywhere in your JavaScript code.

### Local Scope and Functions Passed
*
```js
function myTest() {
  var loc = "foo";
  console.log(loc);
  * A function can include the return statement but it does not have to. In the case that the function doesn't have a return statement, when you call it, the function processes the inner code but the returned value is undefined
}
myTest(); // logs "foo"
console.log(loc); // loc is not defined
```
### Return a Value from a Function with Return Passed
```js
function plusThree(num) {
  return num + 3;
}
var answer = plusThree(5); // 8
```
### Understanding Undefined Value returned from a Function
* A function can include the `return` statement but it does not have to. 
* In the case that the function doesn't have a `return` statement, when you call it, the function processes the inner code but the returned value is `undefined`
```js
var sum = 0;
function addSum(num) {
  sum = sum + num;
}
addSum(3); // sum will be modified but returned value is undefined
```

### Queue
* In Computer Science a queue is an abstract Data Structure where items are kept in order.
*  New items can be added at the back of the queue and old items are taken off from the front of the queue.

### Boolean
* Booleans may only be one of two values: true or false.
*  They are basically little on-off switches, where true is "on" and false is "off." These two states are mutually exclusive

### Comparison with the Equality OperatorPassed
* The most basic operator is the equality operator ==.
*  The equality operator compares two values and returns true if they're equivalent or false if they are not.

### Comparison with the Strict Equality Operator
* Strict equality (===) is the counterpart to the equality operator (==).
*  However, unlike the equality operator, which attempts to convert both values being compared to a common type, the strict equality operator does not perform a `type` conversion.
```js
3 ===  3   // true
3 === '3'  // false
```
### typeof operator
```js
typeof 3   // returns 'number'
typeof '3' // returns 'string'
```
### Comparison with the Inequality Operator Passed
```js
1 !=  2     // true
1 != "1"    // false
1 != '1'    // false
1 != true   // false
0 != false  // false
```
### Comparison with the Strict Inequality Operator Passed
```js
3 !==  3   // false
3 !== '3'  // true
4 !==  3   // true
```
### Comparison with the Greater Than Operator Passed
```js
5   >  3   // true
7   > '3'  // true
2   >  3   // false
'1' >  9   // false
```
### Comparison with the Greater Than Or Equal To Operator
```js
6   >=  6   // true
7   >= '3'  // true
2   >=  3   // false
'7' >=  9   // false
```
### Comparison with the Less Than Operator Passed
```js
2   < 5  // true
'3' < 7  // true
5   < 5  // false
3   < 2  // false
'8' < 4  // false
```
### Comparison with the Less Than Or Equal To Operator Passed
```js
4   <= 5  // true
'7' <= 7  // true
5   <= 5  // true
3   <= 2  // false
'8' <= 4  // false
```
### Comparisons with the Logical And Operator Passed
```js
if (num > 5) {
  if (num < 10) {
    return "Yes";
  }
}
return "No";
```
is equivalent to 
```js
if (num > 5 && num < 10) {
  return "Yes";
}
return "No";
```
### Comparisons with the Logical Or Operator
```js
if (num > 10) {
  return "No";
}
if (num < 5) {
  return "No";
}
return "Yes";
```
is equivalent of
```js
if (num > 10 || num < 5) {
  return "No";
}
return "Yes";
```
### Introducing Else Statements Passed
```js
if (num > 10) {
  return "Bigger than 10";
} else {
  return "10 or Less";
}
```
### Introducing Else If Statements Passed
```js
if (num > 15) {
  return "Bigger than 15";
} else if (num < 5) {
  return "Smaller than 5";
} else {
  return "Between 5 and 15";
}
```
### Selecting from Many Options with Switch Statements
```js
switch(lowercaseLetter) {
  case "a":
    console.log("A");
    break;
  case "b":
    console.log("B");
    break;
}
```
### Adding a Default Option in Switch Statements
```js
switch (num) {
  case value1:
    statement1;
    break;
  case value2:
    statement2;
    break;
...
  default:
    defaultStatement;
    break;
}
```
### Replacing If Else Chains with Switch
```js
if (val === 1) {
  answer = "a";
} else if (val === 2) {
  answer = "b";
} else {
  answer = "c";
}
```
can be replaced by
```js
switch(val) {
  case 1:
    answer = "a";
    break;
  case 2:
    answer = "b";
    break;
  default:
    answer = "c";
}
```
### Returning Boolean Values from Functions
```js
function isEqual(a,b) {
  if (a === b) {
    return true;
  } else {
    return false;
  }
}
```
can be written as
```js
function isEqual(a,b) {
  return a === b;
}
```
### Return Early Pattern for Functions
* When a return statement is reached, the execution of the current function stops and control returns to the calling location.
```js
function myFun() {
  console.log("Hello");
  return "World";
  console.log("byebye")
}
myFun();
```
here "byebye" is never executed.

### Build JavaScript Objects
* Objects are similar to arrays, except that instead of using indexes to access and modify their data, you access the data in objects through what are called `properties`.
```js
var cat = {
  "name": "Whiskers",
  "legs": 4,
  "tails": 1,
  "enemies": ["Water", "Dogs"]
};
```
In this example, all the properties are stored as strings, such as - "name", "legs", and "tails"

### Accessing Object Properties with Dot Notation
* There are two ways to access the properties of an object: dot notation (.) and bracket notation ([]), similar to an array.
* Dot notation is what you use when you know the name of the property you're trying to access ahead of time.
```js
var myObj = {
  prop1: "val1",
  prop2: "val2"
};
var prop1val = myObj.prop1; // val1
var prop2val = myObj.prop2; // val2
```
### Accessing Object Properties with Bracket Notation
* The second way to access the properties of an object is bracket notation ([]). 
* If the property of the object **you are trying to access has a space in its name, you will need to use bracket notation**.
```js
var myObj = {
  "Space Name": "Kirk",
  "More Space": "Spock",
  "NoSpace": "USS Enterprise"
};
myObj["Space Name"]; // Kirk
myObj['More Space']; // Spock
myObj["NoSpace"];    // USS Enterprise
```
* Note that property names with spaces in them must be in quotes (single or double).

### Accessing Object Properties with Variables
* Another use of bracket notation on objects is to access a property which is stored as the value of a variable.
*  This can be very useful for iterating through an object's properties or when accessing a lookup table.
```js
var dogs = {
  Fido: "Mutt",  Hunter: "Doberman",  Snoopie: "Beagle"
};
var myDog = "Hunter";
var myBreed = dogs[myDog];
console.log(myBreed); // "Doberman"
```
### Updating Object Properties
```js
var ourDog = {
  "name": "Camper",
  "legs": 4,
  "tails": 1,
  "friends": ["everything!"]
};
ourDog.name = "Happy Camper";
```
### Add New Properties to a JavaScript Object
* You can add new properties to existing JavaScript objects the same way you would modify them.
```js
var ourDog = {
  "name": "Camper",
  "legs": 4,
  "tails": 1,
  "friends": ["everything!"]
};

ourDog.bark = "bow-wow";
```
### Delete Properties from a JavaScript Object
```js
var ourDog = {
  "name": "Camper",
  "legs": 4,
  "tails": 1,
  "friends": ["everything!"],
  "bark": "bow-wow"
};

delete ourDog.bark;
```
### Using Objects for Lookups
* Objects can be thought of as a **key/value storage, like a dictionary**. If you have tabular data, you can use an object to "lookup" values rather than a switch statement or an if/else chain. 
```js
var alpha = {
  1:"Z",
  2:"Y",
  3:"X",
  4:"W",
  ...
  24:"C",
  25:"B",
  26:"A"
};
alpha[2]; // "Y"
alpha[24]; // "C"

var value = 2;
alpha[value]; // "Y"
```
### Testing Objects for Properties
* Sometimes it is useful to check if the property of a given object exists or not.
*  We can use the .hasOwnProperty(propname) method of objects to determine if that object has the given property name.
*  ` .hasOwnProperty()` returns true or false if the property is found or not.
```js
var myObj = {
  top: "hat",
  bottom: "pants"
};
myObj.hasOwnProperty("top");    // true
myObj.hasOwnProperty("middle"); // false
```
### Manipulating Complex Objects
```js
var ourMusic = [
  {
    "artist": "Daft Punk",
    "title": "Homework",
    "release_year": 1997,
    "formats": [ 
      "CD", 
      "Cassette", 
      "LP"
    ],
    "gold": true
  }
];
```
### Accessing Nested Objects
```js
var ourStorage = {
  "desk": {
    "drawer": "stapler"
  },
  "cabinet": {
    "top drawer": { 
      "folder1": "a file",
      "folder2": "secrets"
    },
    "bottom drawer": "soda"
  }
};
ourStorage.cabinet["top drawer"].folder2;  // "secrets"
ourStorage.desk.drawer; // "stapler"
```
### Accessing Nested Arrays
```js
var ourPets = [
  {
    animalType: "cat",
    names: [
      "Meowzer",
      "Fluffy",
      "Kit-Cat"
    ]
  },
  {
    animalType: "dog",
    names: [
      "Spot",
      "Bowser",
      "Frankie"
    ]
  }
];
ourPets[0].names[1]; // "Fluffy"
ourPets[1].names[0]; // "Spot"
```
### Iterate with JavaScript While Loops
* The first type of loop we will learn is called a while loop because it runs "while" a specified condition is true and stops once that condition is no longer true
```js
var ourArray = [];
var i = 0;
while(i < 5) {
  ourArray.push(i);
  i++;
}
```
### Iterate with JavaScript For Loops
* The most common type of JavaScript loop is called a for loop because it runs "for" a specific number of times.
* `for ([initialization]; [condition]; [final-expression])`
```js
var ourArray = [];
for (var i = 0; i < 5; i++) {
  ourArray.push(i);
}
```
### Iterate Odd Numbers With a For Loop
```js
var ourArray = [];
for (var i = 0; i < 10; i += 2) {
  ourArray.push(i);
}
```
note: dont forget to declare variable :)

### Count Backwards With a For Loop
```js
var ourArray = [];
for (var i = 10; i > 0; i -= 2) {
  ourArray.push(i);
}
```
### Iterate Through an Array with a For Loop
* A common task in JavaScript is to iterate through the contents of an array. One way to do that is with a for loop
```js
var arr = [10, 9, 8, 7, 6];
for (var i = 0; i < arr.length; i++) {
   console.log(arr[i]);
}
```
### Nesting For Loops
```var arr = [
  [1,2], [3,4], [5,6]
];
for (var i=0; i < arr.length; i++) {
  for (var j=0; j < arr[i].length; j++) {
    console.log(arr[i][j]);
  }
}
```
### Iterate with JavaScript Do...While Loops
* The next type of loop you will learn is called a do...while loop. It is called a do...while loop because it will first do one pass of the code inside the loop no matter what, and then continue to run the loop while the specified condition evaluates to true.
```js
var ourArray = [];
var i = 0;
do {
  ourArray.push(i);
  i++;
} while (i < 5);
```
### Recursion
```js
  function multiply(arr, n) {
    if (n <= 0) {
      return 1;
    } else {
      return multiply(arr, n - 1) * arr[n - 1];
    }
  }
```
### Generate Random Fractions with JavaScript
* JavaScript has a `Math.random()` function that generates a random decimal number between 0 (inclusive) and not quite up to 1 (exclusive). 
* Thus `Math.random()` can return a `0` but never quite return a `1`

### Generate Random Whole Numbers with JavaScript
* Use Math.random() to generate a random decimal.
* Multiply that random decimal by 20.
* Use another function, **Math.floor() to round the number down to its nearest whole number**
```js
Math.floor(Math.random() * 20);
```
for random numbers between 0 to 19.

### Generate Random Whole Numbers within a Range
* we can generate a random whole number that falls within a range of two specific numbers.
* To do this, we'll define a minimum number min and a maximum number max
```js
Math.floor(Math.random() * (max - min + 1)) + min
```
### Use the parseInt Function
* The parseInt() function parses a string and returns an integer
```js
var a = parseInt("007");
```
* The above function converts the string "007" to an integer 7. 
* If the first character in the string can't be converted into a `number`, then it returns `NaN`.

### Use the parseInt Function with a Radix
* The parseInt() function parses a string and returns an integer. 
* It takes a second argument for the radix, which specifies the base of the number in the string.
*  The radix can be an integer between 2 and 36
```js
parseInt(string, radix);
var a = parseInt("11", 2);
```
### Use the Conditional (Ternary) Operator
* The conditional operator, also called the ternary operator, can be used as a one line if-else expression.
* `condition ? expression-if-true : expression-if-false;`
```js
function findGreater(a, b) {
  if(a > b) {
    return "a is greater";
  }
  else {
    return "b is greater";
  }
}
```
can be written as
```js
function findGreater(a, b) {
  return a > b ? "a is greater" : "b is greater";
}
```
### Use Multiple Conditional (Ternary) Operators
```js
function findGreaterOrEqual(a, b) {
  if (a === b) {
    return "a and b are equal";
  }
  else if (a > b) {
    return "a is greater";
  }
  else {
    return "b is greater";
  }
}
```
can be written as
```js
function findGreaterOrEqual(a, b) {
  return (a === b) ? "a and b are equal" 
    : (a > b) ? "a is greater" 
    : "b is greater";
}
```
### Explore Differences Between the var and let Keywords
```js
var camper = 'James';
var camper = 'David';
console.log(camper);
// logs 'David'
```
* As you can see in the code above, the camper variable is originally declared as James and then overridden to be David. 
* In a small application, you might not run into this type of problem, but when your code becomes larger, you might accidentally overwrite a variable that you did not intend to overwrite.
*  Because this behavior does not throw an error, searching and fixing bugs becomes more difficult.
*  **A new keyword called let was introduced in ES6 to solve this potential issue with the var keyword. If you were to replace var with let in the variable declarations of the code above, the result would be an error.**
```js
let camper = 'James';
let camper = 'David'; // throws an error
```
*  So unlike var, when using let, a variable with the same name can only be declared once. **Note the "use strict"**
*  This enables Strict Mode, which catches common coding mistakes and "unsafe" actions.
```js
"use strict";
x = 3.14; // throws an error because x is not declared
```
### Compare Scopes of the var and let Keywords
* When you declare a variable with the let keyword inside a block, statement, or expression, **its scope is limited to that block, statement, or expression.**

### Declare a Read-Only Variable with the const Keyword
* `const` has all the awesome features that let has, with the added bonus that **variables declared using const are read-only**. 
* They are a constant value, which means that once a variable is assigned with const, **it cannot be reassigned**.
* **Note**: It is common for developers to use **uppercase variable identifiers for immutable values** and **lowercase or camelCase for mutable values **(objects and arrays)

### Mutate an Array Declared with const
* It is important to understand that objects (including arrays and functions) assigned to a variable **using const** are still mutable.
*  Using the const declaration only prevents reassignment of the variable identifier

### Prevent Object Mutation
* To ensure your data doesn't change, JavaScript provides a function `Object.freeze` to prevent data mutation.
* Once the object is frozen, you can no longer add, update, or delete properties from it. Any attempt at changing the object will be rejected without an error
```js
let obj = {
  name:"FreeCodeCamp",
  review:"Awesome"
};
Object.freeze(obj);
obj.review = "bad"; // will be ignored. Mutation not allowed
obj.newProp = "Test"; // will be ignored. Mutation not allowed
console.log(obj); 
// { name: "FreeCodeCamp", review:"Awesome"}
```
### Use Arrow Functions to Write Concise Anonymous Functions
* In JavaScript, we often don't need to name our functions, especially when passing a function as an argument to another function.
*  Instead, we create **inline functions.**
*   We don't need to name these functions because we do not reuse them anywhere else.
```js
const myFunc = function() {
  const myVar = "value";
  return myVar;
}
```
can be wriiten as 
```js
const myFunc = () => {
  const myVar = "value";
  return myVar;
}
```
can be also written as
```js
const myFunc = () => "value";
```
using arrow functions

### Write Arrow Functions with Parameters
* Just like a regular function, you can pass arguments into an arrow function.
```js
// doubles input value and returns it
const doubler = (item) => item * 2;
doubler(4); // returns 8

// the same function, without the parameter parentheses
const doubler = item => item * 2;

// multiplies the first input value by the second and returns it
const multiplier = (item, multi) => item * multi;
multiplier(4, 2); // returns 8
```
### Set Default Parameters for Your Functions
* In order to help us create more flexible functions, ES6 introduces default parameters for functions.
```js
const greeting = (name = "Anonymous") => "Hello " + name;

console.log(greeting("John")); // Hello John
console.log(greeting()); // Hello Anonymous
```
### Use the Rest Parameter with Function Parameters
*  ES6 introduces the rest parameter for function parameters. 
*  With the rest parameter, you can create functions that take a variable number of arguments.
*  These arguments are stored in an array that can be accessed later from inside the function.
```js
function howMany(...args) {
  return "You have passed " + args.length + " arguments.";
}
console.log(howMany(0, 1, 2)); // You have passed 3 arguments.
console.log(howMany("string", null, [1, 2, 3], { })); // You have passed 4 arguments.

The rest parameter eliminates the need to check the args array and allows us to apply map(), filter() and reduce() on the parameters array.

Modify the function sum using the rest parameter in such a way that the function sum is able to take any number of arguments and return their sum.

The result of sum(0,1,2) should be 3

The result of sum(1,2,3,4) should be 10

The result of sum(5) should be 5

The result of sum() should be 0

sum should be an arrow function which uses the rest parameter syntax (...) on the args parameter.
```
### Use the Spread Operator to Evaluate Arrays In-Place
* ES6 introduces the spread operator, which allows us to expand arrays and other expressions in places where multiple parameters or elements are expected.
* The spread operator makes this syntax much better to read and maintain.
```js
const arr = [6, 89, 3, 45];
const maximus = Math.max(...arr); // returns 89
```
* `...arr` returns an unpacked array. In other words, it spreads the array. However, the spread operator only works in-place, like in an argument to a function or in an array literal. 

### Use Destructuring Assignment to Extract Values from Objects
* Destructuring assignment is special syntax introduced in ES6, for neatly assigning values taken directly from an object.
```js
const { name, age } = user;
// name = 'John Doe', age = 34
```
instead of
```js
const user = { name: 'John Doe', age: 34 };

const name = user.name; // name = 'John Doe'
const age = user.age; // age = 34
```
### Use Destructuring Assignment to Assign Variables from Objects
* Destructuring allows you to assign a new variable name when extracting values. You can do this by putting the new name after a colon when assigning the value.
```
const user = { name: 'John Doe', age: 34 };
const { name: userName, age: userAge } = user;
```
### Use Destructuring Assignment to Assign Variables from Nested Objects

```js
const user = {
  johnDoe: { 
    age: 34,
    email: 'johnDoe@freeCodeCamp.com'
  }
};

const { johnDoe: { age, email }} = user;

//or

const { johnDoe: { age: userAge, email: userEmail }} = user;
```
### Use Destructuring Assignment to Assign Variables from Arrays
* ES6 makes destructuring arrays as easy as destructuring objects.
* One key difference between the spread operator and array destructuring is that the spread operator unpacks all contents of an array into a comma-separated list. Consequently, you cannot pick or choose which elements you want to assign to variables.
* The variable a is assigned the first value of the array, and b is assigned the second value of the array. We can also access the value at any index in an array with destructuring by using commas to reach the desired index:
```js
const [a, b] = [1, 2, 3, 4, 5, 6];
console.log(a, b); // 1, 2

const [a, b,,, c] = [1, 2, 3, 4, 5, 6];
console.log(a, b, c); // 1, 2, 5

```
### Use Destructuring Assignment with the Rest Parameter to Reassign Array Elements
* In some situations involving array destructuring, we might want to collect the rest of the elements into a separate array.
```js
const [a, b, ...arr] = [1, 2, 3, 4, 5, 7];
console.log(a, b); // 1, 2
console.log(arr); // [3, 4, 5, 7]
```
### Use Destructuring Assignment to Pass an Object as a Function's Parameters
```js
const profileUpdate = (profileData) => {
  const { name, age, nationality, location } = profileData;
  // do something with these variables
}
```
can be written as
```js
const profileUpdate = ({ name, age, nationality, location }) => {
  /* do something with these fields */
}
```
### Create Strings using Template Literals
* A new feature of ES6 is the template literal. This is a special type of string that makes creating complex strings easier.
* Template literals allow you to create multi-line strings and to use string interpolation features to create strings.
```js
const person = {
  name: "Zodiac Hasbro",
  age: 56
};

// Template literal with multi-line and string interpolation
const greeting = `Hello, my name is ${person.name}!
I am ${person.age} years old.`;

console.log(greeting); // prints
// Hello, my name is Zodiac Hasbro!
// I am 56 years old.

```
### Write Concise Object Literal Declarations Using Object Property Shorthand
```js
const getMousePosition = (x, y) => ({
  x: x,
  y: y
});
```
can be written as
```js
const getMousePosition = (x, y) => ({ x, y });
```
### Write Concise Declarative Functions with ES6
```js
const person = {
  name: "Taylor",
  sayHello: function() {
    return `Hello! My name is ${this.name}.`;
  }
};
```
can be written as
```
const person = {
  name: "Taylor",
  sayHello() {
    return `Hello! My name is ${this.name}.`;
  }
};
```
### Use class Syntax to Define a Constructor Function
* ES6 provides a new syntax to create objects, using the `class` keyword.
```js
var SpaceShuttle = function(targetPlanet){
  this.targetPlanet = targetPlanet;
}
var zeus = new SpaceShuttle('Jupiter');
```
can be written as
```js
class SpaceShuttle {
  constructor(targetPlanet) {
    this.targetPlanet = targetPlanet;
  }
}
const zeus = new SpaceShuttle('Jupiter');
```
* It should be noted that the **class keyword declares a new function, to which a constructor is added. This constructor is invoked when new is called to create a new object**.
* UpperCamelCase should be used by convention for ES6 class names, as in SpaceShuttle used above.
* The constructor method is a special method for creating and initializing an object created with a class. 

### Use getters and setters to Control Access to an Object
* You can obtain values from an object and set the value of a property within an object.
* These are classically called **getters and setters**.
* Getter functions are meant to simply **return (get) the value of an object's private variable** to the user without the user directly accessing the private variable.
* Setter functions are meant to **modify (set) the value of an object's private variable based on the value passed into the setter function**. This change could involve calculations, or even overwriting the previous value completely.
```js
class Book {
  constructor(author) {
    this._author = author;
  }
  // getter
  get writer() {
    return this._author;
  }
  // setter
  set writer(updatedAuthor) {
    this._author = updatedAuthor;
  }
}
const novel = new Book('anonymous');
console.log(novel.writer);  // anonymous
novel.writer = 'newAuthor';
console.log(novel.writer);  // newAuthor
```
* Note: Notice the syntax used to invoke the getter and setter. They do not even look like functions. Getters and setters are important because they hide internal implementation details. Note: It is convention to precede the name of a private variable with an underscore (_)

###
* ES6 introduced a way to easily share code among JavaScript files. This involves exporting parts of a file for use in one or more other files, and importing the parts you need, where you need them. In order to take advantage of this functionality, you need to create a script in your HTML document with a type of module
 ```js
 <script type="module" src="filename.js"></script>
 ```
 * A script that uses this module type can now use the **import and export features**
 
 ### Use export to Share a Code Block
 * Imagine a file called math_functions.js that contains several functions related to mathematical operations. One of them is stored in a variable, add, that takes in two numbers and returns their sum. You want to use this function in several different JavaScript files. In order to share it with these other files, you first need to export it.
 ```js
 export const add = (x, y) => {
  return x + y;
}
```
also written as
```js
const add = (x, y) => {
  return x + y;
}

export { add };
```
### Reuse JavaScript Code Using import
* `import` allows you to choose which parts of a file or module to load
```js
import { add } from './math_functions.js';
```
* Here, import will find add in math_functions.js, import just that function for you to use, and ignore the rest. The ./ tells the import to look for the math_functions.js file in the same folder as the current file. The relative file path (./) and file extension (.js) are required when using import in this way.
```js
import { add, subtract } from './math_functions.js';
```
### Use * to Import Everything from a File
* Suppose you have a file and you wish to import all of its contents into the current file. This can be done with the import * as syntax. Here's an example where the contents of a file named math_functions.js are imported into a file in the same directory:
```js
import * as myMathModule from "./math_functions.js";
```
* The above import statement will create an object called myMathModule. This is just a variable name, you can name it anything. The object will contain all of the exports from math_functions.js in it, so you can access the functions like you would any other object property. Here's how you can use the add and subtract functions that were imported:
```js
myMathModule.add(2,3);
myMathModule.subtract(5,3);
```
### Create an Export Fallback with export default
* In the export lesson, you learned about the syntax referred to as a *named export*. This allowed you to make multiple functions and variables available for use in other files.
* There is another export syntax you need to know, known as *export default*. Usually you will use this syntax if only **one value is being exported from a file.** It is also used to create a **fallback value for a file or module**.
```js
export default function add(x, y) {
  return x + y;
}

// anonymous function
export default function(x, y) {
  return x + y;
}
```
### Import a Default Export
* In the following example, add is the default export of the math_functions.js file
```js
import add from "./math_functions.js";
```
* The syntax differs in one key place. The imported value, add, is not surrounded by curly braces ({}). add here is simply a variable name for whatever the default export of the math_functions.js file is.

### Create a JavaScript Promise
* A promise in JavaScript is exactly what it sounds like - you use it to make a promise to do something, usually asynchronously.
*  When the task completes, you either fulfill your promise or fail to do so.
* Promise is a constructor function, so you need to use the new keyword to create one. 
* It takes a function, as its argument, with two parameters - **resolve and reject**. These are methods used to determine the outcome of the promise. The syntax looks like this:
```js
const myPromise = new Promise((resolve, reject) => {

});
```
### Complete a Promise with resolve and reject
* A promise has three states: **pending, fulfilled, and rejected.**
* The promise you created in the last challenge is forever stuck in the pending state because you did not add a way to complete the promise. The resolve and reject parameters given to the promise argument are used to do this. 
* **resolve is used when you want your promise to succeed, and reject is used when you want it to fail.**
```js
const myPromise = new Promise((resolve, reject) => {
  if(condition here) {
    resolve("Promise was fulfilled");
  } else {
    reject("Promise was rejected");
  }
});
```
### Handle a Fulfilled Promise with then
* Promises are most useful when you have a process that takes an unknown amount of time in your code (i.e. something asynchronous), often a server request. 
* When you make a server request it takes some amount of time, and after it completes you usually want to do something with the response from the server.
*  This can be achieved by using the then method. The then method is executed immediately after your promise is fulfilled with resolve
```js
myPromise.then(result => {
  // do something with the result.
});
```
### Handle a Rejected Promise with catch
* catch is the method used when your promise has been rejected. 
* It is executed immediately after a promise's reject method is called
```js
myPromise.catch(error => {
  // do something with the error.
});
```
* error is the argument passed in to the reject method.

## Regular Expressions
### Using the Test Method
* If you want to find the word "the" in the string "The dog chased the cat", you could use the following regular expression: /the/
* JavaScript has multiple ways to use regexes. 
* One way to test a regex is using the .test() method. 
* The .test() method takes the regex, applies it to a string (which is placed inside the parentheses), and returns true or false if your pattern finds something or not
```js
let testStr = "freeCodeCamp";
let testRegex = /Code/;
testRegex.test(testStr);
// Returns true
```
### Match Literal Strings
* Any other forms of "Kevin" will not match. For example, the regex /Kevin/ will not match "kevin" or "KEVIN".
```js
let wrongRegex = /kevin/;
wrongRegex.test(testStr);
// Returns false
```
### Match a Literal String with Different Possibilities
* You can search for multiple patterns using the alternation or OR operator: |.
* This operator matches patterns either before or after it. For example, if you wanted to match "yes" or "no", the regex you want is /yes|no/.
* You can also search for more than just two patterns. You can do this by adding more patterns with more OR operators separating them, like /yes|no|maybe/.

### Ignore Case While Matching
* Case (or sometimes letter case) is the difference between uppercase letters and lowercase letters. Examples of uppercase are "A", "B", and "C". Examples of lowercase are "a", "b", and "c".
* You can match both cases using what is called a flag. There are other flags but here you'll focus on the flag that ignores case - the i flag. You can use it by appending it to the regex. An example of using this flag is /ignorecase/i. This regex can match the strings "ignorecase", "igNoreCase", and "IgnoreCase".

### Extract Matches
* You can also extract the actual matches you found with the .match() method
```js
"Hello, World!".match(/Hello/);
// Returns ["Hello"]
let ourStr = "Regular expressions";
let ourRegex = /expressions/;
ourStr.match(ourRegex);
```
* Note that the .match syntax is the "opposite" of the .test method you have been using thus far:
```js
'string'.match(/regex/);
/regex/.test('string');
```
### Find More Than the First Match
* To search or extract a pattern more than once, you can use the g flag.
```js
let repeatRegex = /Repeat/g;
testStr.match(repeatRegex);
// Returns ["Repeat", "Repeat", "Repeat"]
```
### Match Anything with Wildcard Period
* Sometimes you won't (or don't need to) know the exact characters in your patterns. Thinking of all words that match, say, a misspelling would take a long time. Luckily, you can save time using the wildcard character:` .`
* The wildcard character . will match any one character. The wildcard is also called dot and period. You can use the wildcard character just like any other character in the regex. For example, if you wanted to match "hug", "huh", "hut", and "hum", you can use the regex /hu./ to match all four words.
```js
let humStr = "I'll hum a song";
let hugStr = "Bear hug";
let huRegex = /hu./;
huRegex.test(humStr); // Returns true
huRegex.test(hugStr); // Returns true
```
### Match Single Character with Multiple Possibilities
* You can search for a literal pattern with some flexibility with character classes. Character classes allow you to define a group of characters you wish to match by placing them inside square ([ and ]) brackets
```js
let bigStr = "big";
let bagStr = "bag";
let bugStr = "bug";
let bogStr = "bog";
let bgRegex = /b[aiu]g/;
bigStr.match(bgRegex); // Returns ["big"]
bagStr.match(bgRegex); // Returns ["bag"]
bugStr.match(bgRegex); // Returns ["bug"]
bogStr.match(bgRegex); // Returns null
```
### Match Letters of the Alphabet
* Inside a character set, you can define a range of characters to match using a hyphen character: -
```js
let catStr = "cat";
let batStr = "bat";
let matStr = "mat";
let bgRegex = /[a-e]at/;
catStr.match(bgRegex); // Returns ["cat"]
batStr.match(bgRegex); // Returns ["bat"]
matStr.match(bgRegex); // Returns null
```
### Match Numbers and Letters of the Alphabet
* Using the hyphen (-) to match a range of characters is not limited to letters. It also works to match a range of numbers.
```js
let jennyStr = "Jenny8675309";
let myRegex = /[a-z0-9]/ig;
// matches all letters and numbers in jennyStr
jennyStr.match(myRegex);
```
### Match Single Characters Not Specified
* but you could also create a set of characters that you do not want to match. These types of character sets are called negated character sets.
* To create a negated character set, you place a caret character `(^)` after the opening bracket and before the characters you do not want to match.
* For example, `/[^aeiou]/gi` matches all characters that are not a vowel. Note that characters like ., !, [, @, / and white space are matched - the negated vowel character set only excludes the vowel characters.

### Match Characters that Occur One or More Times
* Sometimes, you need to match a character (or group of characters) that appears one or more times in a row. This means it occurs at least once, and may be repeated.
* You can use the `+` character to check if that is the case. Remember, the character or pattern has to be present consecutively. That is, the character has to repeat one after the other.
* For example, /a+/g would find one match in "abc" and return `["a"].` Because of the +, it would also find a single match in "aabc" and return `["aa"]`.
* If it were instead checking the string "abab", it would find two matches and return `["a", "a"]` because the a characters are not in a row - there is a b between them. Finally, since there is no "a" in the string "bcd", it wouldn't find a match.

### Match Characters that Occur Zero or More Times
* There's also an option that matches characters that occur zero or more times.
* The character to do this is the asterisk or star: `*`.
```js
let soccerWord = "gooooooooal!";
let gPhrase = "gut feeling";
let oPhrase = "over the moon";
let goRegex = /go*/;
soccerWord.match(goRegex); // Returns ["goooooooo"]
gPhrase.match(goRegex); // Returns ["g"]
oPhrase.match(goRegex); // Returns null
```
### Find Characters with Lazy Matching
* In regular expressions,**a greedy match** finds the longest possible part of a string that fits the regex pattern and returns it as a match. The alternative is called a **lazy match**, which finds the smallest possible part of the string that satisfies the regex pattern.
* You can apply the regex `/t[a-z]*i/` to the string "titanic". This regex is basically a pattern that starts with t, ends with i, and has some letters in between.
* Regular expressions are by default greedy, so the match would return `["titani"]`. It finds the largest sub-string possible to fit the pattern.
* However, you can use the ? character to change it to lazy matching. "titanic" matched against the adjusted regex of `/t[a-z]*?i/` returns `["ti"]`.

### Match Beginning String Patterns
* Outside of a character set, the caret is used to search for patterns at the beginning of strings.
```js
let firstString = "Ricky is first and can be found.";
let firstRegex = /^Ricky/;
firstRegex.test(firstString);
// Returns true
let notFirst = "You can't find Ricky now.";
firstRegex.test(notFirst);
// Returns false
```
### Match Ending String Patterns
* You can search the end of strings using the dollar sign character $ at the end of the regex.
```js
let theEnding = "This is a never ending story";
let storyRegex = /story$/;
storyRegex.test(theEnding);
// Returns true
let noEnding = "Sometimes a story will have to end";
storyRegex.test(noEnding);
// Returns false

```
### Match All Letters and Numbers
* The closest character class in JavaScript to match the alphabet is `\w`. 
* This shortcut is equal to `[A-Za-z0-9_]`. This character class matches upper and lowercase letters plus numbers. 
* Note, this character class also includes the underscore character `(_)`
```js
let longHand = /[A-Za-z0-9_]+/;
let shortHand = /\w+/;
let numbers = "42";
let varNames = "important_var";
longHand.test(numbers); // Returns true
shortHand.test(numbers); // Returns true
longHand.test(varNames); // Returns true
shortHand.test(varNames); // Returns true
```
### Match Everything But Letters and Numbers
* You can search for the opposite of the `\w` with` \W`. 
* Note, the opposite pattern uses a capital letter. This shortcut is the same as `[^A-Za-z0-9_]`
```js
let shortHand = /\W/;
let numbers = "42%";
let sentence = "Coding!";
numbers.match(shortHand); // Returns ["%"]
sentence.match(shortHand); // Returns ["!"]
```
### Match All Numbers
* The shortcut to look for digit characters is `\d`, with a lowercase d.
*  This is equal to the character class [0-9], which looks for a single character of any number between zero and nine

### Match All Non-Numbers
* The shortcut to look for non-digit characters is `\D`.
*  This is equal to the character class `[^0-9]`, which looks for a single character that is not a number between zero and nine.

### Restrict Possible Usernames ***

### Match Whitespace
* You can search for whitespace using `\s`, which is a lowercase s.
*  This pattern not only matches whitespace, but also carriage return, tab, form feed, and new line characters.
*   You can think of it as similar to the character class `[ \r\t\f\n\v]`

### Match Non-Whitespace Characters
* Search for non-whitespace using \S, which is an uppercase s. 
* This pattern will not match whitespace, carriage return, tab, form feed, and new line characters. 
* You can think of it being similar to the character class [^ \r\t\f\n\v]
```js
let whiteSpace = "Whitespace. Whitespace everywhere!"
let nonSpaceRegex = /\S/g;
whiteSpace.match(nonSpaceRegex).length; // Returns 32
```
### Specify Upper and Lower Number of Matches
* 































