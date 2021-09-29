### <**Login** /> and <**Auth** />

### Why is the Context API useful?

The React Context API is a way for a React app to effectively produce global variables that can be passed around. This is the alternative to "prop drilling" or moving props from grandparent to child to parent, and so on. Context is also touted as an easier, lighter approach to state management using Redux.


### What are some common use cases for using the Context API

Some sample use cases where the Context API proves helpful are: Theming — Pass down app theme. i18n — Pass down translation messages. Authentication — Pass down current authenticated user


### Describe “Context Hell”

Like the callback hell, usual when jQuery was used for everything, the React Context hell is the nasty code you get taking advantage of the React Context API

----------------------

### Terms:

**global state:** 
pass data through the component tree without having to pass props down manually at every level, managing state in multiple components that are not directly connected


**provider:**
The <**Provider**> component makes the Redux store available to any nested components that need to access the Redux store. Since any React component in a React Redux app can be connected to the store

**consumer:**
The Consumer component allows a React component to subscribe to the context changes. The component makes the data available using a render prop
