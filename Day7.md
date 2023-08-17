## Introduction :tulip:

### JavaScript principles::tulip:
*When JavaScript code runs, it: <br/>*
- Goes through the code line-by-line and run/excutes aech line **Known as thread of excutions**.
- Saves data like strings and arrays so we can use that data later - in it's memory. We can even save code 'functions'.
- **Functions:** Code we save() ('define') functions & can use (call/invoke/execute/run) later with the function's name & {}.
- **Excution context:** Created to run the code of a function - has 2 parts (we've already seen them!):
    1. Tread of execution.
    2. Memory.
       
- **Call stack:**:fire::fire:
    1. JavaScript keeps track of what function is currently running. (wheres the thread of excution)
    2. Run a function - add to call stack.
    3. Finish running the function - JS removes it from call stack.
    4. Whatever is top of the call stack " thats the function we're currently running.
  
 ## Functions & Callbacks :tulip:
 ### Why we use functions::fire:
- DRY principle: Don't Repeat Yourself.
- Generalizing functions: parameters means we don't need to decide what data to run our functionality on until we run the code.
- Then provide an actual value ('arguments') when we run the function.
- Higher order functions follow this principle.
- We may not want to decide exactly what some of our functionality is unti we run our function.

>💌 Note:<br/>
> We could generalize our function - So we pass in our specific instruction only when we run the higher order function (outerfunction).

### How was passing function in onther function possiable :question::exclamation:
**Function in javascript = first class object<br/>**
They can co-exist and can be treated like any other javascript object:<br/>
1. Assigned to variables and properties of other objects. ( Methods ) => defin the function for object property called method. 
2. Passed an arguments into functions. 
3. Returned as values from functions. 
    
#### Which is our Higher Order Function::bell:
- The Outer function that takes in a function is our higher-order function.
#### Which is our Callback Function::bell:
- Function we insert inside the outer function is our callback function. 

>💌 Note:<br/>
> **Higher function (outer function) & Callback function simplify our code & make it DRY.**

> *Declartive readable code:* Map, filter, reduce - the most readable way to write code to work with data.<br/>
> *Codesmith & pro interview prep:* One of the most popular topics to test in interview both for Codesmith and Mid/senior level.<br/>
> *Asynchronous JavaScript:* Callbacks are a core aspect of async JavaScripts, and are under-the-hood of promises, async/wait.<br/>
 
> **Outer function called map. becuase it has some mapping functionality & create new collection of data.** 

#### Anonymous and arrow functions:💎
- Improve immediate legibility of the code.
- But at least for our purposes here they are 'syntactic sugar' we'll see their full effects later.
- Understanding how they're working under-the-hood is vital to avoid confusion.

## Delieverables⚙️

