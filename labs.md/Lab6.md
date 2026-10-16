# Lab Name - User role can be modified in user profile

## Vulnerability

Horizontal Privilege Escalation

## Objective

Access the admin functionality as a non-admin user using to change the Roleid . 

## Steps

1. First, logged in as the normal "wiener" user using the password "carlos".

2. Turned on Intercept and captured the traffic using Burp Suite.

3. Sent the HTTP request to Burp Repeater.

4. In the HTTP JSON Request change the username **wiener** to **carlos** 
5. 

6. Clicked **Send** and received a "200-OK" response.
   
7. in response get the carlos **api key** 

8. after getting admin panel delete the  user carlos . 

## Result

Successfully accessed the other user account . 

## Key Learning

server must check the  username id  name . so that they donot validate unauthroized access .

proof of concept . 
![http resonpse ](horizontallab1.png.png)
![solved lab ](horizontallab1(2).png.png)
