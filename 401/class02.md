# Express

---


## What’s the difference between PUT and PATCH?

- **PUT**: Is a method of modifying resource where the client sends data that updates the entire resource. It is used to set an entity’s information completely

- **PATCH**: Applies a partial update to the resource. This means that you are only required to send the data that you want to update, and it won’t affect or change anything else. 


---

## Provide links to 3 services or tools that allow you to “mock” an API for development like json-server

1. [Nock](https://github.com/nock/nock)
2. [Canned](https://github.com/sideshowcoder/canned)
3. [Dyson](https://npmjs.org/package/dyson)

----

## Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?

- Swagger 


        '200':
          description: OK
        '400':
          description: Bad request. User ID must be an integer and larger than 0.
        '401':
          description: Authorization information is missing or invalid.
        '404':
          description: A user with the specified ID was not found.
        '5XX':
          description: Unexpected error


- APIDoc.js 1

        '200':
        	Successful request and response.
        '400':
        	Malformed parameters or other bad request.



---

## Compare and contrast SOAP and REST

-**SOAP provides the following advantages when compared to REST**:

• Language, platform, and transport independent (REST requires use of HTTP)

•    Works well in distributed enterprise environments (REST assumes direct point-to-point communication)

•    Standardized

•    Provides significant pre-build extensibility in the form of the WS* standards

•    Built-in error handling

•    Automation when used with certain language products


-**REST is easier to use for the most part and is more flexible. It has the following advantages over SOAP**:

•    No expensive tools require to interact with the web service
•    Smaller learning curve
•    Efficient (SOAP uses XML for all messages, REST can use smaller message formats)
•    Fast (no extensive processing required)
•    Closer to other web technologies in design philosophy

---

**Document the following Vocabulary Terms**

Term | Meaning
-------- | ------------
Web Server | On the hardware side, a web server is a computer that stores web server software and a website's component files.  On the software side, a web server includes several parts that control how web users access hosted files
Express | It is a web framework written in JS and hosted by node.js
Routing | is the mechanism by which requests (as specified by a URL and HTTP method) are routed to the code that handles them.
WRRC | Web Request Response Cycle