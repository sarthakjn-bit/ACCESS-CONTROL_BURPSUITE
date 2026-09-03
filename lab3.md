# Lab: User Role Controlled by Request Parameter

**Vulnerability:** Vertical Privilege Escalation

**Objective:** Access the admin functionality as a non-admin user.

**Steps:**

1. Open Burp Suite and capture the traffic.
2. Log in as the normal wiener:peter user.
3. Click on the **Admin panel** and observe that access is denied.
4. Log in as the administrator using the `dmin account.
5. Send the HTTP request for /admin/login to Burp Repeater.
6. Replace the administrator's cookie with the non-admin user's cookie.
7. Change the `admin=false
8.  parameter to `admin=true and send the request.
9. Access the Admin panel and delete the user carlos.

**Result:** Successfully accessed admin functionality as a low-privileged user.

**Key Learning:** Authorization must be validated server-side; changing role parameters should not grant access.