## Context API - Behaviors

### When you have multiple contexts, what component type should you use (class/function) and why?
you can use class component or functional components, in class component it depend on states , but in functional components it based on props

### What are some good use cases for using the Context API for global state?
React global state management with Context API (no Redux)

There are multiple ways to add global state to your React project and each way comes with its own set of strengths & weaknesses. A common, outdated solution to managing global state is a practice known as prop drilling. This involves manually passing in the shared data to each component as props. While this is a simple solution, it is inefficient as components take in props which they have no use for. 

Perhaps the most popular solution, Redux, is a third party state management library. Redux has a lot of support and there are some very useful debugging features which is why major companies like Amazon, Instagram, & Doordash use it.

### How can you best test context?
The best way to test Context is to make our tests unaware of its existence and avoiding mocks. We want to test our components in the same way that developers would use them (behavioral testing) and mimic the way they would run in our applications (integration testing).

---------------------------

### Terms: 

**context:**
Context provides a way to pass data through the component tree without having to pass props down manually at every level.

In a typical React application, data is passed top-down (parent to child) via props, but such usage can be cumbersome for certain types of props (e.g. locale preference, UI theme) that are required by many components within an application. Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.

**useContext():**
“useContext” hook is used to create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level. Context defined will be available to all the child components without involving “props”.

**static context:**
A static method or, block belongs to the class and these will be loaded into the memory along with the class. You can invoke static methods without creating an object. ... But static contexts(methods and blocks) doesn't have any instance they belong to the class.
