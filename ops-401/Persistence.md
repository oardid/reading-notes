## [PowerShell Empire No Longer Maintained](https://www.bleepingcomputer.com/news/security/powershell-empire-framework-is-no-longer-maintained/)

### What is one of the major advantages of PowerShell Empire?
Uses encrypted communication with the command and control server and makes it difficult to detect its traffic, especially in large networks. 
### What are some of the APT groups that have been known to use PS Empire and into which step of the Cyber Kill Chain does the use of PS Empire fall?
APT28 (Fancy Bear): a Russian-speaking group believed to be sponsored by the Russian government.
The use of Empire falls into the command and control (c2) step of the cyber kill chain.
### What are the four main components needed to pull off an attack using PS Empire?
* Listener: the listener is a process which listens for a connection from the machine we are attacking. This helps Empire send the loot back to the attacker’s computer.
* Stager: A stager is a snippet of code that allows our malicious code to be run via the agent on the compromised host.
* Agent: An agent is a program that maintains a connection between your computer and the compromised host.
* Module: These are what execute our malicious commands, which can harvest credentials and escalate our privileges as mentioned above.

##### Bookmark and Review
##### [Hacking with Empire – PowerShell Post-Exploitation Agent](https://www.hackingarticles.in/hacking-with-empire-powershell-post-exploitation-agent/)
