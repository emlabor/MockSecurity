# Mock Security
This project was created for *CSCI-UA 9480*, Introduction to Computer Security. I performed four different attacks on DVWA, the Damn Vulnerable Web Application. Full report available in PDF.

#### Attack 1: Blind SQL Injection  
For the first attack I use a blind SQL injection to steal users’ authentication information from the DVWA database. The attack is similar to a regular SQL injection except little to no feedback is displayed onscreen, so I have to do more guessing. For this I use Burp Suite and the SQL injection tool SQLMap. 

#### Attack 2: Weak Session IDs 
In this attack I exploit DVWA’s insecure generation of session IDs. Communicated via cookies, session IDs indicate to the site which user is logged in so that they do not have to continually authenticate themselves. These IDs should be hard to guess and drawn from a large address space so that users’ sessions cannot be impersonated.

#### Attack 3: Stored XSS  
A cross site scripting attack (XSS) involves injecting a malicious script (typically JavaScript) into an otherwise trusted website so that users of the site unknowingly execute the attacker’s code. In a stored XSS attack, the injection persists in the database until manually removed, giving it the capacity for widespread damaging consequences.

#### Attack 4: Brute Force  
The last attack is to try to guess the admin’s password by brute force. This is a relatively unsophisticated strategy but provides the opportunity to work with some new tools. I use Burp Suite, as before, and Hydra.



