## [Understanding SQL Injection, Identification and Prevention](https://www.varonis.com/blog/sql-injection-identification-and-prevention-part-1)

### What is SQL injection?
It is a flaw that lets attackers execute arbitrary commands on a server
### Can you give an example of how a hacker could use SQL injection to gain unauthorized access?
Suppose a web application has a login page that accepts user input for the username and password. The application uses a query like this to verify the credentials:
```
SELECT * FROM users WHERE username = 'username' AND password = 'password';
```
If an attacker enters a malicious input, such as:
```
' OR 1=1 --
```
The resulting query would become:
```
SELECT * FROM users WHERE username = '' OR 1=1 -- AND password = '';
```
This query would return all rows in the user's table because the OR 1=1 clause is always true. The -- at the end is a comment that tells the database to ignore any further code.
The attacker could then use this vulnerability to extract sensitive data, such as passwords or credit card numbers, or even take control of the entire database.
### What are some ways to prevent SQL injection attacks on a web server?
They perform two important tasks:

First, they offer specific user input sanitization countermeasures to defeat common SQL Injection patterns: the framework will strip NULL characters, line breaks, single quotes, etc. that are often used to piggyback additional SQL commands into an intended query.

Second, they provide a syntax for declaring what a SQL statement is supposed to look like before actually trying to execute it. Depending on what framework you’re using, the name may vary, but the intent is the same: make sure that the form of the SQL statement that you want to execute is correct prior to running it.
