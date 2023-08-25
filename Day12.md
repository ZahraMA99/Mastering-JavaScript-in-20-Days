## Philosophy of Coercion :notes:
- coercion refers to the process of converting a value from one type to another, usually during the evaluation of expressions or operations. Coercion can be either explicit or implicit.
1. Explicit Coercion: Also known as type casting, explicit coercion involves deliberately converting a value from one type to another using built-in functions or methods. For example:
```js
const numStr = "42";
const num = Number(numStr); // Explicitly coercing the string to a number
```
2. Implicit Coercion: Implicit coercion happens automatically when JavaScript attempts to perform operations on values of different types. JavaScript will try to make sense of the situation and convert the values to a common type before executing the operation. This can sometimes lead to unexpected behavior. For example:
```js
const num = 42;
const numStr = "2";
const result = num + numStr; // JavaScript implicitly coerces the number to a string and performs string concatenation
// result will be "422"
```
> :love_letter:Note<br/>
> It's important to be aware of coercion, especially implicit coercion, as it can lead to code that's difficult to understand and predict. In many cases, it's a good practice to use explicit coercion to ensure that the types are converted as intended and to make the code more readable.

### trim() method: :mushroom:
- is a built-in string method that is used to remove whitespace characters from both the beginning and the end of a string. Whitespace characters include spaces, tabs, and newline characters.

### Validation :mushroom:
*Read from chatGbt*
- Validation involves checking whether data conforms to certain rules, constraints, or expectations before it is used further in the application.

## Equality :notes:
- == checks value (loose)
- === checks value and type (strict)

### double equal algorithem :mushroom: 
*chatGbt* 
> :love_letter:Note <br/>
> Note that the double equal operator performs type coercion, meaning it tries to convert values to the same type before making the comparison. This can lead to unexpected results and is often considered a source of bugs in JavaScript code.

### Summary :mushroom:
1. if the types are the same: ===
2. if null || undefined: equal
3. if non-primitives: toPrimitive
4. Prefer: ToNumber

### Corner Summary: "avoid to use":
1. == with 0 or "" (or even " ")
2. == with non-primitives
3. == true or == false : allow ToBoolean or use ===

> :love_letter:Note
> Knowing types is always better than not knowing them Static Types is not the only (or even necessarily best) way to know your types

> == is not about comparisons with unknown types == is about comparisons with known type(s), optionally where conversions are helpful

> If you know the type(s) in a comparison:
> If both types are the same, == is identical to === Using === would be unnecessary, so prefer the shorter ==

> all the casess explained on the slides on telegram.

## Static Typing :notes:
JavaScript is known for its dynamic typing, where variables are not bound to a specific data type during declaration and can change their data type during runtime. This can lead to flexibility but also sometimes results in unexpected behavior. However, there are ways to introduce static typing in JavaScript using tools and extensions.

### Benefits: 
1. Catch type-related mistakes
2. Communicate type intent
3. Provide IDE feedback
4. validating operand types to avoid errors

## Delieverables⚙️
**- **<br/>
🎃Excersie Link: <br/>
💡My Solution: <br/>
```js


```

### Here are two popular approaches:
1. TypeScript *chatGpt*
2. Flow *chatGpt*


   
