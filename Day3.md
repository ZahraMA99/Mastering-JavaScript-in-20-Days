## Arrays :bug:
**The Array object** enables storing a collection of multiple items under a single variable name, and has members for performing common array operations.

**Array Methods:**
- .length : represents the number of elements in that array.
- .pop() : removes the last element from an array and returns that element.
- .push() : adds the specified elements to the end of an array and returns the new length of the array.
- .join() : returns a new string by concatenating all of the elements in this array, separated by commas or a specified separator string.
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
- Immutable: data always stays the same. (e.g. Strings & other primitives)

 💌 Note:
WHEN WE USE IMMUTABLE VARIABLE WITH MUTABLE VALUE LIKE ARRAY! (e.g below)
<br/> WE HAVE TO DISTINGUISH BETWEEN THE IMMUTABILITY OF CONST VARIABLES AND THE MUTABILITY OF VALUES THAT WE ASSIGN TO THEM. SO IT'S POSSIABLE TO HAVE AN IMMUTABLE REFERANCE, IMMUTABLE ARROW :arrow_right: A MUTABLE VALUE.<BR/> WE MEAN ARRAY ITSELF HASN'T CHANGED "ARRAY NAME STILL A POINTER TO THE [] ITSELF", BUT THE VALUES INSIDE THE ARRAY CAN BE CHANGABLE "WE CAN STILL MESS WITH IT". 
```
 const operands = [4,5];
 const sum = operands[0] + operands[1];
 operands[0] = 6;
 const newSum = operands[0] + operands[1];
 Result: 11.

