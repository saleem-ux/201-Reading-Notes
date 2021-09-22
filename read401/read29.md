# Read: Class 29 : Advanced State with Reducers

![img](https://camo.githubusercontent.com/39edc655449f6262a9a7be81b38da2a83896b55c8c1b146a8922ae1804ccbe91/68747470733a2f2f7265732e636c6f7564696e6172792e636f6d2f64676576653764616f2f696d6167652f75706c6f61642f76313538303636353932322f5573655f526564756365725f536964655f4566666563745f44656d6f2e706e67)

# Review, Research, and Discussion

## How can we ensure that an effect hook runs only once?

#### If we pass an empty array [] , it just renders the component only once like componentDidMount

## Can useState() update more than one state variable at the same time?

#### You could combine the state into one state object and then you could do one setState call and there will only be one render. Unlike the setState in class components, the setState returned from useState doesn't merge objects with existing state, it replaces the object entirely

```

  const [form, setState] = useState({
    username: '',
    password: ''
  });

```

## Is useState() synchronous?

#### useState and setState both are asynchronous. Even though they are asynchronous, the useState and setState functions do not return promises. Therefore we cannot attach a then handler to it or use async/await to get the updated state values

# Document the following Vocabulary Terms

#### State Hook The useState() is a Hook that allows you to have state variables in functional components , it takes the initial state as an argument and returns an array of two entries

#### Component Lifecycle the series of methods that are invoked in different stages of the component’s existence. The three phases are: Mounting, Updating, and Unmounting

# Preparation Materials

## useReducer Hook

* #### "useReducer is one of the additional Hooks that shipped with React 16.8. An alternative to the useState Hook, it helps you manage complex state logic in React applications"

* #### "useReducer is used to store and update states, just like the useState Hook. It accepts a reducer function as its first parameter and the initial state as the second"

* #### "useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks"

* #### "There are two different ways to initialize useReducer state. You may choose either one depending on the use case. The simplest way is to pass the initial state as a second argument, You can also create the initial state lazily. To do this, you can pass an init function as the third argument. The initial state will be set to init(initialArg)"

* #### There are three main building blocks in Redux

1. A store — an immutable object that holds the applications state data
2. A reducer — a function that returns some state data, triggered by an action type
3. An action — an object that tells the reducer how to change the state. It must contain a type property, and it can contain an optional payload property.

## The reducer function

* #### "The reduce() method in JavaScript executes a reducer function on each element of the array an and then returns a single value. The reduce() method accepts a reducer function, which itself can accept up to four arguments"

* #### "The reducer function itself accepts two parameters and returns one value. The first parameter is the current state, and the second is the action. The state is the data we are manipulating. The reducer function receives an action, which is executed by a dispatch function"

## Preview

### Which 3 things had you heard about previously and now have better clarity on?

#### usestate , useeffect , functional components

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

#### Hooks , DOM

### What are you most excited about trying to implement or see how it works?

#### using functional components with hooks , instead of building classes

## Resources

* [useReducer hook](https://reactjs.org/docs/hooks-reference.html#usereducer)
* [Ultimate Guide to useReducer](https://blog.logrocket.com/guide-to-react-usereducer-hook/)
