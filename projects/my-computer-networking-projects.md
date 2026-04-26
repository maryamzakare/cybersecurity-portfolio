# My Computer Networking Projects

## What This Project Is About

This portfolio page summarizes three computer networking projects I completed in my Computer Networks course. The projects focused on TCP socket programming, reliable file transfer over UDP, and building a minimal HTTP/1.1 web server.

Together, these projects helped me understand how real networked systems communicate, how reliability is built into protocols, and how client-server applications work.

## Project 1: TCP Command-Line Chat Application

In this project, I built a command-line chat application using Java socket programming.

The application allowed two users to connect and exchange messages through a client-server model.

### What I Implemented

- Server mode
- Client mode
- Auto mode
- Connection status command
- Quit command
- Real-time two-way communication
- Socket binding, listening, connecting, and closing

### Technical Concepts

- TCP sockets
- Client-server architecture
- Java `ServerSocket`
- Java `Socket`
- Input and output streams
- Threading for asynchronous communication
- Port binding and cleanup

### What I Learned

I learned how applications communicate through sockets, how ports are opened and released, and why asynchronous communication is important for real-time messaging.

This project also helped me understand how communication apps work at a basic networking level.

## Project 2: Reliable File Transfer Over UDP

In this project, I built a reliable file transfer system on top of UDP.

Because UDP does not guarantee delivery, I implemented reliability using sequence numbers, acknowledgments, timeouts, and retransmission.

### What I Implemented

- UDP sender
- UDP receiver
- Stop-and-Wait transfer mode
- Sliding Window transfer mode
- Packet sequence numbers
- ACK handling
- Timeout and retransmission logic
- File reconstruction at the receiver

### Packet Structure

| Field | Purpose |
| --- | --- |
| Sequence Number | Tracks packet order |
| Flags | Identifies control information such as ACK or EOF |
| Data Length | Shows how much payload data is included |
| Payload | Contains the file data being transferred |

### Technical Concepts

- UDP communication
- Reliability over unreliable transport
- Stop-and-Wait protocol
- Sliding Window protocol
- Packet design
- Flow control
- Retransmission
- File transfer integrity

### What I Learned

I learned that reliability is not automatic in every protocol. It must be designed using acknowledgments, ordering, timeout handling, and retransmission.

This project helped me understand how real-world protocols build stable communication on top of lower-level network behavior.

## Project 3: Minimal HTTP/1.1 Server

In this project, I worked on a minimal HTTP/1.1 server using the Java Socket API.

The server was designed to support basic web requests and responses using the GET and HEAD methods.

### What The Server Supports

- HTTP GET requests
- HTTP HEAD requests
- Host header validation
- HTTP status codes
- Serving files from a safe `public_html` directory
- Multiple concurrent requests using multithreading
- Response headers such as `Server`, `Content-Length`, and `Content-Type`

### HTTP Status Codes Practiced

| Status Code | Meaning |
| --- | --- |
| 200 OK | Request succeeded |
| 400 Bad Request | Request was malformed |
| 404 Not Found | Requested resource was not found |
| 501 Not Implemented | Request method is not supported |

### Technical Concepts

- HTTP request parsing
- HTTP response construction
- TCP-based application protocols
- Web server behavior
- File serving restrictions
- Multithreading
- Content types
- Security considerations for file access

## Cybersecurity Connection

These projects connect strongly to cybersecurity because security analysts need to understand how systems communicate before they can detect abnormal or malicious behavior.

The projects helped me understand:

- How clients and servers communicate
- How ports and services behave
- How TCP and UDP differ
- How packet order and reliability work
- How web servers process requests
- Why unsafe file access can create security risks
- How network behavior supports incident response and traffic analysis

## Skills I Practiced

- Java socket programming
- TCP communication
- UDP communication
- HTTP protocol basics
- Client-server design
- Packet structure design
- Multithreaded programming
- Debugging network applications
- Command-line testing
- GitHub workflow

## Tools and Technologies

- Java
- Java Socket API
- TCP
- UDP
- HTTP/1.1
- VS Code
- GitHub Classroom
- Terminal commands
- Build scripts
- Local network testing

## What I Learned Overall

These three projects gave me hands-on experience with networking beyond theory. I learned how messages, files, and web requests move between systems, and I practiced building parts of the communication process myself.

This foundation is important for cybersecurity because many attacks, investigations, and defenses depend on understanding network behavior.
