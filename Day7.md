## Introduction :tulip:

### JavaScript principles::fire:
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
> We could generalize our function - So we pass in our specific instruction only when we run the mother function (big/first function).

### How was passing function in onther function possiable :question::exclamation:
**Function in javascript = first class object<br/>**
They can co-exist and can be treated like any other javascript object:<br/>
    - Assigned to variables and properties of other objects.
    - Passed an arguments into functions.
    - Returned as values from functions. 
    
    


