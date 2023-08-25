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

 
