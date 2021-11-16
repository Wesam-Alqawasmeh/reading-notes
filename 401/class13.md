# Message Queues

---

**What does it mean that web sockets are bidirectional?**

- Whereas HTTP relies on a client request to receive a response from the server for every exchange, WebSockets allow for full-duplex bidirectional communication. This enables the server to send real-time updates asynchronously, without requiring the client to submit a request each time.

**Does socket.io use HTTP? Why?**

- yes, it depends on HTTP for its initial connection setup.

**What happens when a client emits an event?**

- it will send a request to the server in packets contains the payload for that event.

**What happens when a server emits an event?**

- it will send a request to the client in packets contains the payload for that event.

**What happens if a client “misses” an event**

- nothing will happen it will be ignored.

**How can we mitigate this?**

- by always having the handlers installed and then deciding in the handlers (based on other state) whether to do anything with the message or not.

---

## Document the following Vocabulary Terms

**Socket**: an endpoint of a communication between two programs running on a network.

**Web Socket**: is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.

**Socket.io**: Realtime application framework

**Client**: the side that will request from the server

**Server**: the side that will response to the clients request.

**OSI Model**: (Open Systems Interconnection Model) is a conceptual framework used to describe the functions of a networking system.

**TCP Model**: The TCP/IP model is a concise version of the OSI model. It contains four layers, unlike seven layers in the OSI model.

**TCP**: Transmission Control Protocol/Internet Protocol. TCP/IP is a set of standardized rules that allow computers to communicate on a network such as the internet

**UDP**: User Datagram Protocol, is a communication protocol used across the Internet for especially time-sensitive transmissions such as video playback or DNS lookups

**Packets**: is a formatted chunk of data sent over a network.

---

## More sources to reading

[Socket.io Chat Example](https://socket.io/get-started/chat/)

[Rooms and Namespaces](https://socket.io/docs/rooms-and-namespaces/)

[Socket.io Emit Cheatsheet](https://socket.io/docs/emit-cheatsheet/)
