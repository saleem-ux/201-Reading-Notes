# Event Driven Applications
**Why is access control important?**  
limit access to information and information processing systems. When implemented effectively, they mitigate the risk of information being accessed without the appropriate authorization, unlawfully and the risk of a data breach.   


**Describe an application that would need access control**   

any market , education website , bank website ....

**What is a role used for?**   
to give some roles access to do things not given to others

**Why is role based access control more scalable than discretionary or mandatory access control?**  

because it can given and restricted easier than other type access control

##  Vocabulary   

| voc                               | related to |
|-------------------------------------|--------------|
|Authorization |is a security mechanism to determine access levels or user/client privileges related to system resources including files, services, computer programs, data and application features.|
|Role Based Access Control|is an approach to restricting system access to authorized users.|
|Capabilities| is a communicable, unforgeable token of authority. It refers to a value that references an object along with an associated set of access rights. |
|



## Preview  


*Which 3 things had you heard about previously and now have better clarity on?*  
- sql
- authorization and authentication


*Which 3 things are you hoping to learn more about in the upcoming lecture/demo?*  
- testing xD


*What are you most excited about trying to implement or see how it works?*  
- as well as our topic next week is events, so events

&nbsp;

## Preparation Materials

> Event Driven Programming     
- Event-Driven Programming in Node.js  
is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.  


- Event-Driven Programming makes use of the following concepts:  

1. An Event Handler is a callback function that will be called when an event is triggered.
2. A Main Loop listens for event triggers and calls the associated event handler for that event.



**EventEmitter**   
module that allows us to get started incorporating Event-Driven Programming in our project right away.

**Removing Listeners**   
To remove event listeners in EventEmitter we can use the `removeListener` or `removeAllListeners` method.   





&nbsp;

&nbsp;

> Node docs: events   

- Events   
All objects that emit events are instances of the EventEmitter class. These objects expose an eventEmitter.on() function that allows one or more functions to be attached to named events emitted by the object.   
 

 - When the EventEmitter object emits an event, all of the functions attached to that specific event are called synchronously. Any values returned by the called listeners are ignored and discarded.   

 - The standard this keyword is intentionally set to reference the EventEmitter instance to which the listener is attached. `but` when using arrow function, the this keyword will no longer reference the EventEmitter instance   to which the listener is attached

 - The EventEmitter calls all listeners synchronously in the order in which they were registered. but can switch to an asynchronous mode of operation using the `setImmediate()` or `process.nextTick()` methods   

 - When a listener is registered using the `eventEmitter.on() `method, that listener is invoked every time the named event is emitted.   

 - Error events  
  If an EventEmitter does not have at least one listener registered for the 'error' event, and an 'error' event is emitted, the error is thrown, a stack trace is printed, and the Node.js proce 