# Lab: Unprotected Admin Functionality

**Lab Name:** Unprotected Admin Functionality with Unpredictable URL

**Vulnerability:** Vertical Privilege Escalation

**Objective:** Access the admin functionality as a non-admin user.

**Steps:**

1. Open Developer Tools in the browser.
2. Go to the **Network ** tab and inspect the relevant JSON response.
3. Identify and copy the admin URL from the admin panel.
4. Paste the admin URL into the browser while logged in as a non-admin user.
5. The non-admin user was able to access the admin functionality.

**Result:** Successfully accessed admin functionality as a low-privileged user.

**Key Learning:** Hiding or making an admin URL difficult to discover does not provide access control. 
The server must verify whether the user is authorized to access the functionality. 