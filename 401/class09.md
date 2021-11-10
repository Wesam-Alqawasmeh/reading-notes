# Authorization/Authentication

---

**What header(s) are used in authentication and authorization**

- To pass the Authorization (basic auth username and password encoded by base-64 ) or (bearer token).

**What is safe to put into a JWT**

- Tokens and Secrets.

**How are JWTs validated**

- JWT.verify will check if the token and the secret matches the signed token with the same secret.

---

## Document the following Vocabulary Terms

- **RBAC**: Role-based access control (RBAC) is a popular mechanism to enforce authorization in applications. When using RBAC, an application developer defines roles rather than authorizing individual users or groups.

- **User Roles**: It is the permessions that manage resources and what users can do with those resources.

- **JWT Token**: It is the authentication signature which is issued by JWT by passing the pay load and a secret to add more security and keep the user logged in while routes are refreshing.