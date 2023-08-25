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


## Delieverables⚙️
**- **<br/>
🎃Excersie Link: <br/>
💡My Solution: <br/>
```js


```
