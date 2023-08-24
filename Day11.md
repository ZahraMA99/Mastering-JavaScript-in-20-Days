## Deep JavaScript Foudation - V3
## Introduction:tokyo_tower::rainbow:

- LEARN THE DNA OF JAVASCRIPT & ALGORITHEMS.:performing_arts:
```js
// ex
let x = 40;
x++; // x = 41 
++x;  // 41 => x = x + 1
```
> 💌Note: Evrey thing inside JS is an object? Evereh thing can bevhave as an object.

## Types:tokyo_tower:
### Primitive Types:
1. undefined: means dosen't currently hava a value.
2. string
3. number
4. boolean
5. object
6. symbol
7. bigInt (future): let i = 22n
> 💌 Note: function & arrays are a subtype of a object type.

- Objects::thumbsup:
1. object 
2. function
3. array 

- Not Object::thumbsdown:
1. undefined
2. string
3. number
4. boolean
5. object
6. symbol 
7. null => It is one of JavaScript's primitive values and is treated as falsy for boolean operations. *in the begining of js they defined null as object.*
8. bigint => values represent numeric values which are too large to be represented by the number primitive.

> 💌 Note:
> In JavaScript: variables don't have types, values do.

#### typeof : operator returns a string indicating the type of the operand's value.

> 💌 Notes:
>- function and arrays aren't types of the top level they are sub types of object. when using `typeof(array)`: return(object), while `typeof(function)`: return(function).
>- `typeof(null)`: return(object). *it is a bug in JS, ih they want to correct it a lot of things will fail in the JS*

#### Nan::rainbow:
- *(Special Values)* values that not equall to it self.
- `typeof(NaN)`: return(number).

#### isNan()::rainbow:
- Evaluate any argument to number then cheak weather it's a Nan or not.

```js
Number.isNan()

isNaN("ahmad")          // true
Number.isNaN("ali")   // false
```

#### Object.is( , ):rainbow:
- it’s built in cheaker.

#### better way for cheaking equality === :rainbow:

```js
// we might use -0 for directons in some applecaions which the sign means direct.
 
-0 === 0                // true
Object.is(-0 ,0 )       // false
```

>💌 Note:
=== failed in Nan & -0

```js
console.log(Object.is("42",42) === false);
console.log(Object.is("foo","bar") === false);
console.log(Object.is(false,true) === false);
console.log(Object.is(null,undefined) === false);
console.log(Object.is(undefined,null) === false);

console.log(Object.is(42,42) === true);
console.log(Object.is("foo","foo") === true);
console.log(Object.is(false,false) === true);
console.log(Object.is(null,null) === true);

console.log(Object.is(-0,0) === false);
console.log(Object.is(0,-0) === false);
console.log(Object.is(0,NaN) === false);
console.log(Object.is(NaN,0) === false);
console.log(Object.is(42,"42") === false);

console.log(Object.is(undefined,undefined) === true);
console.log(Object.is(NaN,NaN) === true);
console.log(Object.is(-0,-0) === true);
console.log(Object.is(0,0) === true);
```

## Coercion :rainbow:
- type conversion

### Abstract Operations: ToPrimitive:rainbow:
- **.toString ()**:rainbow:
```js
(null).toString()                  // "null"
undefined.toString()               // "undefined"
true.toString()                    // "true"
false.toString()                   // "false"
3.14159.toString()                 // "3.14159"
(0).toString()                     // "0"
(-0).toString()                    // "0"

([]).toString()                    // ""
[1, 2, 3].toString()               // "1,2,3"
[null, undefined].toString()       // ","
[[[], [], []], []].toString()      // ",,,"
([,,,,]).toString()                // ",,,"

{}      "[object Object]"
{a:2}   "[object Object]"
```

- **ToNumber**:rainbow:
```js
// using Number(x)

""        // 0
"0"       // 0
"-0"      // -0
" 009 "   // 9
"3.14159" // 3.14159
"0."      // 0
".0"      // 0
"."       // NaN
"0xaf"    // 175 // consvert hexacecimal to decimal

false      // 0
true       // 1
null       // 0
undefined  // Nan

[""]        // 0
["0"]       // 0
["-0"]      // 0-
[null]      // 0
[undefined] // 0
[1,2,3]     // NaN
[[[[]]]]    // 0
{ .. }      // NaN
```

#### Why true & false shouldn’t convert to 1&0 ??:rainbow:
```js
3 > 2 > 1
(true) > 1
1 > 1 // false !!!!
```
- **ToBoolean()**:rainbow:
// Falsy values:
```js
“”
0, -0
null
NaN
false
undefined
// anything eles will be truthy value
```
#### Cases of coercion::rainbow: 
```js
// string concatination calls toString method
"ali" + 20

`lol ${variable}`
// also use toString

`lol ${variable.toString()}
// impicit `coercion, primitve types don't have methods

// all of the above are implicit
// explicit 
String(variable)
```
## Delieverables⚙️
**- **<br/>
🎃Excersie Link: <br/>
💡My Solution: <br/>
```js


```
