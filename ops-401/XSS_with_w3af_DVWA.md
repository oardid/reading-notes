## [Cross-site scripting](https://portswigger.net/web-security/cross-site-scripting)

### Explain how a cross-site scripting attack works in non-technical terms.
Imagine you're browsing your favorite website, and you click on a link that looks like it's part of the website. But, this link is actually controlled by an attacker. When you click on it, the attacker's code runs on your browser, allowing them to steal your login credentials, and sensitive information, or even take control of your account.

### What are the three types of XSS attacks?
* Reflected XSS, where the malicious script comes from the current HTTP request.
* Stored XSS, where the malicious script comes from the website's database.
* DOM-based XSS, where the vulnerability exists in client-side code rather than server-side code.
### If an attacker successfully exploits an XSS vulnerability, what malicious actions would they be able to perform?
Steal sensitive information like login credentials, credit card numbers, or personal data. Hijack user sessions or take control of their accounts. Redirect users to phishing websites or download malware.
### What are some security controls that can be implemented to prevent XSS attacks?
* **Filter input on arrival.** At the point where user input is received, filter as strictly as possible based on what is expected or valid input.
* **Encode data on output.** At the point where user-controllable data is output in HTTP responses, encode the output to prevent it from being interpreted as active content. Depending on the output context, this might require applying combinations of HTML, URL, JavaScript, and CSS encoding.
* **Use appropriate response headers.** To prevent XSS in HTTP responses that aren't intended to contain any HTML or JavaScript, you can use the Content-Type and X-Content-Type-Options headers to ensure that browsers interpret the responses in the way you intend.
* **Content Security Policy.** As a last line of defense, you can use a Content Security Policy (CSP) to reduce the severity of any XSS vulnerabilities that still occur.
##### Bookmark and Review
##### [Security Report for In-Production Web Applications](https://www.rapid7.com/globalassets/_pdfs/whitepaperguide/rapid7-tcell-application-security-report.pdf)
