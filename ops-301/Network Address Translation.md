# ***[Network Address Translation (NAT)](https://www.geeksforgeeks.org/network-address-translation-nat/)***
### What is the main purpose for implementing NAT on a network?
To allow multiple devices to access the Internet through a single public address.
### At what layer of the OSI model does NAT happen?
Layer 3, Network layer
### What happens to packets when NAT runs out of addresses in the pool of available IPs?
The packets will be dropped and an INternet Control Message Protocol (ICMP) host unreachable packet to the destination is sent.
### What disadvantage does using NAT pose for routers?
* Translation results in switching path delays.  
* Certain applications will not function while NAT is enabled.  
* Complicates tunneling protocols such as IPsec. 
* Also, the router being a network layer device, should not tamper with port numbers(transport layer) but it has to do so because of NAT. 
