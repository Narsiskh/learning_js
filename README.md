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
2. Undefined: sth that hasnt been defined
3. Null: nothing
4. Boolean : true or false
5. Symbol: an immutable primitive value that is unique
6. Objetc: can store a lot of different key value pairs

#### Ways to declare a variable in JavaScript:

1. Var: A variable allows computers to store and manipulate data in a dynamic lable to point to the data: 
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

### Incrementing & Decrementing Numbers :
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
var secondToLastLetterOfLastName = lastName[lastName.length-2];
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
Earlier we learned how to use bracket notation to find a specific index in a string. You can do the same thing with arrays.
```javascript
var theArray = [50,60,70];
var ourData = theArray[0];
```
#### Modify Array Data:
You can use array indexe to modify arrays.
```javascript
var thisArray = [18,64,99]
var thisArray[1] = 45
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

! Block: We refer to the space between two curly braces `{ ... }`  a block in JavaScript. For example, the space inside `if`, `while`, and other statements.
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
As we mentioned, we call the space between two curly braces a block. Variables defined with `let` and `const` are only accessible within that block:
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
#### And / Or Operator:
##### And:
Sometimes you want to check if 2 things are true at the same time.
Here we can add `and` statement, which is just two pipes `&&`.
```javascript
function testLogicalAnd(val) {
   if (val <= 50 && val >= 25) {
      return "Yes";
   }
   return "No";
}

testLogicalAnd(10);
``` 
So this says if value is less than or equal to 50, and the value is also more than or equal 25. Then we are going to return "Yes". So both statements have to be true to get inside this if statemnet here.

##### Or:
In this code here, we are checking if the value is not between 10 and 20. So, if the values is less than 10, we return "Outside", and if the value is more than 20, we return "Outside". Here we can add `or`statement, which is just two pipes `||`.
```javascript
function testLogicalOr(val) {
   if (val < 10 || val > 20) {
      return "Outside";
   }
   return "Inside";
}

testLogicalOr(15);
```
So, now, we are checking if the value is less than 10 or if the value is more than 20.

### Else Statement:
When an if statement is true, normally the block of code right after the if statement will be evaluated, and if its not true, nothing happens.
 But with an else statement, an alternate block of code can be executed when its not true.

 ```javascript
 function testElse(val) {
   var result = "";

   if (val > 5) {
      result = "Bigger than 5";
   } else {
      result = "5 or smaller";
   }
   return result;
 }

 testElse(4);
 ```

 ### ELse If statement:
 If you have multiple conditions that need to be addressed, you can use else if statement. Its a way of chaning if statements together.
 ```javascript
 function testElseIf(val) {
   if (val > 10) {
      return "Greater than 10";
   } else if (val < 5) {
      return "Smaller than 5";
   } else {
      return "Between 5 and 10";
   }
 }

 testElseIf(7);
 ```

 #### Logical Order in If Else Statements:
 When you are using else if statements, order is very important.
 ```javascript
 // Wrong
 function orderMyLogic(val) {
   if (val < 10) {
      return "Less than 10";
   } else if (val < 5) {
      return "Less than 5";
   } else {
      return "Greater than or equal to 10";
   }
 }

 console.log(orderMyLogic(3));
 // Less Than 10
 ```
 ```javascript
 // Right
 function orderMyLogic(val) {
   if (val < 5) {
      return "Less than 5";
   } else if (val < 10) {
      return "Less than 10";
   } else {
      return "Greater than or equal to 10";
   }
 }

 console.log(orderMyLogic(3));
 // Less Than 5
 ```
 #### Chaining If Else Statements:
 You can also chain if and else if statements.
 ```javascript
 function testSize(num) {
   if (num < 5) {
      return "Tiny"
   } else if (num < 10) {
      return "Small"
   } else if (num < 15) {
      return "Medium"
   } else if (num < 20) {
      return "Large"
   } else {
      return "Huge"
   }
 }

