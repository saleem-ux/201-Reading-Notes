## Things I want to know more about
## React Docs - thinking in React
### How would you break a mock into a component heirarchy?
- The first thing you’ll want to do is to draw boxes around every component in the mock and give them all names. Use the same techniques for deciding if you should create a new function or object.

### What is the single responsibility principle and how does it apply to components?
- single responsibility principle technique, that is, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller sub-components.

is a computer-programming principle that states that every module, class or function in a computer program should have responsibility over a single part of that program's functionality, and it should encapsulate that part.

### What does it mean to build a ‘static’ version of your application?
- build a version that takes your data model and renders the UI but has no interactivity.

### Once you have a static application, what do you need to add?
- We need to Identify The Minimal Representation Of UI State.

### What are the three questions you can ask to determine if something is state?
- Is it passed in from a parent via props? If so, it probably isn’t state.
Does it remain unchanged over time? If so, it probably isn’t state.
Can you compute it based on any other state or props in your component? If so, it isn’t state.
### How can you identify where state needs to live?
-Identify every component that renders something based on that state.
Find a common owner component (a single component above all the components that need the state in the hierarchy).
Either the common owner or another component higher up in the hierarchy should own the state.
If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.