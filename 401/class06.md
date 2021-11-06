# Authentication

---

## Explain what a “Singleton” is (in Computer Science terms)

- It is a design pattern limits the number of instances of a particular object to just one. Where this single instance is called the singleton.

---

## Explain how the Singleton pattern can be used with Node modules, specifically with classes

- **example**


        - The getInstance method is Singleton's gatekeeper. It returns the one and only instance of the object while maintaining a private reference to it which is not accessible to the outside world.

        - The getInstance method demonstates another design pattern called Lazy Load. Lazy Load checks if an instance has already been created; if not, it creates one and stores it for future reference. All subsequent calls will receive the stored instance. Lazy loading is a CPU and memory saving technique by creating objects only when absolutely necessary.

        class Singleton {
            constructor (){
                this.instance = "";
            }

            createInstance() {
                let createdInstace = "I am the instance";
                return createdInstace;
            }

            
            getInstance() {
                if (!instance) {
                        instance = this.createInstance();
                    }
                return instance;
                }
         
        };

        function run() {

            let instance1 = Singleton.getInstance();
            let instance2 = Singleton.getInstance();

            console.log("Same instance? " + (instance1 === instance2));
        };

        run(); // Same instance? true


---

## If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?

1. follow the best code structure by separating the files.

2. write all of the middle wares in middleware file and each middle ware should has its own js file.

3. export the middle wares and import them were the CRUD operations called.

4. use the imported middle wares as a global or local middle ware to check for all CRUD operations when it is happening.

---

## Document the following Vocabulary Terms

- **Router Middleware**: It is the middle ware that holds all of CRUD methods and uses the Route to manage the procces.

- **Dynamic Module Loading**: it is loading a module into memory, retrieve the addresses of functions and variables contained in the module, execute those functions or access those variables, and unload the module from memory.

- **Singleton Pattern**: It is a design pattern limits the number of instances of a particular object to just one. Where this single instance is called the singleton.

- **CRUD -> REST Method Matches**: create, read, update and delete. they are the four basic operations of persistent storage.

- **Mock Testing**: is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules.


--- 

## Preparation Materials

**Securing Passwords with Bcrypt Hashing Function**

- We all know storing passwords in clear text in your database is not secure. Many desktop applications and almost every web service including, blogs, forums eventually need to store a collection of user data and the passwords, that has to be stored using a hashing algorithm. Cryptographic hash algorithms MD5, SHA1, SHA256, SHA512, SHA-3 are general purpose hash functions, designed to calculate a digest of huge amounts of data in as short a time as possible. Hashing is the greatest way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.

**Basic access authentication**

- is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request.

- Protocol: 

    1. Server side:

        When the server wants the user agent to authenticate itself towards the server after receiving an unauthenticated request, it must send a response with a HTTP 401 Unauthorized status line and a WWW-Authenticate header field.

        The WWW-Authenticate header field for basic authentication is constructed as following:

        `WWW-Authenticate: Basic realm="User Visible Realm"`

        The server may choose to include the charset parameter from RFC 7617:

        `WWW-Authenticate: Basic realm="User Visible Realm", charset="UTF-8"`



    2. Client side: 

    When the user agent wants to send authentication credentials to the server, it may use the Authorization header field.

    The Authorization header field is constructed as follows:

    1. The username and password are combined with a single colon (:). This means that the username itself cannot contain a colon.
    
    2. The resulting string is encoded into an octet sequence. The character set to use for this encoding is by default unspecified, as long as it is compatible with US-ASCII, but the server may suggest use of UTF-8 by sending the charset parameter.
    
    3. The resulting string is encoded using a variant of Base64 (+/ and with padding).
    
    4. The authorization method and a space (e.g. "Basic ") is then prepended to the encoded string.



**Authentication**

-  is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.

- Session Management: is a process by which a server maintains the state of an entity interacting with it. This is required for a server to remember how to react to subsequent requests throughout a transaction. Sessions are maintained on the server by a session identifier which can be passed back and forward between the client and server when transmitting and receiving requests. Sessions should be unique per user and computationally very difficult to predict.