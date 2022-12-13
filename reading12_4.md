# SOCKET.io

## Web Sockets

What is a Web Socket?

- WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection. The WebSocket protocol was standardized by the IETF as RFC 6455 in 2011.

Describe the Web Socket request/response handshake and what happens once the connection is established.

- WebSocket handshake uses the HTTP Upgrade header to change from the HTTP protocol to the WebSocket protocol


Web Sockets provide a standardized way for the server to send content to a client without first receiving a ____ from that client.

- request


## Socket.io Tutorial

What does the event handler io.on() do?

- An event handler that will be called when the server broadcasts a notification to this socket


Describe some possible proof of life or proof that the code works as expected

- When a server can emit and recives a message


What does socket.emit() do?

 - emit a message to this socket using a certain message


## Socket.io vs Web Sockets

What is the difference between WebSocket and Socket.IO? (think Git and GitHub, or OAuth and Auth0).

- WebSocket is the communication Protocol that provides bidirectional communication between the Client and the Server over a TCP connection; WebSocket remains open all the time, so they allow real-time data transfer. When clients trigger the request to the server, it does not close the connection on receiving the response; it rather persists and waits for the Client or server to terminate the request.

Socket.IO is a library that enables real-time and full-duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts; both WebSocket vs Socket.io are event-driven libraries.


When would you use Socket.IO?

- It helps in broadcasting to multiple sockets at a time and handles the connection transparently.
It works on all platform, server or device, ensuring equality, reliability, and speed.
It automatically upgrades the requirement to WebSocket if needed.
It is a custom real-time transport protocol implementation on top of other protocols.
It requires both libraries to be used Client side as well as a server-side library.
IO works on work-based events. there are some reserved events that can be accessed using the Socket on the server side like Connect, message, Disconnect, Ping and Reconnect.
There are some Client based reserved events like Connect, connect- error, connect-timeout and Reconnect etc.


When would you use WebSockets?

- WebSocket helps in real-time communication between the Client and the webserver.
This protocol helps in transforming to cross-platform in a real-time world between the server and the client.
This also enables the business worldwide for a real-time web application to enhance and increase the feasibility.
The major advantage it stands over an HTTP connection that it provides full-duplex communication.