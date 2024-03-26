# [***VirtualBox Network Settings Guide***](https://www.nakivo.com/blog/virtualbox-network-setting-guide/)
### Which network mode in VirtualBox can be used to emulate unplugging the Ethernet cable from the network?
Not attached mode 
### Which network mode would be best if you wanted to run a server on a VM that could be fully accessible from your physical local area network?
NAT newtwork
### What are the three options of promiscuous mode and what does each do?
* Deny. Any traffic that is not intended to the virtual network adapter of the VM is hidden from the VM. This option is set by default.
* Allow VMs. All traffic is hidden from the VM network adapter except the traffic transmitted to and from other VMs.
* Allow All. There are no restrictions in this mode. A VM network adapter can see all incoming and outgoing traffic.
### What is Port Forwarding?
Port Forwarding is a process of intercepting traffic addressed to the appropriate IP address and port in addition to redirecting that traffic to a different IP address and/or port.
