# Introduction:flags:
- JavaScript is a dynamic programming language that's primarly used for web development and make websites interactive.
- JavaScript used to modify and interact with HTML.
- It was created in 1995.
- where we can run js:
   1. On the Browsers: Console.
   2. Servers using projects called: Node.js. 
   3. Embedded devices.

# DOM (Document Object Model):boom:
- DOM represents a document with a logical tree,Each branch of the tree ends in a node, and each node contains objects. DOM methods allow programmatic access to the tree.  
- We can access several elements in the tree using DOM methods and change the document's structure, style, or content, for example:
     1. `document.title`: It returns the title of the page.
     2. `document.body`: It returns the body of the document.
     3. `document.body.children`: It returns a group of elements that's entire the body like: div, header.. 
     4. `document.getElementById("id")`: It returns a specific element that has this id.
     5. `document.querySelector("#id")`: It returns a specific element that has this css selector (#id), the same of the above point.
     6. `document.getElementsByTagName("h1")`: It returns all the elements with the same tag.
     7. `document.querySelectorAll("h1")`: Same of the above but using css selector.
     8. `document.getElementsByClassName("player")`: It returns element with the same class name.
     9. `document.querySelectorAll(".player")`: Same of the above but using css selector.
     10. `document.getElementsByClassName("player").length`: It Finds the nubmer of elements with specific class name.
     11. `document.querySelectorAll(".player").length`: Same of the above but using css selector.
     12. `document.getElementById("p1-name")`: To get the text of element with this of id.


 - Editing the DOM with JS: 
      1. `document.getElementById("player").textContent = ossy"`: It will set the content of the element to the new value "ossy".
      2. `document.getElementById("player").append(" & sofia")"`: Player content will be ossy & sofia.
      3. `document.title = "my page"`: A new title for the page.
         
>💌 Note:<br/> 
>querySelector: this method returns the first element while querySelectorAll: this method returns a NodeList containing all elements that match the specified selector.

# Delieverables⚙️
**- Compound Assignment With Augmented Multiplication**
<br />:jack_o_lantern:Excersie Link: https://tinyurl.com/yck2kavm
<br />💡My Solution: 
```js
let a = 5;
let b = 12;
let c = 4.6;

// Only change code below this line
a *= 5;
b *= 3;
c *= 10
```
**- Concatenating Strings with the Plus Equals Operator**
<br />:jack_o_lantern:Excersie Link: https://tinyurl.com/3h8jzw4b
<br />💡My Solution: 
```js
let myStr = "This is the first sentence.";
myStr += " This is the second sentence.";
```
**- Use Bracket Notation to Find the Nth-to-Last Character in a String**
<br />:jack_o_lantern:Excersie Link: https://tinyurl.com/bdztyv7n
<br />💡My Solution: 
```js
// Setup
const lastName = "Lovelace";

// Only change code below this line
const secondToLastLetterOfLastName = lastName[lastName.length - 2] ; // Change this line
```
