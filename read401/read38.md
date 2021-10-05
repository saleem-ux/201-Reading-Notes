## Redux - Asynchronous Actions

### Redux Middleware and Side Effects

By itself, a Redux store doesn't know anything about async logic. It only knows how to synchronously dispatch actions, update the state by calling the root reducer function, and notify the UI that something has changed. Any asynchronicity has to happen outside the store.

Redux reducers must never contain "side effects".
A **"side effect"** is any change to state or behavior that can be seen outside of returning a value from a function.

* Some common kinds of side effects are things like:

 - Logging a value to the console
 - Saving a file
 - Setting an async timer
 - Making an AJAX HTTP request
 - Modifying some state that exists outside of a function, or mutating arguments to a function

However, any real app will need to do these kinds of things somewhere. So, if we can't put side effects in reducers, where can we put them?

**Redux middleware were designed to enable writing logic that has side effects.**

Middleware also have access to dispatch and getState. That means you could write some async logic in a middleware, and still have the ability to interact with the Redux store by dispatching actions.

### Redux Async Data Flow
So how do middleware and async logic affect the overall data flow of a Redux app?

Just like with a normal action, we first need to handle a user event in the application, such as a click on a button. Then, we call dispatch(), and pass in something, whether it be a plain action object, a function, or some other value that a middleware can look for.

Once that dispatched value reaches a middleware, it can make an async call, and then dispatch a real action object when the async call completes.

### Using the Redux Thunk Middleware
As it turns out, Redux already has an official version of that **"async function middleware"**, called the **Redux "Thunk" middleware**.

The thunk middleware allows us to write functions that get dispatch and getState as arguments. The thunk functions can have any async logic we want inside, and that logic can dispatch actions and read the store state as needed.

**Thunk** is a programming concept where a function is used to delay the evaluation/calculation of an operation.

**Redux Thunk**
middleware libraries that allow for side effects and asynchronous actions, is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store’s dispatch method, which is then used to dispatch regular synchronous actions inside the function’s body once the asynchronous operations have been completed.