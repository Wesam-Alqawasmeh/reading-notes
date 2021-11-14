# Event Driven Applications

---

**Why is access control important?**

- To regulate who can view or use any given resource in the website and the database.

**Describe an application that would need access control**

- E-learning application: the student (regular user) can view part of the content and do the assignments just. on the other hand the teacher (admin user) can view all of the content and the users and their roles, and the accessability publish the assignments and grade the students.

**What is a role used for?**

- To assign the user accessability.

**Why is role based access control more scalable than discretionary or mandatory access control?**

- Because it takes more of a real world approach to structuring access control. Access under RBAC is based on a user's job function within the organization to which the computer system belongs. Essentially, RBAC assigns permissions to particular roles in an organization.

---

## Document the following Vocabulary Terms

- **Authorization**: It is the process of giving someone the ability to access a resource.
- **Role Based Access Control**: (RBAC) it is a popular mechanism to enforce authorization in applications. When using RBAC, an application developer defines roles rather than authorizing individual users or groups.
- **Capabilities**: They are the operations that can the user do depending on the user role.

---

## Event Driven Programming

- Every time you interact with a webpage through it’s user interface, an event is happening. When you click a button a click event is triggered. When you press a key a keydown event is triggered. These events have associated functions that, when triggered, are executed to make a change to the user interface in some way.

**Event-Driven Programming makes use of the following concepts**

- An Event Handler: is a callback function that will be called when an event is triggered.
- A Main Loop listens for event triggers and calls the associated event handler for that event.

**EventEmitter**

- Node.js natively provides us with a useful module called EventEmitter that allows us to get started incorporating Event-Driven Programming in our project right away.

- We access the EventEmitter class through the events module. Once imported we’ll need to create a new object from the class to start using it.

        const EventEmitter = require('events').EventEmitter;
        const myEventEmitter = new EventEmitter;

**Example: adding an event listener**:

Imagine we’re creating a chat room. We want to alert everyone when a new user joins the chat room. We’ll need an event listener for a userJoined event. First, we’ll write a function that will act as our event listener, then we can use EventEmitters on method to set the listener.

        const EventEmitter = require('events').EventEmitter;
        const chatRoomEvents = new EventEmitter;

        function userJoined(username){
        // Assuming we already have a function to alert all users.
        alertAllUsers('User ' + username + ' has joined the chat.');
        }

        // Run the userJoined function when a 'userJoined' event is triggered.
        chatRoomEvents.on('userJoined', userJoined);

The next step would be to make sure that our chat room triggers a userJoined event whenever someone logs in so that our event handler is called. EventEmitter has an emit method that we we use to trigger the event. We would want to trigger this event from within a login function inside of our chatroom module.

        function login(username){
        chatRoomEvents.emit('userJoined', username);
        }

![event](https://image.slidesharecdn.com/eventdrivenprogrammingamazeballs-130313050806-phpapp02/95/event-driven-programming-amazeballs-4-638.jpg?cb=1363151381)
