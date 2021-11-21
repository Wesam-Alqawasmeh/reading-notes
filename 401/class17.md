# AWS: S3 and Lambda

---

**Describe “The Cloud”**

- "The cloud" refers to servers that are accessed over the Internet, and the software and databases that run on those servers. Cloud servers are located in data centers all over the world. By using cloud computing, users and companies do not have to manage physical servers themselves or run software applications on their own machines.

**What is a container (as it relates to computers and servers)?**

- It is a software unit that packs application code and all the dependencies used in the application into a single package.

**What is auto-scaling?**

- It is a method used in cloud computing that dynamically adjusts the amount of computational resources in a server farm

example

        the number of servers running behind a web application may be increased or decreased automatically based on the number of active users on the site.

**What is bandwidth?**

- It the amount of data your website can transfer to your users in a given amount of time.

---

## Document the following Vocabulary Terms

- **Server Instances**: It is a collection of Servers which are run by a solitary Server service or instance. The details of each server instance can be viewed on the service console which can be web-based or command-line based. The instances are not linked with each other and can be controlled or managed separately.
- **Containers**: It is a software unit that packs application code and all the dependencies used in the application into a single package.
- **Cloud Services**: They are infrastructure, platforms, or software that are hosted by third-party providers and made available to users through the internet.facilitate the flow of user data from front-end clients (e.g. users’ servers, tablets, desktops, laptops—anything on the users’ ends), through the internet, to the provider’s systems, and back. Users can access cloud services with nothing more than a computer, operating system, and internet connectivity or virtual private network (VPN).
- **Cloud Architecture**: The technology components that are combined to build a cloud.
- **AWS**: Amazon Web Service.
- **EC2/Beanstalk vs Heroku**: Heroku’s pricing takes exponential price jumps as one adds common additional features, e.g., auto-scaling, where-as AWS pricing is fairly linear. On the other hand, Heroku is generally simpler to get up and running as AWS has a fairly steep initial learning curve.

---

## AWS S3

- Amazon Simple Storage Service (Amazon S3) is an object storage service offering industry-leading scalability, data availability, security, and performance. Customers of all sizes and industries can store and protect any amount of data for virtually any use case, such as data lakes, cloud-native applications, and mobile apps. With cost-effective storage classes and easy-to-use management features, you can optimize costs, organize data, and configure fine-tuned access controls to meet specific business, organizational, and compliance requirements.

**use cases**:

1. Build a data lake.
2. Back up and restore critical data.
3. Archive data at the lowest cost.
4. Run cloud-native applications.

**CDN**

- A Content Delivery Network (CDN) is a geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.
