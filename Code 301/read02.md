## Things I want to know more about

## React lifecycle 

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’? 

- the render

2. What is the very first thing to happen in the lifecycle of React? 

- constructor

3. Put the following things in the order that they happen: 

- constructor
- render 
- React Updates
- componentDidMount 
- componentWillUnmount 

4. What does componentDidMount do?

This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in componentWillUnmount()

## React State Vs Props 

1. What types of things can you pass in the props?
- We pass props as an argument it can be strings or numbers.


2. What is the big difference between props and state?
- props: you pass into component (props handled outside of component  )
- state: is handled inside that component and you can updated inside the component


3. When do we re-render our application?
- when we change the state inside of the app or change the props outside the component.


4. What are some examples of things that we could store in state?

- input element and checkbox
