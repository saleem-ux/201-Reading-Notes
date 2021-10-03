# Read: Class 36 : Application State with Redux

![img](https://miro.medium.com/max/1838/1*fcbWaGi9QCNYa5DoUYmERw.png)

## Review, Research, and Discussion

### What are the advantages of storing tokens in “Cookies” vs “Local Storage”

* #### Cookies are automatically saved, sent and removed by the browser. The frontend developer does not have to worry about implementing this part, nor is there any scope of a mistake from the frontend side. This is not true for localstorage


* #### for API calls to the server, they will only get the session tokens if they are using cookies – localstorage will not work" 


* #### The objective here is that the user should use the same session when navigating to different subdomains of a site. This can be easily done via cookies by setting the cookie domain as “.yoursite.com”. This is not easily possible to do via localstorage since the store is not shared across domains / subdomains.

### Explain 3rd party cookies :

#### A third-party cookie is placed on a website by someone other than the owner (a third party) and collects user data for the third party. As with standard cookies, third-party cookies are placed so that a site can remember something about the user at a later time. Third-party cookies, however, are often set by advertising networks that a site may subscribe to in the hopes of driving up sales or page hits


### How do pixel tags work?

* #### It’s a 1×1-pixel graphic used for tracking user behavior, site conversions, web traffic, and other metrics at a site’s server level. In other words, it is a tiny pixel-sized image, usually hidden, embedded in everything, from banner ads to emails.

* #### You add the tracking pixel using a code in your site’s HTML code or email, which contains an external link to the pixel server. When someone visits your website, the HTML code is processed by their browser, which follows the link and opens the hidden graphic. This action is identified and recorded in the server’s log files. This method allows for different information about the visitor to be transmitted


## Document the following Vocabulary Terms

* #### cookies: Cookies are small pieces of data stored as text on the client's computer. Normally cookies are used only to store small amounts of data, including user preferences, time and more. Even though cookies are not harmful some people do not permit cookies due to concerns about their privacy.its used to identify your computer as you use a computer network. Data stored in a cookie is created by the server upon your connection. This data is labeled with an ID unique to you and your computer.

* #### authorization: Authorization is the process of giving someone permission to do or have something. and its a security mechanism to determine access levels or user/client privileges related to system resources including files, services, computer programs, data and application features.

* #### access control: Access control is a security technique that regulates who or what can view or use resources in a computing environment.

* #### conditional rendering: Conditional rendering is a term to describe the ability to render different user interface (UI) markup if a condition is true or false. In React, it allows us to render different elements or components based on a condition


## Preparation Materials 
### Redux


* #### Redux is a pattern and library for managing and updating application state, using events called "actions"

* #### Redux is a predictable state container for JavaScript apps.

* #### It helps you write applications that behave consistently…

* #### Redux provides a solid, stable, and mature solution to managing state in your React application

* #### transform your application from a total mess of confusing and scattered state, into a delightfully organized, easy to understand modern JavaScript powerhouse.

```
One application state object managed by one store
```
### Why use Redux?

* #### Redux allows you to manage your app’s state in a single place and keep changes in your app more predictable and traceable. It makes it easier to reason about changes occurring in your app.

### how to use Redux in react

1. create store as we create context
2. pass store and context to provider
3. imported as context exactly

### How Redux works

* #### There is a central store that holds the entire state of the application. Each component can access the stored state without having to send down props from one component to another.

* #### There are three building parts: actions, store, and reducers

### An action creator
is a function that creates and returns an action object. We typically use these so we don't have to write the action object by hand every time:

### A reducer
is a function that receives the current state and an action object, decides how to update the state if necessary, and | returns the new state: (state, action) => newState. 


## Resources

* [worlds easiest guide to redux](https://medium.freecodecamp.org/understanding-redux-the-worlds-easiest-guide-to-beginning-redux-c695f45546f6)
* [testing reducers](https://medium.com/@netxm/testing-redux-reducers-with-jest-6653abbfe3e1)
* [Redux Docs](https://redux.js.org/)