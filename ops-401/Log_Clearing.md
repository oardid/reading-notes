## [Log Tampering 101](https://www.infosecinstitute.com/resources/hacking/ethical-hacking-log-tampering-101/)
### Explain some specifics of why a hacker might want to clear log files to a family member. Do not use the example from the article.
Hackers might clear them to cover their tracks. For example, if they hacked into someone's account, clearing logs would hide evidence. Or, if they used someone else's computer, clearing logs would make it harder to find out.
### What are three methods by which you can clear logs in a Windows system?
Clearlogs.exe:
* Use clearlogs.exe file to clear security logs on a Window system.
* Run the command in a command line
```
clearlog.exe -sec
```
Meterpreter:
* This advanced payload is a type of shell that, will help to clear all logs in a Windows system in newer versions of Meterpreter. After compromising the system with Metasploit, use a Meterpreter command prompt and enter the following command:
```
Meterpreter > clearev
```
Windows Event Viewer:
* Use Windows Event Viewer to clear logs even if auditing has been disabled.
* Navigate to Event Viewer under Windows Logs, right-click on the log type you want to clear, and select "Clear All Events".
* This will clear all events in the selected log type.
### What are the four steps in the process of covering your tracks.
1. Disable auditing
2. Clearing logs
3. Modifying logs
4. Erasing command history
##### Bookmark and Review
##### [NIST SP800-154 Guide to Data-Centric Threat Modeling](https://csrc.nist.gov/pubs/sp/800/154/ipd#pubs-abstract-header)
