# Lab Name - Unprotected Admin Functionality

## Vulnerability

Vertical Privilege Escalation

## Objective

Access the admin functionality as a non-admin user.

## Steps

1. First, logged in as the normal "wiener" user using the password "carlos".

2. Turned on Intercept and captured the traffic using Burp Suite.

3. Sent the HTTP request to Burp Repeater.

4. In the HTTP request, modified the URL by adding "robots.txt at the end.

5. Clicked **Send** and received a "200-OK" response.

6. Pasted the URL into the lab page and accessed the **Admin** functionality.

## Result

Successfully accessed the admin functionality as a low-privileged user.

## Key Learning

Access control must be properly validated on the server side.