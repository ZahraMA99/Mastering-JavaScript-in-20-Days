## Scope :earth_americas:
**JavaScript organizes scopes with functions and blocks**<br/>

### Befor executing the code : 
scope maneger detrmine the scope
then bring data or store it in the variable

> :email: Note:
> Shadowing: Having two varibles with same name in different scopes.

### Auto Globale:
- if I try to use varible in cuurent scope without declaring it, it will be delared in the globale scope
```js
function f1 (){
    name = "ahmad"
    console.log(name)
}
h() //ahmad
```

### Disable it => Strict
```js
function f1 (){
   name = "ahmad"
    console.log(name)
}
h() // erorr
```
## Scope & Function Expressions :earth_americas:
**Named Function Expressions: Benefits** <br/>
1. Reliable function self-reference (recursion, etc)
2. More debuggable stack traces
3. More self-documenting code

### Functional Programming
> :email: Note:
> Functional programming is a good habit. It keeps your code easy to manage, and saves you from sneaky bugs.

### undefiend VS undeclared
- undefined: variables is decleared but still not has a value.
- undeclared: variable not declear yet.
### function expression vs function decleration: 
- Function Declaration: A function declaration is a way to define a named function using the function keyword. It's important to note that function declarations are hoisted, which means they are moved to the top of their scope during the compilation phase. This allows you to use the function before its actual declaration in the code.
```js
function sayHello(name) {
  console.log(`Hello, ${name}!`);
}

```
- Function Expression: A function expression defines a function as part of an expression. It involves assigning an anonymous function (a function without a name) to a variable. Function expressions are not hoisted in the same way as function declarations. They can only be used after they have been defined.
```js
const sayHello = function(name) {
  console.log(`Hello, ${name}!`);
};
```
### Naming Function Expressions:
- Naming function expressions can be helpful for improving code readability, stack traces, and debugging. While function expressions are often used anonymously (without a name), providing a name for a function expression can have its advantages.

Here's how you can name a function expression:
```js
const namedFuncExpr = function myNamedFunction(param) {
  console.log(param);
};
namedFuncExpr("Hello, world!"); // Calling the named function expression
```
> :email:Note:
> In the example above, the function expression is assigned to the variable namedFuncExpr, and it's named as myNamedFunction. This is useful when debugging because the function ill appear with the name myNamedFunction in stack traces, making it easier to identify.

#### Advantages of Naming Function Expressions::
1. Debugging: Named function expressions provide a meaningful name in stack traces, making it easier to identify the function that caused an error.
2. Self-Reference: Named function expressions can reference themselves within their own scope. This is useful for creating self-contained recursive functions.
3. Readability: A named function expression can make the code more self-explanatory by giving context to what the function does.

> :email:Note:
> However, it's important to note that the name you provide to the function expression is only accessible within its own scope. Outside of that scope, the name won't be defined. This can help avoid naming conflicts.

> :email:Note:
> While naming function expressions can have advantages, you should weigh these benefits against your code style and the potential for naming conflicts. If you choose to name function expressions, make sure the names you use are meaningful and provide useful information about the purpose of the function.

### Function Types Hierarchy:
1. (Named) Function Declaration
2. Named Function Expression
3. Anonymous Function Expression
   
## Delieverables⚙️
**- **<br/>
🎃Excersie Link: <br/>
💡My Solution: <br/>
```js


```
