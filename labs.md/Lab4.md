# Lab Name - User role can be modified in user profile

## Vulnerability

Vertical Privilege Escalation

## Objective

Access the admin functionality as a non-admin user using to change the Roleid . 

## Steps

1. First, logged in as the normal "wiener" user using the password "carlos".

2. Turned on Intercept and captured the traffic using Burp Suite.

3. Sent the HTTP request to Burp Repeater.

4. In the HTTP JSON Request, modified the parameter after priority header . 
5. add the role id to 2 aftr email 

6. Clicked **Send** and received a "200-OK" response.
   
7. refresh the lab page and admin panel shows

8. after getting admin panel delete the  user carlos . 

## Result

Successfully accessed the admin functionality as a low-privileged user.

## Key Learning

Access control must be properly validated and the check the role and permission related to users. 

proof of concept 
!["header code "](lab4vertical.png)
![solved lab ](lab4vertical1.png)