console.log(testSize(7));
 
 /*
 Write chained if/else if statements to fulfill the following conditions:

 num < 5 - return "Tiny"
 num < 10 - return "Small"
 num < 15 - return "Medium"
 num < 20 - return "Large"
 num >= 20 - return "Huge"
 */
 ```
 ##### Golf Code:
 In the game of golf each hole has a par, which means the average number of strokes you are supposed to use to get the ball into the hole. So depending on how far above or below par your strokes are, there is a different nickname.
 ```javascript
 var names = ["Hole-in-one!", "Eagle", "Birdie", "Par", "Bogey", "Double Bogey", "Go Home!"]
 function golfScore(par, strokes) {
   if (strokes == 1) {
      return names[0]
   } else if (strokes == <= par - 2) {
      return names[1]
   } else if (strokes == par - 1) {
      return names[2]
   } else if (strokes == par) {
      return names[3]
   } else if (strokes == par + 1) {
      return names[4]
   } else if (strokes == par + 2) {
      return names[5]
   } else if (strokes >= par + 3) {
      return names[6]
   }
 }

console.log(golfScore(5, 4));


 /*
 Strokes        Return
 1              "Hole-in-one!"
 <= par - 2     "Eagle"
 par - 1        "Birdie"
 par            "Par"
 par + 1        "Bogey"
 par + 2        "Double Bogey"
 >= par + 3     "Go Home!"
 */
 ```
### Switch Statements:
Instead of using chained else if statements you can use a switch statement. A switch statement tests a value and can have many case statements which define various possible values.
```javascript
function caseInSwitch(val) {
   var answer = "";
   switch(val) {
      case 1:
         answer = "alpha";
         break;
      case 2:
         answer = "beta"
         break;
      case 3:
         answer = "gamma"
         break;
      case 4:
         answer = "delta"
         break;
   }

   return answer;
}

console.log(caseInSwitch(1));

/*
Write a switch statement which tests val and sets answer for the following conditions:
1 - "alpha"
2 - "beta"
3 - "gamma"
4 - "delta"
*/
```
! Break means that we are at the end of that case statement.

#### Default Option in Switch Statements:
The default option is kind of like else in an if else statement.
What if we want to return something anytime a, b, or c is not passed through?
So, for anything else thats passed into the function, we are going to do default. This is like the else statement.
In this example, whenever we pass in something thats not a, b, or c, its going to return "stuff".
```javascript
function switchOfStuff(val) {
   var answer = "";

   switch(val) {
      case "a":
         answer = "apple";
         break;
      case "b":
         answer = "bird"
         break;
      case "c":
         answer = "cat"
         break;
      default:
         answer = "stuff";  
         break;   
   }

   return answer;
}

console.log(switchOfStuff(3)); //stuff

/* 
Write a switch statement which tests val and sets answer for the following conditions:
a - "apple"
b - "bird"
c - "cat"
*/
```
#### Muktiple Identical Options in Switch Statement:
Sometimes you want a switch statement where multiple inputs give the same output.
```javascript
function sequentialSizes(val) {
   var answer = "";
   switch(val) {
      case 1:
      case 2:
      case 3:
         answer = "Low";
         break;   
      case 4:
      case 5:
      case 6:
         answer = "Mid";
         break; 
      case 7:
      case 8:
      case 9:
         answer = "High";
         break;                  
   }
   return answer;
}

console.log(sequentialSizes(3)); //Low
```
#### Replacing If Else Chains with Switch:
```javascript
function chainToSwitch(val) {
   var answer = "";
   switch(val) {
      case "bob":
         answer = "Marley";
         break; 
      case 42:
          answer = "The Answer";
         break; 
      case 1:
         answer = "There is no #1";
         break;   
      case 99:
          answer = "Missed me by this much";
         break; 
      case 7:
          answer = "Ate Nine";
         break;                   
   }
   return answer;
}

console.log(chainToSwitch("bob"));
```
-------------------------------------
### Returning Boolean Values from Functions:
```javascript
function isLess(a, b) {
   return a < b;
}

console.log(isLess(10, 15));
```
--------------------------------------
### Return Early Pattern for Functions: 
```javascript
function abTest(a, b) {
   if (a < 0 || b < 0) {
      return undefined;
   }
   return Math.round(Math.pow(Math.sqrt(a) + Math.sqrt(b), 2));
}

