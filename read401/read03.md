## Express REST API

### 1. Name 3 real world use cases where you’d want to change the request with custom middleware
application server middleware, message-oriented middleware, web middleware

### 2. True or false: The route handler is middleware?
false , they are not middleware functions by definition. If such function is used on routing methods then they are only handler functions. We use such a handler function which is not a middleware when it is the only one callback function.

 Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle. The next function is a function in the Express router which, when invoked, executes the middleware succeeding the current middleware

### 3. In what ways can a middleware function end the process and send data to the browser?
create a middleware function called “requestTime” and add a property called requestTime to the request object.

When you make a request to the root of the app, the app now displays the timestamp of your request in the browser.

### 4. At what point in the request lifecycle can you “inject” middleware?
the request object can be injected into middleware by passing the Request parameter into the constructor 

### 5. What can cause express to error with “Request headers sent twice, cannot start a second response”

when a server tries to send more than one response to a client. What this means is that for a given client request the server previously sent a response (either a success responsei with the resource requested or error response for a bad request) back to the client and now is unexpectedly trying to send another response

-------------------------------- 

**Middleware:** functions are functions that have access to the request object (req), the response object (res), and the next function in the application’s request-response cycle. The next function is a function in the Express router which, when invoked, executes the middleware succeeding the current middleware.

**Request Object:** is the main entry point for an application to issue a request to the Library - all operations on a URL must use a Request object. The request object is application independent in that both servers and clients use the same Request class.

**Response Object:** One of the most important objects in ASP is the Response object. It is the object which communicates between the server and the output which is sent to the client.

**Application Middleware:** Bind application-level middleware to an instance of the app object by using the app.use() and app.METHOD() functions, where METHOD is the HTTP method of the request that the middleware function handles (such as GET, PUT, or POST) in lowercase.

**Routing Middleware:** Router-level middleware works in the same way as application-level middleware, except it is bound to an instance of express.Router().

**Test Driven Development:** (TDD) is a software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing the software against all test cases. This is as opposed to software being developed first and test cases created later.

**Behavioral Testing:** is a testing of the external behaviour of the program, also known as black box testing. It is usually a functional testing.
