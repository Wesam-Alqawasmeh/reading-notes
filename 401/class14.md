# Event Driven Architecture

---

**What’s the difference between a FIFO and a standard queue?**

- Standard queues provide at-least-once delivery, which means that each message is delivered at least once. FIFO queues provide exactly-once processing, which means that each message is delivered once and remains available until a consumer processes it and deletes it.

**How can the server be assured a message was properly received?**

- By using a message queue in the server and delete the queued message when it receives the client by an emit from the client.

**What classic design pattern is best represented by event driven programming?**

- Observer pattern.

**How do you test an event driven system?**

- By using testing websites or creating a virtual clients and starting the server and clients on the terminal.

---

## Document the following Vocabulary Terms

- **FIFO Queue**: First-In-First-Out queues are designed to enhance messaging between applications when the order of operations and events is critical, or where duplicates can't be tolerated.

- **Pub/Sub**: stands for Publisher/Subscriber, allows services to communicate asynchronously, with latencies on the order of 100 milliseconds.

![pub/sub](https://www.instana.com/media/word-image-345.png)

## Preparation Materials

[AWS SNS and SQS](https://www.youtube.com/watch?v=mXk0MNjlO7A)
