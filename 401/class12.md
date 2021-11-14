# Socket.io

---

- **What is the benefit of transforming data into packets?**

        to meet the demands of pervasive data-centric applications and services

- **UDP is often referred to as a connectionless protocol. Why is this?**

        No connection needs to be established between the source and destination before you transmit data.

- **Can a socket server application have multiple socket connections?, Can a socket connection application be connected to multiple socket servers?**

        Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to

- **Can an application be both a socket server and a socket connection?**

          You can not combine server and client sockets into one, because a TCP/IP connection goes from a source port to a destination port

---

## Document the following Vocabulary Terms

**Observer Pattern**: The observer pattern is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.

**Listener**: a procedure in JavaScript that waits for an event to occur.

**Event Handler**: It is the function that will handle a particular proccess when an event occurred.

**Event Driven Programming**: Event-driven programming is a programming paradigm in which the flow of program execution is determined by events - for example a user action such as a mouse click, key press, or a message from the operating system or another program.

**Event Loop**: is a programming construct or design pattern that waits for and dispatches events or messages in a program.

**Event Queue**: is a repository where events from an application are held prior to being processed by a receiving program or system.

**Call Stack**: is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.

**Emit/Raise/Trigger**: these are terminologies to discribe some functionality in Event Driven Programming.

**Subscribe**: This is a JavaScript object that defines the handlers for the notifications you receive.

**database**: It is the palce that we are saving the data into.

---

## Web Sockets

- WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection. The WebSocket protocol was standardized by the IETF as RFC 6455 in 2011, and the WebSocket API in Web `IDL` is being standardized by the `W3C`.

- WebSocket is distinct from HTTP. Both protocols are located at layer `7` in the `OSI` model and depend on TCP at layer 4. Although they are different, `RFC 6455` states that WebSocket "is designed to work over HTTP ports 443 and 80 as well as to support HTTP proxies and intermediaries," thus making it compatible with HTTP. To achieve compatibility, the WebSocket handshake uses the HTTP Upgrade header to change from the HTTP protocol to the WebSocket protocol.

- The WebSocket protocol enables interaction between a web browser (or other client application) and a web server with lower overhead than half-duplex alternatives such as HTTP polling, facilitating real-time data transfer from and to the server. This is made possible by providing a standardized way for the server to send content to the client without being first requested by the client, and allowing messages to be passed back and forth while keeping the connection open. In this way, a two-way ongoing conversation can take place between the client and the server. The communications are usually done over TCP port number 443 (or 80 in the case of unsecured connections), which is beneficial for environments that block non-web Internet connections using a firewall. Similar two-way browser-server communications have been achieved in non-standardized ways using stopgap technologies such as Comet or Adobe Flash Player.

![web socket](https://upload.wikimedia.org/wikipedia/commons/1/10/Websocket_connection.png)
