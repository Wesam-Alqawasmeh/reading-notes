# AWS: API, Dynamo and Lambda

---

**What are serverless functions?**

- they are a programmatic functions written by a software developers for a single purpose. Hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.

**If you were to create a system that emulated Lambda functions, how would you do it?**

- By Event Driven Programming.

**Describe how a CDN works**

- The mission of a CDN is to reduce latency. Latency is that annoying delay you experience when trying to access a web page or video stream before it fully loads on your device. Although measured in milliseconds, it can feel like forever, and may even result in a load error or time-out. Some content delivery networks alleviate latency by reducing the physical distance that the content needs to travel to reach you. Therefore, larger, more widely distributed CDNs are able to deliver web content more quickly and reliably by putting the content as close to the end user as possible.

- Let’s say it’s the weekend and you want to kick back and stream the latest Hollywood movie release — the CDN finds an optimal server on its network to serve up that video. Usually, that will be the server closest to your physical location. The media files will be cached and remain on that content delivery network server for other user requests in the same geographic area. If the content you requested is unavailable or outdated, the CDN service will store the newly fetched content to serve any future requests.

- While the delivery of website content is a common use for CDNs, it’s not their only function. In fact, CDNs deliver a wide variety of content that includes: 4K and HD-quality video, audio streams, software downloads such as apps, games, and OS updates, and much more. Potentially any data that can be digitized can be delivered through a content delivery network.

---

## Document the following Vocabulary Terms

- **Serverless Functions**: they are a programmatic functions written by a software developers for a single purpose. Hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.

- **Cloud Storage**: is a cloud computing model that stores data on the Internet through a cloud computing provider who manages and operates data storage as a service.

- **CDN**: A Content Delivery Network (CDN) is a geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.

---

## AWS API Gateway

- Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale. APIs act as the "front door" for applications to access data, business logic, or functionality from your backend services. Using API Gateway, you can create RESTful APIs and WebSocket APIs that enable real-time two-way communication applications. API Gateway supports containerized and serverless workloads, as well as web applications.

- API Gateway handles all the tasks involved in accepting and processing up to hundreds of thousands of concurrent API calls, including traffic management, CORS support, authorization and access control, throttling, monitoring, and API version management. API Gateway has no minimum fees or startup costs. You pay for the API calls you receive and the amount of data transferred out and, with the API Gateway tiered pricing model, you can reduce your cost as your API usage scales.

## DynamoDB

- DynamoDB is a hosted NoSQL database offered by Amazon Web Services (AWS). It offers:

        - reliable performance even as it scales.
        - a managed experience, so you won't be SSH-ing into servers to upgrade the crypto libraries.
        - a small, simple API allowing for simple key-value access as well as more advanced query patterns.

DynamoDB is a particularly good fit for the following use cases:

1. Applications with large amounts of data and strict latency requirements.
2. Serverless applications using AWS Lambda.
3. Data sets with simple, known access patterns.
