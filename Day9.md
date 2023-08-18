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
> Accessing Twitter’s server to get new tweets that takes a long time <br/>
> Code we want to run using those tweets <br/>
> Challenge: We want to wait for the tweets to be stored in tweets so that they’re there to run displayTweets on - but no code can run in the meantime <br/>
