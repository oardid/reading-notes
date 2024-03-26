# ***Network Traffic Analysis with Wireshark***

## [***Layers of OSI Model***](https://www.geeksforgeeks.org/open-systems-interconnection-model-osi/)
### 1. What does “OSI” stand for?
OSi stands for Open Systems Interconnection
### 2. List the 7 layers of the OSI model and what each one is responsible for.
1. Physical Layer
2. Data Link Layer
3. Network Layer
4. Transport Layer
5. Session Layer
6. Presentation Layer
7. Application Layer
### 3. Distinguish which layers are the “hardware layers”, and which layers are the “software layers”. What does that even mean?
Hardware layers are Network Layer, Data Link Layer, and Physical Layer. Hardware Layers are the physical components of a computer system. Software layers are Session Layer, Presnetation Layer, and Application Layer. Software Layers are software that interact with hardware to perform speciifc functions.
### 4. How can the OSI model be used in troubleshooting?
It divides network communication into 7 layers which makes it easier to understand.
## [***What Is Wireshark and How Is It Used?***](https://www.comptia.org/content/articles/what-is-wireshark-and-how-to-use-it)
### 1. What is Wireshark?
A network protocol analyzer, or an application that captures packets from a network connection, such as from your computer to your home office or the internet.
### 2. What is a packet?
The name given to a discrete unit of data in a typical Ethernet network.
### 3. What 3 high-level things does Wireshark accomplish? How could these be used for nefarious purposes? For benevolent purposes?
1. Packet Capture: Wireshark listens to a network connection in real time and then grabs entire streams of traffic – quite possibly tens of thousands of packets at a time.
2. Filtering: Wireshark is capable of slicing and dicing all of this random live data using filters. By applying a filter, you can obtain just the information you need to see.
3. Visualization: Wireshark, like any good packet sniffer, allows you to dive right into the very middle of a network packet. It also allows you to visualize entire conversations and network streams.
- Wireshark possesses the potential for both malicious exploitation, including eavesdropping, data theft, and reconnaissance, as well as benevolent applications such as network security, diagnosing network issues, and optimizing network performance.