console.log(abTest(-2, 2));
```
--------------------------------------
###  Counting Cards:
We are going to create a blckjack card counting function.

So, how card counting works? Is that when you see a low card, the count goes up, and when you see a high card, the count goes down, and if its a middle value card, the count stays the same. Then when the count is positive, the player should bet high, and when the count is a zero or negative, the player should bet low.

```javascript
var count = 0;

function cc(card) {
   switch(card) {
      case 2:
      case 3:  
      case 4:      
      case 5:     
      case 6:    
        count++;
        break;
      case 10:
      case "J":  
      case "9":    
      case "Q":  
      case "K":   
      case "A":   
        count++;
        break;  
        count--;
        break;      
   }

   var  holdbet = 'Hold'
   if (count > 0)
     holdbelt = 'Bet'
   return count + " " + holdbet;
}

cc(2); cc('K'); cc(7); cc('K'); cc('A');
console.log(cc(4));
```
-------------------------------------
### Objects:
#### Build JS Objects:
Objects are similar to arryas except that instead of using indexes to access data, you use properties.

Objects are going to be defined with these curly braces at the beginning and the end.

The properties are everything before the colons.

The values are the things after the colons.

! properties can be strings, numbers or arrays.
```javascript
var ourDog = {
   "name": "Camper",
   "legs": 4,
   "tails": 1,
   "friends": ["everything!"]
};
```

#### Dot Notation:
There are two main ways to access a property on an object:

1. Dot Notation
2. Bracket Notation

```javascript
var testObj = {
   "hat": "ballcap",
   "shirt": "jersey",
   "shoes": "cleats"
};

var hatValue = testObj.hat;
var shirtValue = testObj.shirt;
```
#### Bracket Notation:
You can use bracket notation anytime but it is required if the name has a space in it.
```javascript
var testObj = {
   "an entree": "hamburger",
   "my side": "veggies",
   "the drink": "water"
};

var entreeValue = testObj["an entree"];
var drinkValue = testObj['the drink'];
```
#### Variables:
Bracket notation can also be used to look up object properties using variables.
```javascript
var testObj = {
   12: "Namath",
   16: "Montana",
   19: "Unitas",
};

var playerNumber = 16;
var playerNumber = testObj[playerNumber];
```
#### Updating Object Properties:
We can also use dot notation to update object properties.
```javascript
var ourDog = {
   "name": "Camper",
   "legs": 4,
   "tails": 1,
   "friends": ["everything!"]
};

console.log(ourDog.name = "Happy Camper");
```
#### Add New Properties to Object:
You can add new proprties to an object using dot notation or Delete Properties from Object
```javascript
var yourDog = {
    "name": "Camper",
    "legs": 4,
    "tails": 1,
    "friends": ["everything!"]
};

console.log(yourDog.bark = "bow-wow")
```
#### Delete Properties from Object:
```javascript
var yourDog = {
    "name": "Camper",
    "legs": 4,
    "tails": 1,
    "friends": ["everything!"],
};  "bark" : "bow-wow"

delete yourDog.bark;
```
#### Objects for Lookups:
Objects can be thought of as a key value storage like dictionary.
You can use an object to lookup values.
```javascript
function phoneticLookup(val) {
   var result = ""; 

   var lookup = {
      "alpha": "Adams",
      "bravo": "Boston",
      "charlie": "Chicago",
      "delta": "Denver",
      "echo":  "Easy",
      "foxtrot": "Frank"
   };
   result = lookup[val]

   return result;
}

