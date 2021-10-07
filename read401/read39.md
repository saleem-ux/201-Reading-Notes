## Redux - Additional Topics


### What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application

The most 'redux-like' way of handling the pre-loading of data would be to fire off the asynchronous action in the lifecycle method (probably componentWillMount ) of a Higher Order Component that wraps your app

### When using a thunk/async action that dispatches the actual action, which do you export from your reducer?

we export the action and its payload.

------------------------------

### Terms: 

**middleware:**
Middleware allows for side effects to be run without blocking state updates. We can run side effects (like API requests) in response to a specific action, or in response to every action that is dispatched (like logging)

**thunk:**
is a programming concept where a function is used to delay the evaluation/calculation of an operation.

--------------------------

## Redux Toolkit

The Redux Toolkit package is intended to be the standard way to write Redux logic. 
It was originally created to help address three common concerns about Redux:

* "Configuring a Redux store is too complicated"
* "I have to add a lot of packages to get Redux to do anything useful"
* "Redux requires too much boilerplate code"

