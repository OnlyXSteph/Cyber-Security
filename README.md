# Project 9 - Pen Testing Live Targets

Challenge Goals: 

### Username Enumeration

The vulnerability is on the GREEN site. 

The existing user "jmonroe99" allows us to compare the responses we get after testing with an 
existing user and a nonexisting user. This vulnerability allows us to find out whether a username 
exists since the text response for "jmonroe99" is in bold and responses for nonexisting usernames 
are not. 

<img src="usrn_enum.gif" alt="Username Enumeration">
 
### Insecure Direct Object Reference

The vulnerability is on the RED site. 

The id parameter can be modified and generates new GET requests that allow us to view the details 
of some sales people. The ids 10, 11 and 12 give access to pages for 3 otherwise unlisted sales 
people: Testy McTesterson, Lazy Lazyman and John Wick. This vulnerability doesn't exist on the 
Blue and Green sites since illegal id requests will redirect the user to the salesperson page. 


<img src="idor.gif" alt="Insecure Direct Object Reference">

### SQL Injection

The vulnerability is on the BLUE site. 

The site is vulnerable to SQL injection attacks because we can use a URL encoded SQL command 
that makes the database sleep for 5 seconds. 

<img src="SQLI.gif" alt="SQL Injection">

### Cross-Site Scripting

The vulnerability is on the GREEN site.

On the contact page, the contact form's feedback section allows you to enter some javascript that 
can be executed by the browser. 

<img src="cs_scripting.gif" alt="Cross-Site Scripting">

### Cross-Site Request Forgery

<img src="cs_req_forg.gif" alt="Cross-Site Request Forgery">

### Session Hijacking/Fixation

<img src="shf.gif" alt="Session Hijacking/Fixation">
