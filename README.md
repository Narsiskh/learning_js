# JavaScript

in-line cm:create notes for yourself
```
//
```

multiline cm
```
/*   */
```

-----------------------------------

### Data Types & Variables :
#### Data Types:

string, number, object, underfined, null, boolean, symbol

1. String: any sort of text
2. Underfined: sth that hasnt been defined
3. Null: nothing
4. Boolean : true or false
5. Symbol: an immutable primitive value that is unique
6. Objetc: can store a lot of different key value pairs

#### Ways to declare a variable in JavaScript:

1. Var: A variable allows computers to store and manipulate data in a dynamic fashion/a lable to point to the data: 
```javascript
var x = ""
```
2. Let
 ```javascript
let x = " "
   ```
3. Const
```javascript
const x = " "
```
! Const can never change.

----------------------------------

### Incrementing & Decrememting Numbers :
#### Incrementing Numbers:

To increment a number means to add 1 to it

```javascript
var myVar = 87
myVar = myVar + 1
or 
myVar++;
```

#### Decrementing Numbers:
To decrement a number means subtracting 1 

```javascript
var myVar = 11
myVar = myVar - 1
or
myVar--
```

----------------------------------

### Finding a Remainder:

#### The remainder operator looks like a %

```javascript
var remainder;
remainder = 11 % 3
```

-----------------------------------

```javascript
var a = 3;
a = a + 12 or a += 12

var a = 11;
a = a- 6 or a -= 6

var a = 5;
a = a * 5 or a *= 5

var a = 48;
a = a / 12 or a /= 12
```

-------------------------------------

### Creat a string in JavaScript:

```javascript
var myfirstName = "Narsis"
```
--------------------------------------

### Show inner quotation mark:

use back slash \ before each quotation mark.

```javascript
var myStr = " I am a \"double quoted\" string inside \"double quoted\""

console.log(myStr)
```
! a string can either be surrounded by 'single quotes' or "double quoates".

```javascript
var myStr = '<p" I am a "double quoted" string inside "double quoted""/>'

console.log(myStr)
```
---------------------------------------

### Escape Sequencess:

Code       Output

`\' `        single quote

`\" `        double quote

`\\ `        backslash

`\n `        newline

`\r `        carriage return

`\t `        tab

`\b `        backspace 

`\f `        form feed

-------------------------------------
### Plus Operator:

#### Concatenating Strings:
you can do it with the + operator.

```JavaScript
var ourStr = "I come first. " + "I come second.";
```
! You should put a space before the end quotation mark.

or 
```javascript
var myStr = "I come first. "; 

myStr += "I come second. " 
```
or
```javascript
var myName = "Narsis" 
var myStr = "My name is " + myName + " And im well!";
```

#### Appending Variables to Strings:
```javascript
var anAdj = "worthwhile";
var myStr = "Learning to code is "
myStr += anAdj
```
-------------------------------------
### Length of String:
```javascript
var firstNameLength = 0
var firstName = "Narsis";
firstNameLength = firstName.length;
```
-------------------------------------
### Bracket Notation:
Bracket notation is a way to get a charachter at a specific index within a string.

! JS -> zero-based Indexing

```javascript
var firstLetterOfFirstName = "";
var firstName = "Ada";
 firstLetterOfFirstName = firstName[0];
 ```
 ! You can also use bracket notation to find the last letter in a string even if you dont know how many letters are in the string.
 ```javascript
 var firstName = "Ada";
 var lastLetterOfFirstName = firstName[firstName.length - 1];
 ```

! You can also use bracket notation to find the second, third, etc. to last letter in a string even if you dont know how many letters are in the string.

```javascript
var lastName = "Khoshnoud";
var seocndToLastLetterOfLastName = lastName[lastName.length-2];
```
-------------------------------------

### Word Blanks:
```javascript
function wordBlanks(noun, adj, verb, adv) {
   var result = "";
   result += "The " + adj + " " + noun + " " + verb + " to the store" + " " + adv;
   return result;
}
   console.log(wordBlanks("dog", "big", "ran", "quickly"));
```
! " " means space.

--------------------------------------

### Arrays:
Arrays allow you to store several pieces of data in one place.

! Arrays always start and end with bracket.

! Every element in the array is separated by a comma.

! Elements can be any data type.

