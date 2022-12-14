# reading 13

## Socket.io Chat Example


What proof of life are we getting on the backend from the above app?

- when a socket is connected


Socket.IO gives us the i0.emit() method to send an event to everyone. What flag would you use if you want to send a message to everyone except for a certain emitting socket?

- you would just send it within the event that sockets into the server

## Rooms

What is a room and how might a room be useful?

- A room is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of clients:



How do you join a room?

- You can call join to subscribe the socket to a given channel:



how do you leave a room?

- To leave a channel you call leave in the same fashion as join.



## Namespaces

What is a Namespace and what does it allow you to do?

- A Namespace is a communication channel that allows you to split the logic of your application over a single shared connection (also called "multiplexing").

Each namespace potentially has its own what? (hint: 3 things)

- event handlers
- rooms
- middlewares

Discuss a possible use case for separate namespaces

- You could create a separate Namespace for each customer,
