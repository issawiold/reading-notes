## Review: High-level HTTP

### What are the five steps in the HTTP Request Lifecycle?

1. LOCAL PROTOCAL
2. resolve ip
3. establish a tcp connection
4. send HTTP request
5. tearing down and cleaning up , end of tcp connection and pc start analysing the data it received

### What are the two things the client needs before it can make an HTTP Request?

1. receive a udp packet 
2. complete a three way handshake 

### Explain the four way handshake and what it does.

Step 1: Active Open by the Client (SYN)

The client (your computer or device) initiates the process by sending a "SYN" (synchronize) packet to the server.
This packet contains a randomly chosen sequence number (let's call it X) and the "SYN" flag.
The client is requesting to establish a connection with the server.
Step 2: Server Responds (SYN-ACK)

The server receives the "SYN" packet from the client and responds with a "SYN-ACK" (synchronize-acknowledge) packet.
The "SYN-ACK" packet contains its own randomly chosen sequence number (let's call it Y), an acknowledgment number (ack) set to the client's sequence number X+1 (acknowledging the receipt of the client's "SYN" packet), and both the "SYN" and "ACK" flags.
The server is acknowledging the client's request and also indicating its willingness to establish a connection.
Step 3: Client Acknowledges (ACK)

The client receives the "SYN-ACK" packet from the server.
The client sends an "ACK" (acknowledge) packet back to the server.
The "ACK" packet's acknowledgment number is set to the server's sequence number Y+1, and it also acknowledges the server's willingness to establish a connection.
Step 4: Server Acknowledges (Final ACK)

The server receives the "ACK" packet from the client.
At this point, the connection is established and data can start flowing between the client and the server.
After the client's "ACK" is received, the server knows that the connection is fully established and ready for data transfer.
This four-step handshake ensures that both the client and server agree to establish a connection and are ready to exchange data. Each step involves exchanging sequence and acknowledgment numbers to confirm the reception of packets and establish the communication parameters. The handshake also ensures reliability and order in data transmission.

The process is symmetric, meaning both sides of the connection go through the same sequence of steps to establish the connection. This handshake is vital for ensuring a reliable and orderly exchange of data between client and server.

## Java HTTP Request example

### True or False: When making an HTTP request, you MUST follow any redirect returned by the request. Back up your answer.

false ,In its default configuration, without explicit action by the user or the web site, no major browsers would automatically use HTTPS. If you redirect HTTP to HTTPS, make sure to mark your cookies as secure so you don't leak them in the initial accesses through http.Jul 28, 2017
// https://www.npmjs.com/package/follow-redirects
### Which built-in Java class can be used to perform an HTTP request?

HttpURLConnection

### What HTTP status codes represent a successful response? A redirect? A client error?
200-299 successful response
300-399 redirect response 
400-499 client error 
500-599 server error
// https://www.cs.ait.ac.th/~on/O/oreilly/java-ent/servlet/appc_01.htm
