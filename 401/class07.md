# Bearer Authorization

---

## Write the following steps in the correct order:

- Receive access token
- Redirect to a third party authentication endpoint
- Register your application to get a client_id and client_secret
- Make a request to a third-party API endpoint
- Ask the client if they want to sign in via a third party
- Receive authorization code
- Make a request to the access token endpoint

**Correct order**

1. Register your application to get a client_id and client_secret.
2. Ask the client if they want to sign in via a third party.
3. Redirect to a third party authentication endpoint.
4. Make a request to a third-party API endpoint.
5. Receive authorization code.
6. Make a request to the access token endpoint.
7. Receive access token

![auth0](https://images.ctfassets.net/cdy7uua7fh8z/2nbNztohyR7uMcZmnUt0VU/2c017d2a2a2cdd80f097554d33ff72dd/auth-sequence-auth-code.png)

---

## What can you do with an authorization code?

- exchange it for an access token.

## What can you do with an access token?

- allow an application to access an API.

## What’s a benefit of using OAuth instead of your own basic authentication?

- OAuth provides clients a "secure delegated access" to server resources on behalf of a resource owner.
- It specifies a process for resource owners to authorize third-party access to their server resources without providing credentials.

---

## Document the following Vocabulary Terms

- **Client ID**: it is a public identifier for apps, must be unique across all clients that the authorization server handles.
- **Client Secret**: it is a secret known only to the application and the authorization server. It must be sufficiently random to not be guessable.
- **Authentication Endpoint**: it is a security mechanism designed to ensure that only authorized devices can connect to a given network, site or service.
- **Access Token Endpoint**: is an HTTP endpoint that micropub clients can use to obtain an access token given an authorization code.
- **API Endpoint**: it is a point at which an API -- the code that allows two software programs to communicate with each other -- connects with the software program.
- **Authorization Code**: it is an alphanumeric password that authorizes its user.
- **Access token**: the authorization of a specific application to access specific parts of a user’s data.