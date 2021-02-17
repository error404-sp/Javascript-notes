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
var arr = [
  [1,2], [3,4], [5,6]
];
for (var i=0; i < arr.length; i++) {
  for (var j=0; j < arr[i].length; j++) {
    console.log(arr[i][j]);
  }
}
















