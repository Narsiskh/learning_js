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
#### Global Scope & Functions:
Scope refers to the visibility of variables. Variables which are defined outside of a function block have global scope. Global Scope means they ca be seen everywhere in your JS code.