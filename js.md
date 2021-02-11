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









