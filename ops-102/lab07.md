# Network Connectivity Class Notes 07
### What is the Secure Shell (SSH) Protocol?
The Secure Shell (SSH) Protocol is a method for secure remote login from one computer to another.
### What are the typical uses of the SSH protocol?
#### * Providing secure access for users and automated processes.
#### * Interactive and automated file transfers.
#### * Issuing remote commands.
#### * Managing network infrastructure and other mission-critical system components.
### How does the SSH protocol work?
SSH client initiales the connection by contacting to SSH server. Uses public key cryptography to verity the identity of the SSH server. Negotiate parameters and open secure channel. User login to server host operating system.
### How is the data kept safe when transmitted between the SSH client and server?
The data that is transmitted is encrypted according to the parameters negotiated in the setup.
### What is SFTP?
The SFTP (SSH File Transfer Protocol) is a secure file transfer protocol
# What is RDP? And how to use it
### What is Windows Remote Desktop Connection?
It is use by giving users the ability to connect a remote Windows PC or server over the internet or local network, giving them full access to the tool and software installed on it.
### What is RDP?
RDP stands for Remote Desktop Protocol allows remote users to see and use Windows on a device in another location. To use RDP you need a RDP server and an RDP client. RDP server is the Windows PC or server you're connecting to and will control. RDP client is a PC or mobile device with an RDP client app installed, from which you control the server.
### What is the RDP port number?
3389
## Source's
- https://www.ssh.com/academy/ssh/protocol#sftp-file-transfer-protocol
- https://www.comparitech.com/net-admin/what-is-rdp/
