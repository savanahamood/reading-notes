# Message Queues

### Socket.io Chat Example

**1.Explain to a non-technical recruiter what the Chat Example (above) does.**

it is a real-time chat application built using Socket.IO, a JavaScript library for enabling real-time, bidirectional communication between a server and multiple clients.

**2.What proof of life are we getting on the backend from the above app?**

we can get a proof of life on the backend by monitoring the connection events between the client and the server and print "connect" on console.

**3.Socket.IO gives us the i0.emit() method to send an event to everyone. What flag would you use if you want to send a message to everyone except for a certain emitting socket?**

socket.broadcast.emit()


### Rooms

**1.What is a room and how might a room be useful?**

A room is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of clients Rooms can be useful such as Chat Applications

**2.How do you join a room?**

You can call join to subscribe the socket to a given channel:

io.on("connection", (socket) => {
  socket.join("some room");
});

And then simply use to or in (they are the same) when broadcasting or emitting:

io.to("some room").emit("some event");

You can emit to several rooms at the same time:

io.to("room1").to("room2").to("room3").emit("some event")


**3.how do you leave a room?**

To leave a channel you call leave in the same fashion as join socket.leave(room)

### Namespaces
**1.What is a Namespace and what does it allow you to do?**

A Namespace is a communication channel that allows you to split the logic of your application over a single shared connection (also called "multiplexing")

**2.Each namespace potentially has its own what? (hint: 3 things)**

Each namespace potentially has its own:
* Set of Connected Sockets
* Event Handlers
* Rooms

**3.Discuss a possible use case for separate namespaces**

separate namespaces provide a way to create isolated and customized communication channels for different organizations or clients within a multi-tenant or multi-application system. It enables efficient management, scalability, and security by keeping the communication separate and tailored to the needs of each entity.



### Resources: 

[Socket.io Chat Example](https://socket.io/get-started/chat/)

[Rooms](https://socket.io/docs/v4/rooms)

[Namespaces](https://socket.io/docs/v4/namespaces/)

[Socket.io Emit Cheatsheet](https://socket.io/docs/v4/emit-cheatsheet/)