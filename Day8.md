## Clousure :closed_lock_with_key:

#### Generalizing functions::milky_way:
- ‘Parameters’ (placeholders) mean we don’t need to decide what data to run our functionality on until we run the function.
- Then provide an actual value (‘argument’) when we run the function Higher order functions follow this same principle.
- We may not want to decide exactly what some of our functionality is until we run our function.

#### Pairing up::milky_way:
- I know what a variable is
- I've created a function before
- I've added a CSS style before
- I have implemented a sort algorithm (bubble, merge etc)
- I can add a method to an object’s prototype
- I understand the event loop in JavaScript
- I understand 'callback functions'
- I can implement filter
- I can handle collisions in a hash table<br/>

💌 **Note:**
> For each topic you know give yourself a point to get a total out of.

#### Anonymous and arrow functions::milky_way:
- Improve immediate legibility of the code.
- But at least for our purposes here they are ‘syntactic sugar’ - we’ll see their full effects later.
- Understanding how they’re working under-the-hood is vital to avoid confusion.

#### Clousre:hibiscus:
- Clousre is the most esotenic of javascript concepts.
- Enables powerful pro-level functions like 'once' and 'memoize'.
- Many JavaScript design patterns including the moddul pattern use clousre.
- Build iterators, handle partial application and maintain state an asynchronous world.

💌 **Note: Concept of clouser scope**
> JavaScript is a static or lexically scoped language.<br/>
> Lexical means the physical positioning on the page. ( in the last e.g on telegrame => I phisically position incremnet counter inside the running of the outer ).<br/>
> JavaScript is a lexical staticlly scope language. ( That means even i retuerned my function out, and theoritcally all this data should have been deleted, Nope! becaues I have this fundamental rule of lexical scoped language! I'll want to grap all that data behind the scenes and put it in the backpack "red bag :joy:"!!<br/>
> Such that when I run the function, I still have all the data from when I last scope. => Not because I go back into the earlier excution context !!! Becuse I pulled the data from when the function incrementCounter was born out with me on my lexical scop property.<br/>
> Behind the scense I pulled the data out and left it attached to my new function. <br/>

#### Functions with memories::milky_way:
- When our functions get called, we create a live store of data (local memory/variable environment/state) for that function’s execution context.
- When the function finishes executing, its local memory is deleted (except the returned value)
- But what if our functions could hold on to live data between executions?
- This would let our function definitions have an associated cache/persistent memory
- But it all starts with us returning a function from another function

#### The bond::milky_way:
- When a function is defined, it gets a bond to the surrounding Local Memory (“Variable Environment”) in which it has been defined.

#### The ‘backpack’::milky_way:
- We return incrementCounter’s code (function definition) out of outer int global and give it a new name - myNewFunction.
- We maintain the bond to outer’s live local memory - it gets ‘returned out’ attached on the back of incrementCounter’s function definition.
- So outer’s local memory is now stored attached to myNewFunction - even though outer’s execution context is long gone.
- When we run myNewFunction in global, it will first look in its own local memory first (as we’d expect), but then in myNewFunction’s ‘backpack’.

#### What can we call this ‘backpack’?:milky_way:
- Closed over ‘Variable Environment’ (C.O.V.E.)
- Persistent Lexical Scope Referenced Data (P.L.S.R.D.)
- ‘Backpack’
- ‘Closure’
  <br/>
💌 **Note:**
> The ‘backpack’ (or ‘closure’) of live data is attached incrementCounter (then to myNewFunction) through a hidden property known as [[scope]] which persists when the inner function is returned out.

#### Individual backpacks::milky_way:
- If we run 'outer' again and store the returned 'incrementCounter' function definition in 'anotherFunction', this new incrementCounter function was created in a new execution context and therefore has a brand new independent backpack.

#### Closure gives our functions persistent memories and entirely new toolkit for writing professional code::milky_way:
- Helper functions: Everyday professional helper functions like ‘once’ and ‘memoize’
- Iterators and generators: Which use lexical scoping and closure to achieve the most contemporary patterns for handling data in JavaScript
- Module pattern: Preserve state for the life of an application without polluting the global namespace
- Asynchronous JavaScript: Callbacks and Promises rely on closure to persist state in an asynchronous environment


## Delieverables⚙️
