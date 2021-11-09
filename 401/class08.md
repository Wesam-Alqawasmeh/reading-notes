# Access Control (ACL) 

---

**1.When is Basic Authorization used vs. Bearer Authorization?**

Basic Authorization | Bearer Authorization
--------------------- | -------------------
when an authenticated user sign in | when exchanging the data between two parties

**2.What does the JSON Web Token package do?**

- it can grant access to resources, and transfer the data securely.

**3.What considerations should we make when creating and storing a SECRET?**

1. No one should know what is it except the developer.

2. It must sent with each request the same with out any changes.

3. Save it in .env file and keep it locally don't push it to github.

---

**Document the following Vocabulary Terms**

**encryption**: it is the process of converting human-readable plaintext to incomprehensible text that only authorized parties can understand.

**token**: it is the authentication signature which is issued by a server to add more security and keep the user logged in while routes are refreshing.

**bearer**: A particular type of access token, with the property that anyone can use the token. In other words, a client doesn't need a cryptographic key or other secret to use a bearer token.

**secret**: is a symmetric key that is known by both the sender and the receiver. we use it for JWT methods.

**JSON Web Token**:  is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object.


![jwt](https://cdn2.auth0.com/docs/media/articles/api-auth/client-credentials-grant.png)
---

## RBAC

- Role-based access control (RBAC) is a popular mechanism to enforce authorization in applications. When using RBAC, an application developer defines roles rather than authorizing individual users or groups. An administrator can then assign roles to different users and groups to control who has access to what content and functionality.

- RBAC helps you, as an app developer, manage resources and what users can do with those resources. RBAC also allows an app developer to control what areas of an app users have access to. While admins can control which users have access to an app using the User assignment required property, developers need to account for specific users within the app and what users can do within the app.

![rbac](https://assets.website-files.com/5ff66329429d880392f6cba2/60a23b06b2d3123baf7c305d_RBAC.png)