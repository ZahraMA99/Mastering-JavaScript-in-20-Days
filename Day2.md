## Values & Data Types :sweat_drops:
**JS has two type of data:**
- Primitive data types:
1. String
2. number
3. boolean
4. undefind
5. null
       
- Reference Data Types:
1. Object: Represents a collection of key-value pairs, where values can be of any data type.
2. Array: Represents an ordered list of values, indexed by integers. For example: [1, 2, 3].
3. Function: Represents a block of reusable code. In JavaScript, functions are first-class citizens,<br/>
       which means they can be assigned to variables, passed as arguments, and returned from other functions.
4. Date: Represents dates and times.
5. Map: Represents a collection of key-value pairs where the keys can be of any data type.
6. Set: Represents a collection of unique values.
  
💡 We can use The `typeof` operator that returns a string indicating the type of the operand's value! e.g:
 1. `typeof("sofia")` returns String.
 2. `typeof(42)` returns number.
 3. `typeof(null)` returns object. "Sometimes js does stuff that we don't expect.:sweat_smile:"
 4. `typeof(document.title)` returns String.
 5. `typeof(undefiend)` returns undefined.

:ab: **Srings:**
- Length of String:
`.length` property used to know how many characters in the string. 
(e.g):
<br/>`"sofia".length` returns 5.
<br/>`"some string".length` returns 4.
<br/>`" ".length` returns 1. "space is character".

- Index of String:
<br/>`"sofia"[2]` returns "f".
<br/>`"sofia".indexOf("f")` returns 2.
<br/>`"aloha".indexOf("a")` returns 0. "It take the first appearnce of the charachter."
<br/>`"sofia".indexOf("z")` returns -1. "convention in js🚩! if characters not exist in the string, `indexof` will return -1".
<br/>`"sofia".indexOf("fia")` returns 2.
<br/>`"sofia".indexOf("lol")` returns -1. 

- Includes:
<br/>`"sofia".includes("f")` returns `true`.
<br/>`"sofia".includes("lol")` returns `false`.

- Starts with:
<br/>`"sofia".startsWith("s")` returns `true`.
<br/>`"sofia".startsWith("lol")` returns `false`.

  ⚙️ **Exercises:**
   ```
    // Add your last name in the players listing.
        document.getElementById("p1-name").append(" Vakil")
    // Retrieve the first "T" in the page title.
        document.title returns "JavaScripTacToe"
        document.title.indexOf("T") returns 10
    // Answer whether the page title contains the string "JavaScript"
        document.title.includes("javaScript") returns "false
    // Capitalize the heading "Tic Tac Toe"
        document.querySelector("header h1").style.transform = "uppercase" returns TIC TAC TOE. 
<br/>
💌 Note:
    <br/>JS CAN MANIPULATE THE HTML AND CSS OF THE PAGE


## Operators :sweat_drops:
✨ **Arthimitic Operators:**
- Plus sign (+) 
<br/>It used for several uses:
    1. Adding numbers: (e.g: 1 + 4).
    2. Concatenating strings: (e.g: "sofia" + "ali") || (e.g: "sofia" + 2). "both sides or one side at least must be string".
- Subtract sign (-)
    1. Subtract numbers: (e.g: 8 - 4).
- Multiple sign (*)
    1. multiplicate numbers: (e.g: 2 * 4).
- Division sign (/)
    1. divide numbers: (e.g: 5 / 5).
- Reminder sign (%)
    1. Reminde numbers: (e.g: 5 % 5).
  
✨ **Comparision Operators:**
- Greater than (>)
- Less than (<)
- Greater than or equal to (>=)
- Less than or equal to (<=)

✨ **Equality Operators:**
-  ( == ) => compares just the value.
-  ( === ) => compares value and type.
-  ( !== ) => checks whether its two operands are not equal.

## Expressions :sweat_drops:
**Declaring VS assigning**:v:
- Declaring: is to define a new variable without a value.
- Assigning: is to set a value to the variable.

**Var vs Let vs Const** :dolphin:

| Var | Let | Const |
| ----| ----| ----- |
| functional scope | block scope | block scope |
| It can be updated and re-declared | It can be updated but cannot be re-declared | It cannot be updated or re-declared |
| It can be declared without initialization | It can be declared without initialization | It cannot be declared without initialization |
| It can be accessed without initialization as its default value is “undefined” | It cannot be accessed without initialization otherwise it will give ‘referenceError’ | It cannot be accessed without initialization, as it cannot be declared without initialization |
| hoisting done, with initializing as ‘default’ value | Hoisting is done, but not initialized | Hoisting is done, but not initialized |

**Statement VS Expression**:v:
- Statement: A statement is a unit of code that performs an action or has an effect. Statements are used to control the flow of execution, perform assignments, call functions, and more.
- Expression: An expression is a piece of code that produces a value when executed. 

### Key Differences:
#### Purpose:
- Statements are primarily used to control program flow, perform actions, and create reusable code blocks (functions).
- Expressions are used to compute values and are often used as parts of statements.

#### Result:
- Statements do not produce values.
- Expressions produce values.

#### Semicolon:
- Statements are usually terminated by a semicolon.
- Expressions do not require a semicolon at the end, though they can be part of statements that do.

#### Nesting:
- Statements can contain expressions.
- Expressions can be nested within other expressions.
#### Examples:
- In JavaScript, an assignment statement is x = 10;, where x = 10 is an expression that assigns the value 10 to the variable x.

## Delieverables⚙️
**QUESTION #1**<br/>
🎃 Consider the following JavaScript code:
```
let a = 0;
let b = "0";
let c = false;
let d = "false";

console.log(a == b);
console.log(b === c);
console.log(!!d);
```
💡 Solution:<br/>
1. true: becuse == will compare just the value not the datatype.
2. false: becuse === will compare the both value and datatype.
3. true: because ! will cast string into true because its not empty and then to false. then the second ! will get true.<br/>

**QUESTION #2**<br/>
🎃Consider the following JavaScript expression:
```
console.log(4 + 5 * "7");
```
What will be the output of this expression? You MUST explain the steps of evaluation taken by JS.<br/>
💡 Solution:<br/>
Output = 39. because initially string "7" will cast into number = 7. then multiplication operator take the high priority so 5 * 7 = 35, 35 + 4 = 39.<br/>

**QUESTION #3**<br/>
🎃 Evaluate the following expression:
```
let result = 5 + 2 * 3 - 1;
```
What will be the output of this expression? You MUST explain the steps of evaluation taken by JS.<br/>
💡 Solution:<br/>
Output = 10. priority for * so 2 * 3 = 6, then 6 + 5 = 11 - 1 = 10 || 6 - 1 = 5 + 5 = 10.<br/>

**QUESTION #4**<br/>
🎃 Consider the following code:
```
let x = 10;
let y = '10';
console.log(x == y);
console.log(x === y);
```
What will be the output of each console.log statement? You MUST explain WHY.<br/>
💡 Solution:<br/>
1. true: becuse == will compare just the value not the datatype.
2. false: becuse === will compare the both value and datatype.<br/>

**QUESTION #5**<br/>
🎃 Given the code below:
```
let num = "15";
let isPositive = true;
let result = (num > 10 && isPositive) || num < 0;
console.log(result);
```
What is the value of result? You MUST explain the steps of evaluation taken by JS<br/>
💡 Solution:<br/>
True. "15" will cast into 15. 15 > 10 => true, true && true => true. true || false = true. in OR case there's no need to check  the secnd part of the statment when the first part is true. 
