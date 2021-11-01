# Express REST API

---

## Name 3 real world use cases where you’d want to change the request with custom middleware

1. Login and logout.
2. Updating the database.
3. Exposing Public APIs.

---

## True or false: The route handler is middleware?

- False

---

## In what ways can a middleware function end the process and send data to the browser?


- call next() to pass control to the next middleware,
otherwise the request will be left hanging.

- calling res.end, res.send, res.render or any method that implicitely calls res.end.

---

## At what point in the request lifecycle can you “inject” middleware?

- After routing and before the controlles taake an action. 

--- 

## What can cause express to error with “Request headers sent twice, cannot start a second response”

- means that you're already in the Body or Finished state, but some function tried to set a header or statusCode. When you see this error, try to look for anything that tries to send a header after some of the body has already been written. For example, look for callbacks that are accidentally called twice, or any error that happens after the body is sent.


---

## Document the following Vocabulary Terms 

- **Middleware**: is software that provides common services and capabilities to applications outside of what’s offered by the operating system. Data management, application services, messaging, authentication, and API management are all commonly handled by middleware.

- **Request Object**:  is the main entry point for an application to issue a request to the Library - all operations on a URL must use a Request object.

- **Response Object**: it is an object which contains a server's response to an HTTP request. Every HTTP request sent returns a response from the server (the Response object) which includes quite a bit of information.

- **Application Middleware**: the middleware that checks all of requests (global middleware).

- **Routing Middleware**: it is the same of Apllication middle ware except it is bound to an instance of express.Router(), and handles the requests.

- **Test Driven Development**: is a software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing the software against all test cases.

- **Behavioral Testing**: s a testing of the external behaviour of the program, also known as black box testing. It is usually a functional testing.