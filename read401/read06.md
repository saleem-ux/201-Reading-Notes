#  Authentication 



![img](https://www.researchgate.net/profile/Henning-Klevjer-2/publication/265155465/figure/fig3/AS:669990764154893@1536749654580/Basic-Access-Authentication.png)

# Review, Research, and Discussion

### 1. Explain what a “Singleton” is (in Computer Science terms)

A singleton is a class that allows only a single instance of itself to be created and gives access to that created instance. It contains static variables that can accommodate unique and private instances of itself. It is used in scenarios when a user wants to restrict instantiation of a class to only one object. This is helpful usually when a single object is required to coordinate actions across a system.

The singleton pattern is used in programming languages such as Java and .NET to define a global variable. A single object used across systems remains constant and needs to be defined only once rather than many times.

### 2. Explain how the Singleton pattern can be used with Node modules, specifically with classes
* ### "The singleton pattern is used in programming languages such as Java and .NET to define a global variable. A single object used across systems remains constant and needs to be defined only once rather than many times".

* ### "After we instantiate once, every time we call to instantiate again, it will not create another instance.. instead it will refer to only one instantiation (the first one)".

### Here is an example of singleton http client, which wraps an axios library:



let http = (function () {


  let axios = require('axios')



  return {

    get: function(url) {

      return axios.get(url)

    },

    post: function(url) {

      return axios.post(url)

    }

  }

}())



## If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?

### "The app.get() function is Application-level Middleware. the parameters passed to the method are req, res, and next. These are the incoming request, the response being written, and a method to call to pass the call to the next middleware function once the current middleware is finished. In this case, once the response is sent, the function exits. You could also chain other middleware here by calling the next() method.

# Document the following Vocabulary Terms

|Term||
|-----------------------|--------------------------------------------------|
 Router Middleware|Chainable middleware with familiar req.params and req.query if identical routing is what you are typically used and its works in the same way as application-level middleware, except it is bound to an instance of express.Router().
Dynamic Module Loading|Dynamic loading is a mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory
 Singleton Pattern|the singleton pattern is a software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system. The term comes from the mathematical concept of a singleton.
CRUD -> REST Method Matches| C -> create ,post. R -> retrieve , get. U -> retrieve , get. D -> delete , delete.
Mock Testing|is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules.


# Preparation Materials

## **Securing Passwords with Bcrypt Hashing Function :**


### "Passwords are the first line of defense against cyber criminals. It is the most vital secret of every activity we do over the internet and also a final check to get into any of your user account, whether it is your bank account, email account, shopping cart account or any other account you have".

## **Basic access authentication :

### basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic , where credentials is the Base64 encoding of ID and password joined by a single colon .

# #**OWASP auth cheatsheet :**

* ### "Authentication is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know".

* ### "Session Management is a process by which a server maintains the state of an entity interacting with it. This is required for a server to remember how to react to subsequent requests throughout a transaction".




# Preview

### Which 3 things had you heard about previously and now have better clarity on?

*  CRUD and REST are just about drilled into my head.

### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

* I hope to learn more about how the singleton pattern will be integrated with compartmentalized code.

### What are you most excited about trying to implement or see how it works?

I am enjoying the testing of an application.

## Resuorses :

* [Securing Passwords](https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html)


* [Basic Auth](https://en.wikipedia.org/wiki/Basic_access_authentication)


* [OWASP auth cheatsheet](https://www.owasp.org/index.php/Authentication_Cheat_Sheet)


* [bcrypt docs](https://www.npmjs.com/package/bcrypt)

