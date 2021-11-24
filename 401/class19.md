# AWS: Events

---

**Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server**

- Both of them can do some functionality and deal with the database when an http request occurred.

**List the AWS Database offerings and talk about the pros and cons of each**

- [AWS Databases](https://aws.amazon.com/products/databases/)

**What’s the difference between a FIFO and a standard queue?**

- Standard queues provide at-least-once delivery, which means that each message is delivered at least once. FIFO queues provide exactly-once processing, which means that each message is delivered once and remains available until a consumer processes it and deletes it.

**How can the server be assured a message was properly received?**

- By creating a message queue that is holding the message till the receiver send back that the message is received successfully.

---

## Document the following Vocabulary Terms

- **Serverless API**: it is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers.

- **Triggers**: it is a Lambda resource or a resource in another service that you configure to invoke your function in response to lifecycle events, external requests, or on a schedule.

- **Dynamo vs Mongo**: MongoDB is a general-purpose, document-based distributed NoSQL database , DynamoDB is a proprietary NoSQL database by Amazon that supports key-value and document data offered via the Amazon Web Services. MongoDB stores the data as a json objects in collections, DynamoDB stores the data in table forms consists of raws and columns.

![MongoDB vs DynamoDB](https://webassets.mongodb.com/_com_assets/cms/MongoDB_compared_DynamoDB-x6jmjtyquh.png)

---

## Preparation Materials

[SQS and SNS Basics](https://www.youtube.com/watch?v=UesxWuZMZqI)

[AWS SQS vs SNS](https://medium.com/awesome-cloud/aws-difference-between-sqs-and-sns-61a397bf76c5)

[SNS Javascript SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SNS.html)

[SQS Javascript SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SQS.html)
