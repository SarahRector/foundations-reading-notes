
# JavaScript Asynchronous Programming and Callbacks
https://flaviocopes.com/javascript-callbacks/

* computers do things asynchronously but JavaScript is synchronous by default - code cannot run in parallel
    * the browser provides an environment where we can mess with asychronous code

* we define an event handler that accepts a function that will be called when the event is triggered creating a *callback*

* callbacks add nesting which gets real complicated real quick

# Understanding JavaScript Promises
https://flaviocopes.com/javascript-promises/

* a promise is a proxy for a value that will eventually become available
    * once a promise is called it starts in *pending state*
    * the caller function waits for it to either return the promise in *resolved state* or in *rejected state* but the function continues its execution while the promise does it's work
    ```js
        let done = true

        const isItDoneYet = new Promise((resolve, reject) => {
        if (done) {
            const workDone = 'Here is the thing I built'
            resolve(workDone)
        } else {
            const why = 'Still working on something else'
            reject(why)
        }
        })
    ```
* promises can also be chained and used to catch errors

# MDN Asynchronous JavaScript
https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous

* lists lots of guides for working with async JS
* Intro
    * web APIs now run async code
    * but we don't know how long it will take to get a response and so we need our code to wait until there is a response
    * can use callbacks or promises
        * fetch() 
            * it takes the URL of a resource you want to fetch from the api and returns a promise

* Graceful Asynchronous Programming with Promises
    * an object that represents an intermediate state of an operation
    * callbacks can do something similar but get real complicated real quick
    * promises also let us do more advanced error handling by using ```.catch()```

    # MDN Using Promises
    https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Using_promises

    * Unlike old-fashioned passed-in callbacks, a promise comes with some guarantees:

        *  Callbacks will never be called before the completion of the current run of the JavaScript event loop.
    * Callbacks added with then(), as above, will be called even after the success or failure of the asynchronous operation.
    * Multiple callbacks may be added by calling then() several times. Each callback is executed one after another, in the order in which they were inserted.

    * you can also run two or more async operations back to back where each one starts when the last one succedes, with the result from the previous step = a *promise chain*
    ```js
    const promise = doSomething();
    const promise2 = promise.then(successCallback, failureCallback);
    ```

    # JavaScript Promises in Sixteen Minutes
    https://medium.com/quick-code/javascript-promises-in-twenty-minutes-3aac5b65b887

    * this is a great run through of what actually happens in code execution and why promises are necessary

    # JavaScript Promises: An Introduction
    https://web.dev/promises/

    * lots of good code examples expecially on chaining
    * good reference guide at the end

    # MDN Using Fetch
    https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch

    * the promise returned from fetch() wont reject on HTTP error status
    * you can establish cross site session using fetch
    * wont send cookies unless you set credentials init option
    * basic fetch request:
        ```js
        fetch('http://example.com/movies.json')
        .then(response => response.json())
        .then(data => console.log(data));
        ```
    * lots of useful code examples

# That Data looks so fetching on you: Understanding the JS fetch API
https://itnext.io/that-data-looks-so-fetching-on-you-understanding-the-js-fetch-api-880eae0c8d25

* first of all...that title
* fetch() makes a network request to a url and returns a promise
* that promise resolves with a response object when the remote server responds with headers
* to read the response body we have to call a response method on it, like text() or JSON() which will return another promise whose resolve value is the body of the response

