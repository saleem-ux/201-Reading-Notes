# Read: Class 37 : Redux - Combined Reducers

## Review, Research, and Discussion

![img](https://www.theconsolelogs.com/react/redux-flow.webp)

#### Why choose Redux instead of the Context API for global state?
If you are using Redux only to avoid passing props down to deeply nested components, then you could replace Redux with the Context API. It is exactly intended for this use case. On the other hand, if you are using Redux for everything else (having a predictable state container, handling your application's logic outside of your components, centralizing your application's state, using Redux DevTools to track when, where, why, and how your application's state changed, or using plugins such as Redux Form, Redux Saga, Redux Undo, Redux Persist, Redux Logger, etc…), then there is absolutely no reason for you to abandon Redux. The Context API doesn't provide any of this.

## What is the purpose of a reducer?

#### In Redux, a reducer is a pure function that takes an action and the previous state of the application and returns the new state. The action describes what happened and it is the reducer's job to return the new state based on that action.

## What does an action contain?

#### an object that have type and paylod

## Why do we need to copy the state in a reducer? 

#### to avoid losing existing data

## Document the following Vocabulary Terms

* #### immutable state :(unchangeable state) state cannot be modified after it is created. React state should be treated as immutable.

* #### time travel in redux :Time travel is the ability to move back and forth among the previous states of an application and view the results in real time. With Redux, given a specific state and a specific action, the next state of the application is always exactly the same.

* #### action creator: An action creator is merely a function that returns an action object. Redux includes a utility function called bindActionCreators for binding one or more action creators to the store's dispatch() function.

* #### reducer:  A reducer is a function that determines changes to an application's state.

* #### dispatch : dispatch() is the method used to dispatch actions and trigger state changes to the store. react-redux is simply trying to give you convenient access to it


## Preparation Materials  

### **combineReducers**

* #### As your app grows more complex, you'll want to split your reducing function into separate functions, each managing independent parts of the state. The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.

* #### The resulting reducer calls every child reducer, and gathers their results into a single state object. The state produced by combineReducers() namespaces the states of each reducer under their keys as passed to combineReducers()

* #### You may call combineReducers at any level of the reducer hierarchy. It doesn't have to happen at the top. In fact you may use it again to split the child reducers that get too complicated into independent grandchildren, and so on.


### There are several important ideas to be aware of when using combineReducers :

1. First and foremost, combineReducers is simply a utility function to simplify the most common use case when writing Redux reducers. You are not required to use it in your own application, and it does not handle every possible scenario.

2. While Redux itself is not opinionated about how your state is organized, combineReducers enforces several rules to help users avoid common errors.

3. One frequently asked question is whether Redux "calls all reducers" when dispatching an action. Since there really is only one root reducer function, the default answer is "no, it does not". However, combineReducers has specific behavior that does work that way.

4. You can use it at all levels of your reducer structure, not just to create the root reducer. It's very common to have multiple combined reducers in various places, which are composed together to create the root reducer.

## Resources

* [Multiple Reducers Example](https://www.youtube.com/watch?v=gBER4Or86hE)
* [Redux Docs: Using Combined Reducers](https://redux.js.org/recipes/structuring-reducers/using-combinereducers/)
* [Redux Docs: Combined Reducer Syntax](https://redux.js.org/api/combinereducers/)