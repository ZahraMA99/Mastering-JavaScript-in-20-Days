## Data Fetching & Promisies :golf::traffic_light:
API Fetch:

- **Promises:**:sparkles:
<br/>Object represents the eventual completion or failure of an asynchronous operation and its resulting value "represent a value that we don’t have yet".
-  Promises can be in 3 possible states:
    1. `Pending`: still waiting for the value, hang tight.
    2. `Fulfilled(aka"resolved")`: finally got the value, all done.
    3. `Rejected`: sorry could't get the value, all done.<br/>
=> It takes time for promises to resolve, so they are "asynchronous".

:sparkles:Are promisies only use with api calls or will we sim them in another usage?<br/> yes, we will see them in other different cases. Fetch is one example of an operation or a function that returns a promise. 

- **await:**:sparkles:
<br/>await lets us tell JS to stop and wait for an asynchronous operation to finish.
```
let response = await fetch("https://dog.ceo/api/breed/hound/list");
console.log(response);
```

- **.json():**:sparkles:
<br/>representing structured data based on JavaScript object syntax (It's body contains the data we care about).
> 💌 Note: **Json() is async function**

## Destructuring Data:sweat_drops:
- Destructuring is a fancy way of declaring multiple variables at once By "extracting" values from an object with their property names.
```
const spices = [{name:"Sarah", nickname:"queen"}]
let {name, nickname} = spices[0];
```
- With arrays:
```
const [one, tow ] = [1,2]

// We can ignore the values in the array we don't need
const [,,melB] = spices;

// We can use ... to collect remaining values
 const [babySpice, ...adultSpices] = spices;
```
🎃**Execise:**
```
/*
	In your Doggo Fetch file, follow TODO 2 to complete the getBreedFromURL 
	function with destructuring
	
	The string method .split() will be useful it returns an array of substrings
	 by splitting a string at a certain character: 
*/
let part = "https://images.dog.ceo/breeds/poodle-standard/n02113799_2280.jpg"
         .split("/") // parts of url
let name =  part[4] // the name
let removed = name.split("-")
let joinedName = removed.join(" ")
let finalName = joinedName.trim() // to remove the white spaces if the name just one word
```
## Async:notes:
- `.createElement()`: In an HTML document, the document.createElement() method creates the HTML element specified by tagName.
```
const button = document.createElement("button")
```
- `.appendChild()`: The appendChild() method of the Node interface adds a node to the end of the list of children of a specified parent node.
```
options.appendChild(button)
```
## Modules :earth_africa:
- Modules let us split big codebases across multiple files.
```
  <script type="module">
    //...
</script>

// JS modules work differently from JS scripts
```
- Module scope: We can't access variables and function in the web console.

## Debugging :seedling:
- We can console.log() (or .warn() or .error()) is one way to understand what's happening when your program runs.
```
function whyIsntThisWorking(input) {
    console.log("Well at least we got this far");
    console.log(input);
    return thingThatDoesntWork(input);
}
```
- You can also use the browser's debugger to pause JS and inspect what's happening.
```
function whyIsntThisWorking(input) {
    debugger;
    return thingThatDoesntWork(input);
}
```
- The debugger statement creates a breakpoint where JS will pause and let you look around.
> 💌 Notes:<br/>
> 1. `.trim()` method removes whitespace from both ends of a string and returns a new string, without modifying the original string.<br/>
> 2. In JS we can creat any element we want to appeare in HTML page.

## Delieverables⚙️

