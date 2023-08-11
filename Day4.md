## Functions :bomb::zap:
**Functions** is a set of statements that performs a task or calculates a value, it should take some input and return an output.
- Parameters: identifies values that are passed into a function.
- Arguments: is a value (primitive or object) passed as input to a function.
- Return values: specifies the functions output value.

**Arrow Functions** :leftwards_arrow_with_hook:
An arrow function expression is a compact alternative to a traditional function expression, with some semantic differences.
<br/>`Syntax` :microscope:
<br/>Identifier nameOfTheFunction = parameters => what to do

> - Since Arrow function are expressions, we can assign them to a variable.
> - For one parameter functions, parantheses are optional.
> - For multiaple parameters, parantheses are required.
> - If we need to do more than just return a value, we can curly braces for a "norma" function body. In that case we still need return. 

## Events & Handlers :saxophone:
**Add Event Listener** let us listen for events on a DOM element. 
<br/>`Syntax` :microscope:
<br/>addEventListener(type, listener)
<br/>addEventListener(type, listener, options)
> We pass two parameter to the method:
>   1. The name of the event that I care about. (e.g. click, dbclick, mouseover, mouseout..).
>   2. Arrow function becuse we don't really need to name it! it's called a **callback function** || **event handler function**. 
