# Numbers
One way to declare numbers
```js
const x=500 //upto 15 digits
const y= 0.5 //upto 17 decimals
```
```
* string + number= string
* number + string= string
* numeric string/ numeric string= answer
* numeric string * numeric string = answer`
```
## NaN - Not a Number
```
* non-numeric string / number = NaN
* NaN + number = NaN
* NaN + string = NaNstring
```
## Decimal to ...
 By default, JavaScript displays numbers as base 10 decimals.

But you can use the `toString()` method to output numbers from base 2 to base 36.

Hexadecimal is base 16. Decimal is base 10. Octal is base 8. Binary is base 2.
Example
```
var myNumber = 32;
myNumber.toString(10);  // returns 32
myNumber.toString(32);  // returns 10
myNumber.toString(16);  // returns 20
myNumber.toString(8);   // returns 40
myNumber.toString(2);   // returns 100000
```
## Comparison
* ==
* ===(strictly equal to)
* object==object is always false
* new keyword to create object

## Arithmetic Operations

| Symbol     | Meaning             | Example      |
|------------|---------------------|--------------|
| **         | Exponentiation      |              |
| ()         | Expression grouping | (3+4)        |
| .          | Member              | person.name  |
| []         | Member              | person[name] |
| ()         | Function call       | myFunction() |
| new        | create              | new Date()   |
| ++i        | prefix increment    |              |
| --i        | prefix decrement    |              |
| i++        | postfix increment   |              |
| i--        | postfix decrement   |              |
| !          | Logical not         | !(x==y)      |
| typeof     | Type of             | typeof x     |
| in         | Property in object  | 'PI' in Math |
| instanceof | Instance of object  | instanceof   |
| !=         | unequal             |              |
| !==        | Strict unequal      |              |
| &&         | Logical AND         | x&&y         |
| \|\|       | Logical OR          | X\|\|Y       |
| ?:         | CONDITION           | ?"yes":"no"  |