console.log(phoneticLookup("charlie"));

 ```
 #### Testing Objects for Properties:
 You can check if an object has a property with the hasown property method. If it doesnt have the property, we will return "Not found".
 ```javascript
 var myObj = {
   gift: "pony",
   pet: "kitten",
   bed: "sleigh"
 };

 function checkObj(checkProp) {
   if (myObj.hasOwnProperty(checkProp)) {
      return myObj[checkProp]
   } else {
      return "Not Found"
   }
 }

 console.log(checkObj("Hello"));
 ```
#### Manipulating Complex Objects:
A JS object is a way to store flexible data.
```javascript
var myMusic = [
   {
      "artist": "Billy Joel",
      "title"; "Piano Man",
      "release_year": 1973,
      "formats": [
         "CD",
         "8T",
         "LP"
      ],
      "gold": true
   },
   {
      "artist": "Beau Carnes",
      "title": "Cereal Man"
      "release_year": 2003,

   }
];
```
#### Nested Objects:
##### Accessing Nested Objects:
```javascript
var myStorage = {
   "car": {
      "inside": {
         "glove box": "maps",
         "passenger seat": "crumbs"
      },
      "outside":{
         "trunk:; "jack"      }
   }
}
Var gloveBoxContents = myStorage. car.inside["glove box];

console.log(gloveBoxContents);
```

#### Nested Arrays:
```javascript
var myPlants = [
   {
      type: "flowers",
      list: [
         "rose",
         "tulip",
         "dandelion",
         ]
   },
   {  type: "trees",
      list: [
         "fir",
         "pine",
         "birch"
      ]
   }
       
];

console.log(secondTree = myPlants[1].list[1])
```
### Loops:
Loops allow you to run the same code multiple times.

#### While Loops:
A while loop that runs while a specified condition is true and stops once its no longer true.
```javascript
var myArray = []

var i = 0;
while(i < 5) {
   myArray.push(i);
   i++;
}
console.log(myArray);
```
#### For Loops:
A for loop is the most common type of loop in javascript. We start with the keyWord 'For', and then we have these parantheses with three different items and they are separated by semicolons.

The first things is the initiazization. Then we have the conidition, and then we have the final expression.
```javascript
var ourArray = [];

for (var i = 0; i < 5; i++) {
   ourArray.push(i);

}
console.log(ourArray);
```
##### Odd Number With a For Loop:
Loops dont just have to increment one at a time.
```javascript
var myArr = [];

for (var i = 0; i < 10; i+= 2) {
   myArr.push(i);
}
console.log(myArr);
```
##### Count Backwards with a For Loop:
A for loop can also be used to count backwards. So if we see this for loop here, we are initializing i to 10. We are starting at 10 and we are going back to 0.
```javascript
var herArr = [];
for (var i = 10; i > 0; i -= 2) {
   herArr.push(i);
}

console.log(herArr);
```
##### Iterate Through an Array with a For Loop:
```javascript
var myArr = [2, 3, 4, 5, 6];
var total = 0;

for (var i = 0; i < myArr.length; i++) {
   total += myArr[i];
}

console.log(total);
```
##### Nesting For Loops:
If you have a multidimensional or nested array, we can use nested for loops to access all the array elements.
```javascript
function multiplyAll(arr) {
   var product = 1;

   for (var i = 0; i < arr.length; i++) {
      for (var j = 0; j < arr[i].length; j++) {
         product *= arr[i][j]
      }
   }

   return product;
}

var product = multiplyAll([[1,2],[3,4],[5,6,7]]);
console.log(product);
```
#### Do...While Loops:
In a do while loop, this is always run at least once before it checks thr=e condition.
```javascript
var hisArr = [];
var i = 10;

do {
   hisArr.push(i);
   i++;
} while (i < 5)

console.log(i, hisArr);
```
-------------------------------------------------------------

### Random Fractions and Whole Numbers:
#### Generate Random Fractions:
There's a simple way to creat a random decimal number in JS. It's with the math.random function.
Its always going to be a number between 0 and 1. It could be 0 but it could not be 1.
```javascript
 function  randomFraction() {

     return  Math.random()
 }
 console.log(randomFraction());
```
#### Generate Random Whole Numbers:
Often you want a randome whole number instead of a random decimal number. That can be accomplished with `Math.floor`. This rounds down to the nearest whole number.
```javascript
var randomNumberBetween0and19 = Math.floor(Math.random() * 20);

function randomWholeNum() {
   return Math.random();
}

console.log(randomWholeNum());
```
So we pass in `Math.random()*20`, and then we round down to the nearest whole number. This going to ccreate a random whole number between 0 and 19.

! Remember `Math.random` can never be 1. So when we multiply it by 20, we are going to get a number between 0 and 20, but not including 20.

#### Generate Random Whole Numbers within a Range:
You can also generate random whole numbers within a range.
```javascript
function ourRandomRange(ourMin, ourMax) {
   return Math.floor(Math.random() * (ourMin - ourMax + 1)) + ourMin;

}

console.log(ourRandomRange(1, 9));
```
------------------------------------------------------------
 ### ParseInt Function: 
 #### Use the ParseInt Function:
 Another useful function is the parseInt function. It takes a string and returns an integer. A lot of times you want to make sure you are dealing with integers and not strings for different calculations and things like that. If the string cannot be converted into an integer, it returns in NaN for Not a Number.
 ```javascript
 function convertToInteger(str) {
   return parseInt(str);

 }
 convertToInteger("56");
 ```
#### Use the ParseInt Function with a Radix:
The parseInt function can also be used with a radix. The radix specifies the base of the number in the string.
```javascript
 function convertToIntegers(str) {
   return parseInt(str, 2);

 }
 convertToIntegers("10011");
 ```
 --------------------------------------------------------------

### Ternary Operator:
#### Use the Ternary Operator:
It is like a one line if else expression.

This is what it looks like:

condition ? statement-if-true : statement-if-false;

You have your condition just like in an if statement. Then you would have a question mark. After the question mark you have whats going to happen if the conditionis is true, then you have a colon. Then you have what is going to happen if the condition is false.

```javascript
function checkEqual(a, b) {
   return a === b ? true : false;

   /* in real life we use: 
   return a === b; */
   
}
checkEqual(1, 2);
```
#### Use Multiple conditional (Ternary) Operators:
One of the great things about conditional or ternary operators is that you can nest them within each other which gives them even more power.
```javascript
function checkSign(num) {
   return num > 0 ? "positive" : num < 0 ? "negative" : "zero"
}

console.log(checkSign(0));
```
-------------------------------------------------------------

### Var vs Let: 
For a long time in JS if you were going to declarea vriable, you had to use the `var` keyword. But starting with ES^ in 2015 we can now declare variables with `let` and `const` as well.

! `let` does not let you declare a variable twice.
```javascript
var catName = "Quincy";
var quote;

var catName = "Beau";

function catTalk() {
   "use strict";

   catName = "Oliver";
   quote = catName + "says Meow!";
}
catTalk();
```
If we change all the `var` to `let`, and we load it again, we will see an error, Duplicate declararion "catName". So, this is good that its creating this error, because you usually dont want to declare a variable two times in the same scope. So, this allows yout program to give you an error to tell you that you have done something wrong.
```javascript
let catName = "Quincy";
let quote;

catName = "Beau";

function catTalk() {
   "use strict";

   catName = "Oliver";
   quote = catName + "says Meow!";
}
catTalk();
```
#### Compare Scope of the var and let keywords:
Another major difference between the var and let keywords is that when you declare a variable with var, it is declared globally or locally if declared inside a function. However, `let`-the scope of let is limited to the block statement or  expression that it was declare in.
```javascript
function checkScope() {
   "use strict";
   if (true) {
      let i = "block scope";
      console.log("Block scope i is: ", i);
   }
   console.log("Function scope i is: ", i);
   return;
}

checkScope();
```
So, thats another reasons why people use `let` instaed of `var`.

### Const Keyword:
#### Declare a Read-Only Variable with the const Keyword:
Const is another way to declare a variable. It has all the features of `let` but its also read-only. You cannot reassign a `const`.

! When you are using `const` its very common to use all capital letters.

```javascript
function printManyTimes(str) {
   "use strict";

   const SENTENCE = str + " is cool!";

   sentence = str + " is amazing!"

   for(let i = 0; i < str.length; i+=2) {
      console.log(sentence);
   }
}
printManyTimes("freeCodeCamp");
```
#### Mutate an Array Declared with const:
While you cannot reassign a variable declare with `const` you can mutate an array.
```javascript
const s = [5, 7, 2];
function editInPlace() {
   "use strict";

   //s = [2, 5, 7];
   s[0] = 2;
   s[1] = 5;
   s[2] = 7;
}
editInPlace();

console.log(s)
```
-------------------------------------------------------------

### Prevent Object Mutation:
As seen previouslyt, a const declaration alone doesnt really protect your data from mutation.
```javascript
function freezeObj() {
   "use strict";
   const MATH_CONSTANTS = {
      PI: 3.14
   };

   Object.freeze(MATH_CONSTANTS)

   try {
      MATH_CONSTANTS.PI = 99;
   } catch( ex ) {
      console.log(ex);
   }
   return MATH_CONSTANTS.PI;
}

const PI = freezeObj();

console.log(PI);
```
--------------------------------------------------------------
### Arrow Functions:
#### Use Arrow Function to Write Concise Anonymous Functions:
This funtion here is called an anonymous function. It doesnt have a name. It is assigned to this variable magic, but there is no word right before the function keyword to assign the name to the function.
```javascript
var magic = function() {
   return new Date();
};
```
Whenever you have an anonymous function, you can convert it into an arrow function. That makes it a little quicker to write. So instead of the word function, Im going to take that out completely, and then put an arrow here.
```javascript
const magic = () => new Date();
```
#### Write Arrow Functions with Parameters:
Just like in a normal function, you can pass arguments to arrow functions.
```javascript
var myConcat = function(arr1, arr2) {
   return arr1.concat(arr2)
};
console.log(myConcat([1, 2], [3, 4, 5]));
```
How to convert this function into an arrow function? 
```javascript
const myConcat = (arr1, arr2) => arr1.concat(arr2);

console.log(myConcat([1, 2], [3, 4, 5]));
```
#### Write Higher Order Arrow Functions:
Arrow functions work relly well with higher order functions such as map, filter, and reduce. They take functions as arguments for processing collections of data.Whenever one function takes another function as an argument, thats a good time for an arrow function.
```javascript
const realNumberArray = [4, 5.6, -9.8, 3.14, 42, 6, 8.34, -2];

const squareList = (arr) => {
   const squaredIntegers = arr.filter((num) => Number.isInteger(num) && num > 0).map((x) => x * x);
   return squaredIntegers;
};

const squaredIntegers = squareList(realNumberArray);
console.log(squaredIntegers);
```
---------------------------------------------------------------
### Default Parameters:
In order to creat more flexible functions you can use default parameteres.
```javascript
const increment = (function() {
   return function increment(number, value) {
      return number + value;
   };
})();
console.log(increment(5, 2));
console.log(increment(5));
```
----------------------------------------------------------------
### Rest Operator:
The rest operator allows you to create a function that takes a variable number of arguments.
```javascript
const sum = (function() {
   return function sum(x, y, z) {
      const args = [ x, y, z];
      return args.reduce((a, b) => a + b, 0);
   };
})();
console.log(sum(1, 2, 3));
```
#### Use the Rest Operator with Function Parameters:
Here the rest operator will convert everything thats passed in into one array and the array is called args . So we dont need `const args = [ x, y, z];`.
```javascript
const sum = (function() {
   return function sum(...args) {
      return args.reduce((a, b) => a + b, 0);
   };
})();
console.log(sum(1, 2, 3));
```
-------------------------------------------------------------
### Spread Operator:
The spread operator looks just like the rest operator, three dots. But it expands an already existing array or it spreads out an array.

Here we are making `arr2` equal all of the contents of `arr1` so they will be different.
```javascript
const arr1 = ['JSAN', 'FEB', 'MAR', 'APR', 'MAY'];
let arr2;
(function() {
   arr2 = [...arr1];
   arr1[0] = 'potato'
})();
console.log(arr2);
```
--------------------------------------------------------------
###  Destructuring Assignment:
#### Use  Destructuring Assignment to Assign variables from objects:
This is a special syntax for neatly assigning values taken directly from an object to a variable.
```javascript
const AVG_TEMPERATURES = {
   today: 77.5,
   tomorrow: 79
};

function getTempOfTmrw(avgTemperatures) {
   "use strict"

   const { tomorrow : temOfTomorrow } = avgTemperatures;

   return temOfTomorrow
}

console.log(getTempOfTmrw(AVG_TEMPERATURES));
```
#### Destructuring Assignment with Nested Objects:
We can also use destructuring assignment to assign variables from nested objects.
```javascript
const LOCAL_FORECAST = {
      today: { min: 72, max: 83 }
      tomorrow: { min: 73.3, max: 54.6 }
};

function getMAxOfTmrw(forecast) {
   "use strict";

   const { tomorrow : { max : maxOfTomorrow }} = forecast;

   return maxOfTomorrow;
}
console.log(getMaxOfTmrw(LOCAL_FORECAST));
```
--------------------------------------------------------------