```javascript
var ourArray = ["John", 24];
```
#### Nest Arrays:
When one of the elements in an array is another array,that`s called a nested array or a multidimensional array.
```javascript
var myArray = [["Birds", 23], ["White fox, 44]];
```
#### Access Array Data:
Earlier we learned how to ude bracket notation to find a specific index in a string. You can do the same thing with arrays.
```javascript
var theArray = [50,60,70];
var ourData = theArray[0];
```
#### Modify Array Data:
You can use array indexe to modify arrays.
```javascript
var thisarray = [18,64,99]
var thisarray[1] = 45
```
#### Access Multi-Dimensional Arrays:
You can also use bracket notation to select an element in a multi-dimensional or array of arrays.
```javascript
var herArray = [[1,2,3], [4,5,6], [7,8,9], [[10,11,12], 13, 14]];
var herData = herArray[0][1];
```
#### Push():
You can have pinned data to the end of an arrey with the push() function.
```javascript
var ourArray = ["Stimpson", "J", "cat"];
ourArray.push(["happy", "joy"]);
```
#### Pop():
You can remove an item from an array with the pop() function here.
```javascript
var myArray = [1,2,3];
var removedFromMyArray = myArray.pop();
```
#### Shift():
The shift() function is very similar to the pop function except it removes the first element of this array insted of the final element.
```javascript
Var ourArray = ["Stimpson", "J", "cat"];
var removedFromOurArray = ourArray.shift();
```
#### Unshift():
The unshift() function is similar to the push() array function. While push() adds an element to the end of the array, unshift() adds at element to the beginning of the array.
```javascript
var ourArray = ["Stimpson", "J", "cat"];
ourArray.shift();
ourArray.unshift("Happy")
```
#### Sort():
The sort() function use to sort the elements of the array alphabetically.
```javascript
var myArray = ["giga", "tera", "mega"];
myArray.sort();
```

##### Shopping List:
```javascript
var myList = [["cereal", 3], ["milk", 2], ["bananas", 3], ["juice", 2], ["eggs", 7]];
```
------------------------------------

### Function:
#### Write Reusable with Functions:
Functions allow us to create reusable code in JavaScript.
```javascript
function functionName(information) {
   Everything inside the curly bracket is run anytime the 'function' is called or invoked.
}
functionName(); --> Here the 'function' is being called.
```
#### Arguments:
Parameters are variable that act as place holders for the values that are to be input to a function when it is called.
```javascript
function ourFunctionWithArgs(a, b) {
   console.log(a -b);
}
ourFunctionWithArgs(10, 5);
```
#### Scopes:
Generally, scope refers to the parts of a program where a variable, function, object, etc. is accessible.
```javascript
const x = 10;

function getX() {
  alert(x);

  const y = 20;
}

getX();
alert(y); // error
```
In the function `getX` , we were able to access the variable `x` , which was defined outside the function, and `alert` it. Additionally, we defined a variable named `y` in this function and are alerting it in the last line. However, we get an error that `y` is not defined. Why does this happen? This is due to the rules that scopes have in JavaScript!

In JavaScript, we have three types of scopes: 
1. global scope
2. local scope
3. block scope

! Block: We refer to the space between two curly brackets `{ ... }`  a block in JavaScript. For example, the space inside `if`, `while`, and other statements.
```JavaScript
if (...) {
  /* 
    Block
  */
}

for (...) {
  /* 
    Block
  */
}

{
  /* 
    Block
  */
}
```
##### Global Scope & Functions:
Scope refers to the visibility of variables. Variables which are defined outside of a function block have global scope. Global Scope means they ca be seen everywhere in your JS code.
```javascript
const name = "Diego";

function func() {
  alert(name); // Diego
}

func();
```
In the code snippet above, the variable `name` is defined in the global scope because it is not restricted to any function or block and is in the outermost state. Variables defined in the global scope are also accessible in functions. Therefore, the above code runs without any issues.

! Global variables are accessible throughout the program.

##### Local Scope:
Variables defined within a function have local scope and are only accessible within that function.
```javascript
function getUser() {
  // Local Scope

  const user = "Mario";
  alert(user);
}

getUser();   // Mario
alert(user); // ReferenceError: user is not defined
```
In the above code snippet, the `alert` in line 7 works correctly because the variable `user` is in the same scope. However, the `alert` in the last line throws an error because the variable `user` does not exist in that scope. This scope is called Function Scope.

! What about Nested Functions?
 ```javascript
 function func1() {
  // Local Scope #1
  const name = "Mario";

  function func2() {
    // Local Scope #2 
    const lastname = "Doe";

    alert(`${name} ${lastname}`);
  }

  func2();
}

func1(); // John Doe
```
As we can see, a function named `func2` is defined inside another function named `func1`. According to the rules of scopes, inner functions can access the variables of their outer scopes. Therefore, the `func2` function has access to the `name` variable which is defined outside of it. However, the reverse is not true. Outer scopes cannot access the members of inner scopes.
```javascript
function func1() {
  function func2() {
    const x = 10;
  }

  alert(x);
}

func1(); // ReferenceError: x is not defined
```

##### Block Scope:
As we mentioned, we call the space between two brackets a block. Variables defined with `let` and `const` are only accessible within that block:
```javascript
{
  let x = 29;
}

alert(x) // ReferenceError: x is not defined
```
However, this is not the case for `var`. A variable defined with `var` inside a block is also accessible outside that block:
```javascript
{
  var x = 12;
}

alert(x) // 12
```
In fact, the scope that a block creates is the same as local scope. That is, it is only accessible in that place:
```javascript
const x = 10;
{
  const x = 20;
  alert(x); // 20
}

alert(x); // 10
```
By running the above code, we can see that the variable `x` inside the block does not interfere with the `x` defined outside. These two are actually separate variables.

! If we have nested blocks, members of an outer block cannot access members of inner blocks; but members of inner blocks can access members of outer blocks:
```javascript
const x = 1;
{
  const y = 2;
  {
    alert(x); // ok
    alert(y); // ok

    const z = 3;
  }
  alert(z); // error
}

alert(y); // error
```
#### Return a Value from a Function:
you can return a Value from a function with this return statement.
```javascript
function minusSeven(num) {
   return num - 7;
}
console.log(minusSeven(20));
```
#### Undefined Value Returned:
If you dont specify a return value, the return value is just undefined.
```javascript
var sum = 0
function addThree() {
   sum = sum + 3;
}

function addFive() {
   sum += 5;
}
```
#### Assignment With a Returned Value:
Assignment with a Returned Value in JavaScript means assigning a value using the return value of a function. In other words, you can assign the return value of a function to a variable.
```javascript
var changed = 0;

function change(num) {
   return (num + 5) / 3;
}

changed = changed(10);

var processed = 0;

function processArg(num) {
   return (num + 3) / 5;
}

processed = processedArg(7);
```
#### Stand in Line:

In computer science a cue is an abstract data structure where items are kept in order.
New items can be added to the back of the cue and old items are taken off from the front of the cue.
```javascript
function nextInLine(arr, item) {
   arr.push(item);
   return arr.shift();

}

var testArr = [1,2,3,4,5];

console.log("Before: " + JSON.stringify(testArr));
console.log(nextInLine(testArr, 6));
console.log("After: " + JSON.stringify(testArr));
```
--------------------------------------
### Boolean Values:
Booleans are another data type in JS.
They are only two values:
1. True
2. False

! They dont use quotation marks around the Boolean.
```javascript
function welcomeToBooleans() {
   return true;
}
```
--------------------------------------
### If Statements:
An if statement is used to make decisions in code.

The keyword `if` tells JS to execute the code in the curly braces under certain conditions defined in the paranthesis

! Theres always parenthesis the keyword `if` ,and shows the condition.

```javascript
function trueOrFalse(wasThatTrue) {
   if (wasThatTrue) {
      return "Yes, that was true";
   }
   return "No, that was false";
}

console.log(trueOrFalse(true));
```
#### Equality Operators:
##### Equality Operators: 
There are many comparison operators in JS that will return a Boolean of true or false.The most common is the equality operator ,and it often used in an if statement.

```javascript
function testEqual (val) {
   if (val == 12) {
      return "Equal";
   }
}

console.log(testEqual(10));
```
##### Strict Equality Operators:
We learned about the equality operator which is the double equal == sign. Theres also the strict equality operator the triple equal sign ===.

```javascript
function testStrict(val) {
   if (val === 7) {
      return "Equal";
   }
   return "Not Equal";
}

testStrict(10);
/*
3 == 3
3 === '3'
*/
```
###### Practice Comparing Different Values:
Lets do one more review with the equality operators and the strict equality operators.
```javascript
function compareEquality(a, b) {
   if (a === b) {
      return "Equal";
   }
   return "Not Equal";
}

console.log(compareEquality(10, "10"));
```
```javascript
function compareEquality(a, b) {
   if (a == b) {
      return "Equal";
   }
   return "Not Equal";
}

console.log(compareEquality(10, "10"));
```

##### Comparison with the Inequality Operator: 
 Here we show you the inequality operator, which is basically the opposite of the equality operator.
 ```javascript
 function testNotEqual(val) {
   if (val != 99) {
      return "Not Equal";
   }
   return "Equal";
 }

 console.log(testNotEqual(10));
 ``` 

 ##### Comparison with the Strict Inequality Operator:
 Here we show you the inequality operator, which is basically the opposite of the strict equality operator.
 ```javascript
 function testStrictNotEqual(val) {
  if (val !== 17) {
     return "Not Equal";
  }
  return "Equal";
}

console.log(testNotEqual(10));
 ```

 ##### Comparison with the Logical And Operator:
We can also use the greater than operator.
```javascript
function testGreaterThan(val) {
   if (val > 100) {
      return "over 100";
   }
 
   if (val > 10) {
      return "over 10";
   }

   return "10 or Under";
}

console.log(testGreaterThan(10));
```
##### Comparison with the Greater Than or Equal To Operator:
```javascript
function testGreaterOrEqual(val) {
   if (val >= 20) {
      return "20 or over";
   }

   if (val >= 10) {
      return "10 or over";
   }

   return "Less than 10";
}

console.log(testGreaterOrEqual(10));
```
 ##### Comparison with the Less Than Operator:
 ```javascript
function testLessThan(val) {
   if (val < 25) {
      return "Under 25";
   }

   if (val < 55) {
      return "Under 55";
   }

   return "55 or Over";
}

console.log(testLessThan(10));
```
##### Comparison with the Less Than or Equal To Operator:
```javascript
function testLessOrEqual(val) {
   if (val <= 12) {
      return "Smaller Then or Equal to 12";
   }

   if (val <= 24) {
      return "Smaller Then or Equal to 24";
   }

   return "More than 24";
}

console.log(testLessOrEqual(10));
```