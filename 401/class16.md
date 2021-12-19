# AWS: Cloud Servers

---

**Describe the Web-Request-Response-Cycle**

- The request/response cycle traces how a user’s request flows through the app. Understanding the request/response cycle is helpful to figure out which files to edit when developing an app.

- First a user gives a client a URL, the client builds a request for information (or resources) to be generated by a server. When the server receives that request, it uses the information included in the request to build a response that contains the requested information. Once built, that response is sent back to the client in the requested format, to be rendered to the user.

![wrrc](https://miro.medium.com/max/697/1*fPLxbzS5zdJlKrzxf4VVXQ.png)

**Explain what a “server” is, as it relates to the WRRC**

- It is the side that receive a request for some kind of information from the client, then `responses` back to the client.

**What does it mean to “deploy” an application?**

- It means to store the application in place that will make it usable by anyone, not just by the developer on the local machine.

---

## Document the following Vocabulary Terms

- **Server**: It is a piece of computer hardware or software (computer program) that provides functionality for other programs or devices, called "clients".

- **Pub/Sub**: The Publish/Subscribe pattern, also known as pub/sub, is an architectural design pattern that provides a framework for exchanging messages between publishers and subscribers. This pattern involves the publisher and the subscriber relying on a message broker that relays messages from the publisher to the subscribers. The host (publisher) publishes messages (events) to a channel that subscribers can then sign up to.

- **WRRC**: The request/response cycle traces how a user’s request flows through the app. Understanding the request/response cycle is helpful to figure out which files to edit when developing an app.

---

## AWS EC2

- Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the cloud. It is designed to make web-scale cloud computing easier for developers. Amazon EC2’s simple web service interface allows you to obtain and configure capacity with minimal friction. It provides you with complete control of your computing resources and lets you run on Amazon’s proven computing environment.

To know more [AWS EC2](https://aws.amazon.com/ec2/)