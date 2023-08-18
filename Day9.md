## Asynchronous JavaScript 🎯

#### Promises, Async & the Event Loop::blossom:
- Promises - the most signficant ES6 feature
- Asynchronicity - the feature that makes dynamic web applications possible
- The event loop - JavaScript’s triage
- Microtask queue, Callback queue and Web Browser features (APIs) <br/>

#### Asynchronicity is the backbone of modern web development in JavaScript yet!:blossom:
**JavaScript is:**
- Single threaded (one command runs at a time).
- Synchronously executed (each line is run in order the code appears).<br/>
> So what if we have a task: <br/>
> - Accessing Twitter’s server to get new tweets that takes a long time <br/>
> - Code we want to run using those tweets <br/>
> - Challenge: We want to wait for the tweets to be stored in tweets so that they’re there to run displayTweets on - but no code can run in the meantime <br/>

### JavaScript is not enough - We need new pieces (some of which aren’t JavaScript at all):first_quarter_moon:💎
*Our core JavaScript engine has 3 main parts:*:blossom:
- Thread of execution
- Memory/variable environment
- Call stack <br/>

*We need to add some new components::blossom:*
- Web Browser APIs/Node background APIs
- Promises
- Event loop, Callback/Task queue and micro task queue <br/>

> Code Example on setTimeOut() and callback Queue::bomb:
```
We’re interacting with a world outside of JavaScript now - so we need rules:
function printHello(){ console.log("Hello"); }
function blockFor1Sec(){ //blocks in the JavaScript thread for
1 sec }
setTimeout(printHello,0);
blockFor1Sec()
console.log("Me first!");

=> console: Me first! Hello
```
#### ES5 Web Browser APIs with callback functions::bomb:
#### Problems ☄️
- Our response data is only available in the callback function - Callback hell
- Maybe it feels a little odd to think of passing a function into another function only for it
to run much later
#### Benefits :hibiscus:
- Super explicit once you understand how it works under-the-hood

### ES6+ Solution (Promises):ribbon:
*Using two-pronged ‘facade’ functions that both:<br/>*
- Initiate background web browser work and
- Return a placeholder object (promise) immediately in JavaScript

> ES6+ Promises code example::crown:
```
function display(data){
 console.log(data)
}
const futureData = fetch('https://twitter.com/will/tweets/1')
futureData.then(display);

console.log("Me first!");
```

### ES6+ Solution (Promises)
- Special objects built into JavaScript that get returned immediately when we make a call to a web browser API/feature (e.g.fetch) that’s set up to return promises (not all are).
- Promises act as a placeholder for the data we expect to get back from the web browser feature’s background work.

### then method and functionality to call on completion
- Any code we want to run on the returned data must also be saved on the promise object
- Added using .then method to the hidden property ‘onFulfilment’
- Promise objects will automatically trigger the attached function to run (with its input being the returned data

### Promises
### Problems☄️
- 99% of developers have no idea how they’re working under the hood
- Debugging becomes super-hard as a result
- Developers fail technical interviews
### Benefits :hibiscus:
- Cleaner readable style with pseudo-synchronous style code
- Nice error handling process<br/>

## We have rules for the execution of our asynchronously delayed code💎
> Hold promise-deferred functions in a microtask queue and callback function in a task queue (Callback queue) when the Web Browser Feature (API) finishes Add the function to the Call stack (i.e. run the function) when:
 - Call stack is empty & all global code run (Have the Event Loop check this condition).
 - Prioritize functions in the microtask queue over the Callback queue.

## Promises, Web APIs, the Callback & Microtask Queues and Event loop enable:💎
> - **Non-blocking applications:** This means we don’t have to wait in the single thread and don’t block further code from running 
> - **However long it takes:** We cannot predict when our Browser feature’s work will finish so we let JS handle automatically running the function on its completion 
> - **Web applications:** Asynchronous JavaScript is the backbone of the modern web - letting us build fast ‘non-blocking’ applications 

## Delieverables⚙️
