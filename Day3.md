## Arrays :bug:
**The Array object** enables storing a collection of multiple items under a single variable name, and has members for performing common array operations.

**Array Methods:**
- .length : represents the number of elements in that array.
- .pop() : removes the last element from an array and returns that element.
- .push() : adds the specified elements to the end of an array and returns the new length of the array.
- .join() : method is used to join all the elements of an array into a single string, we can separate them by a separator.
- .toString() : converts an array to a string.
- .shift() : removes the first element from an array and returns that removed element.
- .unshift() : adds the specified elements to the beginning of an array and returns the new length of the array.
- .delete() : removes a property from an object.
- .concat() : merge two or more arrays and returns the new array. 
- .flat() : creates a new array with all sub-array elements concatenated into it recursively up to the specified depth.
- .splice() : removing or replacing existing elements and/or adding new elements.
- .slice() : returns a shallow copy of a portion of an array into a new array object selected from start to end.
- .sort() : sorting an array.


**Mutable and Immutable data:**:cactus: 
- Mutable: data can be edited. (e.g. Arrays)
- Immutable: data always stays the same. (e.g. Strings & other primitives) => If you have the choice keep thing immutable.

>💌 Note:
WHEN WE USE IMMUTABLE VARIABLE WITH MUTABLE VALUE LIKE ARRAY! (e.g below)
<br/> WE HAVE TO DISTINGUISH BETWEEN THE IMMUTABILITY OF CONST VARIABLES AND THE MUTABILITY OF VALUES THAT WE ASSIGN TO THEM. SO IT'S POSSIABLE TO HAVE AN IMMUTABLE REFERANCE, IMMUTABLE ARROW :arrow_right: A MUTABLE VALUE.<BR/> WE MEAN ARRAY ITSELF HASN'T CHANGED "ARRAY NAME STILL A POINTER TO THE [ ] ITSELF", BUT THE VALUES INSIDE THE ARRAY CAN BE CHANGABLE "WE CAN STILL MESS WITH IT".

  ```js
   const operands = [4,5];
   const sum = operands[0] + operands[1];
   operands[0] = 6;
   const newSum = operands[0] + operands[1];
   Result: 11.
   //The default for array is const unlees you have a good reson to use let.
  ```


## Objects :pushpin:
**Object** type represents one of JavaScript's data types. It is used to store various keyed collections and more complex entities.

- Built-In Objects:
  1. document
  2. console
  3. Math
  4. String
 
 💌 Note:<br/>
EVERYTHING IN JS IS AN OBJECT!! OBJECTS, ARRAYS.. EXPECT PRIMITIVE DATA TYPE LIKE STRING, BOOLEAN, NUMBERS..

#### Spread operator:
> Another huge advantage of the spread operator is the ability to combine arrays, or to insert all the elements of one array into another, at any index. With more traditional syntaxes, we can concatenate arrays, but this only allows us to combine arrays at the end of one, and at the start of another. Spread syntax makes the following operation extremely simple: code example:

> It used with:<br/>
> Spread Operator with Arrays:<br/>
> Spread Operator with objects:<br/>
> Spread Operator with functions:<br/>
 
```js
let thisArray = ['sage', 'rosemary', 'parsley', 'thyme'];

let thatArray = ['basil', 'cilantro', ...thisArray, 'coriander'];
```

### Quiz Project :cyclone:
```js
<!DOCTYPE html>
<!-- saved from url=(0063)https://anjana.dev/javascript-first-steps/2-jsquiz-starter.html -->
<html lang="en-US">
  <head>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />

    <title>Quiz.js</title>
    <style>
      body {
        margin: 1rem auto;
        padding: 3rem;
        font-family: sans-serif;
      }
      header {
        width: 50%;
        margin: 1em auto;
      }
      main {
        min-width: 25rem;
        max-width: 50%;
        margin: 0px auto;
        display: flex;
        flex-direction: column;
      }
      #statement {
        border: 1px solid black;
        border-radius: 0.5rem;
        box-shadow: 5px 5px 5px gray;
        padding: 1rem;
        font-size: x-large;
        text-align: center;
        margin: 1rem 0px;
        min-height: 2em;
      }
      #explanation {
        padding: 1rem;
        text-align: center;
      }
      #options {
        width: 100%;
        display: flex;
        flex-direction: column;
      }
      button {
        padding: 0.5rem;
        font-size: medium;
        border-radius: 5px;
      }
      .correct {
        background-color: lightgreen;
      }
      .incorrect {
        background-color: lightpink;
      }
    </style>
    <style type="text/css" id="operaUserStyle"></style>
  </head>
  <body>
    <header>
      <h1>Quiz.js</h1>
      <p>Do you know JS? Find out!</p>
    </header>

    <main>
      <div id="statement"></div>

      <div id="options">
        <button name="true" value="true">true</button>
        <button name="false" value="false">false</button>
      </div>

      <div id="explanation"></div>
    </main>

    <script type="text/javascript">
      // TODO 1: Declare & assign variables pointing to the corresponding element(s)
      // statement should be the "statement" div
      const statement = document.getElementById("statement");
      // optionButtons should be all the elements within the "options" div
      const optionButtons = document.querySelector("#options").children;
      // explanation should be the "explanation" div
      const explanation = document.getElementById("explanation");

      // TODO 2: Declare & assign a variable called fact
      // Its value should be an object with a statement, true/false answer, and explanation
      const fact = {
        statement: "Arrays are just like objects",
        correctAnswer: true,
        explanation: "Arrays are kind of objects with special character.",
      };

      // TODO 3: Set the text of the statement element to the fact's statement
      statement.textContent = fact.statement;

      // TODO 4: Declare disable & enable functions to set or remove the "disabled" attribute from a given button element
      // disable(button) should set the button element's attribute "disabled" to the value ""
      const disable = (button) => {
        button.setAttribute("disabled", "");
      };
      // enable(button) should remove the attribute "disabled" from the button element
      const enable = (button) => {
        button.removeAttribute("disabled");
      };

      // TODO 5: Declare an isCorrect function that compares a guess to the right answer
      // isCorrect(guess) should return true if the guess matches the fact's answer
      const isCorrect = (guess) => {
        return guess === fact.answer.toString();
      };

      // TODO 6A: Use a for loop to add a click event listener to each of the optionButtons
      for (let ob of optionButtons) {
        ob.addEventListener("click", (event) => {
          // TODO 6B: Within the event handler function, display the fact's explanation by setting the text of the explanation element
          explanation.textContent = fact.explanation;

          // TODO 7: Within the event handler function,
          // Use a for loop to disable all the option buttons
          for (let allB of optionButtons) disable(allB);
          // TODO 8: Within the event handler function,
          // Get the guessed value from the clicked button
          // Use a conditional to compare the guess to the fact's answer
          // and add the "correct"/"incorrect" class as appropriate
          if (isCorrect(ob.value)) {
            ob.classList.add("correct");
          } else {
            ob.classList.add("incorrect");
          }
        });
      }
    </script>
  </body>
</html>
```
## Delieverables⚙️
**- Copy Array Items Using slice()**<br/>
🎃Excersie Link: https://shorturl.at/mxC68 <br/>
💡My Solution:<br/>
```js
function forecast(arr) {
  // Only change code below this line
  arr = arr.slice(2,4)
  return arr;
}

// Only change code above this line
console.log(forecast(['cold', 'rainy', 'warm', 'sunny', 'cool', 'thunderstorms']));
```

**- Combine Arrays with the Spread Operator**<br/>
🎃Excersie Link: https://shorturl.at/fpPT1 <br/>
💡My Solution:<br/>
```js
function spreadOut() {
  let fragment = ['to', 'code'];
  let sentence = ['learning', ...fragment , 'is', 'fun'];
  return sentence;
}

console.log(spreadOut());
```
**- Profile Lookup **<br/>
🎃Excersie Link: https://shorturl.at/bkPZ5 <br/>
💡My Solution:<br/>
```js
// Setup
const contacts = [
  {
    firstName: "Akira",
    lastName: "Laine",
    number: "0543236543",
    likes: ["Pizza", "Coding", "Brownie Points"],
  },
  {
    firstName: "Harry",
    lastName: "Potter",
    number: "0994372684",
    likes: ["Hogwarts", "Magic", "Hagrid"],
  },
  {
    firstName: "Sherlock",
    lastName: "Holmes",
    number: "0487345643",
    likes: ["Intriguing Cases", "Violin"],
  },
  {
    firstName: "Kristian",
    lastName: "Vos",
    number: "unknown",
    likes: ["JavaScript", "Gaming", "Foxes"],
  },
];

function lookUpProfile(name, prop) {
   for(let i in contacts){
    if(contacts[i].firstName == name){
      return contacts[i].lastName;
    }
   
  }
}

console.log(lookUpProfile("Kristian", "lastName"));
```


