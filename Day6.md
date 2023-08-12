## Data Fetching & Promisies :golf::traffic_light:
API Fetch:

**Promises:**🍄
<br/>Object represents the eventual completion or failure of an asynchronous operation and its resulting value "represent a value that we don’t have yet".
-  Promises can be in 3 possible states:
    1. `Pending`: still waiting for the value, hang tight.
    2. `Fulfilled(aka"resolved")`: finally got the value, all done.
    3. `Rejected`: sorry could't get the value, all done.<br/>
=> It takes time for promises to resolve, so they are "asynchronous".

:sparkles:Are promisies only use with api calls or will we sim them in another usage?<br/> yes, we will see them in other different cases. Fetch is one example of an operation or a function that returns a promise. 

**await:**🍄
<br/>await lets us tell JS to stop and wait for an asynchronous operation to finish.
```
let response = await fetch("https://dog.ceo/api/breed/hound/list");
console.log(response);
```

**.json():**🍄
<br/>representing structured data based on JavaScript object syntax (It's body contains the data we care about).
> 💌 Note: **Json() is async function**

## Destructuring Data:sweat_drops:








