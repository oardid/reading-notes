# ***Network scanning with NMAP***
## [***What is a Port Scanner and How Does it Work?***](https://www.varonis.com/blog/port-scanning-techniques)
### What is a port? Describe it with an analogy that would help a family member understand.
A port is a virtual location where networking communication starts and ends. Think of a port like a warehouse. Semi-trucks come into the warehouse to load and unload product. A computer does the same but with data flowing in and out.
### What does a port scanner send to a port to check the current status?
TCP or UDP port on a computer and records the response
### When a port scanner sends a request to connect, what are the three possible responses? Describe them.
 1. Open, Accepted: The computer responds and asks if there is anything it can do for you.
 2. Closed, Not Listening: The computer responds that “This port is currently in use and unavailable at this time.”
 3. Filtered, Dropped, Blocked: The computer doesn’t even bother to respond.
### What is the difference between TCP and UDP?
TCP and UDP are the two most common protocols in use for Internet Protocol (IP) network.
TCP sends each packet in order, complete with error chekcing, verification, and a 3-way handshake to confirm each packet is successful. UDP is a connectionless protocol, so programs that use UDP just send the data - and if you miss a packet, you will never get it again.
## [***Common Ports***](https://www.professormesser.com/network-plus/n10-008/n10-008-video/common-ports-n10-008/)
### List and describe the ports used for the following:
  * Telnet: Telecommunication network protocol, communicates over TCP port 23.
  * SSH: A more secure protocol, communicates over TCP port 22. 
  * DNS:Domain Name System, Comunicates over UDP portocol using port 53.
  * SMTP: Simple Mail Transfer Protocol, Comunicates using TCP port 25. Enrypted form of SMTP that usees TLS commonly uses TCP port 587.
  * HTTP: Hypertext Transfer Protocol, communicates over TCP port 80.
  * HTTPS: Hypertext Transfer Protocol Secure, Comunicates over TCP port 443.
  * RDP: Remote Desktop Protocol, Communicates using TCP port 3389.
  * Ping:
