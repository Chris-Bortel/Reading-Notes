# Read 18: 10-7-2020

## Socket.io

[README](/README.md)

### Review, Research, and Discussion

1. What is the benefit of transforming data into packets? [FNT Software](https://blog.fntsoftware.com/network-transformation-transitioning-to-packet-technology/)

- Part of the Transmission Control Protocol(TCP)They are the most cost-effective, efficient, and scalable networks for content delivery.

2. UDP is often refereed to as a connectionless protocol. Why is this?

3. Can a socket server application have multiple socket connections?

4. Can a socket connection application be connected to multiple socket servers?

- no. There is one client side connection to one port.

5. Can an application be both a socket server and a socket connection?

- yes?

### Document the following Vocabulary Terms

1. OSI Model : Open Systems Interconnection has 7 layers in three categories

- Software layers { Application Layer, Presentation layer, Session layer }

- Heart of OSI { Transport Layer }

- Hardware Layers { Network Layer, Data link layer, Physical layer }

2. TCP Model : Sends data bit by bit and gets acknowledge, then the data gets sent again

3. TCP : Transmission Control Protocol : the protocol works with how much data can be sent at a time and how often it is sent. It is very strict. Data is a big pile of sand, and all of the sand needs to get sent and received or it will not work.

- it is lossless. Data gets sent and then comes back. If the connection gets messed up the process will start over so that you do not lose any of the data

- used for download and the like

- **TCP** is open until it is closed ---> TCP, you are connected to a fiber (socket) for every/ until we end it.

4. UDP : Sister protocol to TCP ---> works the same way, but you do not need all of the data to work.

- UDP is lossy. Drops packets, but the show will keep streaming, just with less pixel/look fuzzy.

- used for streaming

5. Packets : defined amounts of data that are sent at once in order to transfer the data.

6. Socket :

- socket.io is a way to use events over the sockets ---> it allows us to use http to do tcp type work

open server and people are sending things back and forth at real time. Each person is connected to a socket that connects to a server that sends and receives data us data to stream live ? (ex. everyone is using one socket to connect to zoom's servers using UDP) we are ll connected to our own 'wire', that is attached to the server.

- [Web Sockets](https://en.wikipedia.org/wiki/WebSocket)
- [Socket.io Tutorial](https://www.tutorialspoint.com/socket.io/)
- [Socket.io vs Web Sockets](https://www.educba.com/websocket-vs-socket-io/)
- [Socket.io Documentation](https://socket.io/docs/)
- [Socket.io Server API](https://socket.io/docs/server-api)
- [Socket.io Client API](https://socket.io/docs/client-api)
- [Socket Testing Tool](https://amritb.github.io/socketio-client-tool/)
