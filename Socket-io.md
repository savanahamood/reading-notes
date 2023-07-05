# Socket.io
### Web Sockets
**1. What is a Web Socket?**

A WebSocket is a communication protocol that provides full-duplex communication channels over a single TCP connection. It enables real-time, bidirectional communication between a client and a server, allowing them to send messages to each other at any time without the need for frequent HTTP requests.

**2. Describe the Web Socket request/response handshake and what happens once the connection is established.**

The WebSocket request/response handshake is the process that occurs between the client and the server to establish a WebSocket connection. Here's an overview of the handshake process:
* Client sends an HTTP request by sending a regular HTTP request to the server. This request includes specific headers indicating the intent to upgrade the connection to a WebSocket.
* Server responds with an HTTP response the server checks if it supports WebSocket connections. If it does, the server responds with an HTTP response, known as the WebSocket handshake response.
* Upgrade to WebSocket connection This includes the HTTP status code 101 and the "Upgrade" and "Connection" headers.
* Connection established Once the client receives the server's response and verifies that it is a valid WebSocket handshake, it completes the handshake process. At this point, the WebSocket connection is established, and both the client and server can start sending WebSocket messages.

Here's what happens after the connection is established:
* Sending and receiving messages
* Event-driven communication
* Persistent connection
* Closing the connection


**3. Web Sockets provide a standardized way for the server to send content to a client without first receiving a __request __ from that client.**

### Socket.io Tutorial
**1. What does the event handler io.on() do?**

The event handler io.on() in the context of Socket.IO is used to listen for and handle events that occur on the server side. It is a method provided by the Socket.IO library in Node.js to register event handlers for various events.

**2. Describe some possible proof of life or proof that the code works as expected**

* Passing unit tests that cover different scenarios and edge cases.
* Executing the code with sample inputs and verifying the expected outputs.
* Reviewing the code logic and design through code reviews.

**3. What does socket.emit() do?**

socket.emit() enables the server to send custom events and associated data to connected clients, allowing real-time communication and triggering client-side actions based on the received events.


### Socket.io vs Web Sockets

**1. What is the difference between WebSocket and Socket.IO? (think Git and GitHub, or OAuth and Auth0).**

* WebSocket is the communication Protocol that provides bidirectional communication between the Client and the Server over a TCP connection; WebSocket remains open all the time, so they allow real-time data transfer. When clients trigger the request to the server, it does not close the connection on receiving the response; it rather persists and waits for the Client or server to terminate the request.

* Socket.IO is a library that enables real-time and full-duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts; both WebSocket vs Socket.io are event-driven libraries.
Client-Side: it is the library that runs inside the browser
Server Side: It is the library for Node.js


**2. When would you use Socket.IO?**

Socket.IO is used when you need real-time, bidirectional communication between a server and clients, such as in chat applications, live tracking systems, collaborative tools, and real-time analytics.

**3. When would you use WebSockets?**

WebSockets are used when you need a persistent, low-latency, full-duplex communication channel between a client and a server, such as in real-time applications, gaming, live streaming, monitoring systems, collaborative editing, and IoT applications.

### Resources: 

[Socket.io Documentation](https://socket.io/docs/)

[Socket.io Server API](https://socket.io/docs/server-api)

[Socket.io Client API](https://socket.io/docs/client-api)

[Socket Testing Tool](https://amritb.github.io/socketio-client-tool/)


