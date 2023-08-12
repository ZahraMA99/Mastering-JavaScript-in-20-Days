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






