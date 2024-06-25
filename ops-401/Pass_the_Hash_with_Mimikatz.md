## [What is Mimikatz?](https://www.varonis.com/blog/what-is-mimikatz)

### Name the six credential-gathering techniques which Mimikatz is able to perform and explain how two of them work.
* Pass-the-hash: Attackers use Mimikatz to pass an exact hash string to log in to the target computer.
* Pass-the-ticket: Mimikatz provides functionality for a user to pass a Kerberos ticket to another computer and log in with that user's ticket.
* Overpass-the-hash: This technique passes a unique key obtained from a domain controller to impersonate a user.
* Kerberoast golden tickets: A golden ticket gives you non-expiring domain admin credentials to any computer on the network
* Kerberoast sliver tickets: Kerberos grants a user a TGS ticket that's used to log in to any services on the network.
* Pass-the-cache: Generally the same as a pass-the-ticket, but uses the saved and encrypted login data on a Mac/UNIX/Linux system.

Pass-the-Ticket: Mimikatz extracts a Kerberos ticket from a computer's memory or cache, removes constraints such as client address or timestamp, and uses the modified ticket to impersonate the user on another computer. This technique allows access to network resources without knowing the user's password.

Kerberoast Golden Tickets: Mimikatz extracts a Kerberos TGS ticket, modifies it to grant domain admin privileges and removes constraints, and uses the modified ticket to authenticate as a domain admin on any computer in the domain. This technique grants attackers full access to the domain and its resources.
### What are four ways we can defend against Mimikatz attacks. Explain how two of the mitigations can stop Mimikatz.
1. Change admin privilieges.
2. Change caching policy.
3. Turn off debugging privileges.
4. Increase local security authority.
   
Two of these steps can stop Mimikatz attacks:
* Requiring ticket validation on each use prevents Mimikatz from obtaining sensitive information.
* Disabling debugging privileges prevents Mimikatz from running effectively and gathering credentials.
