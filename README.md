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

## Data Types & Variables :
### Data Types:

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
myVar--
```

----------------------------------

### Finding a Remainder :

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

### Creat a string in JavaScript :

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