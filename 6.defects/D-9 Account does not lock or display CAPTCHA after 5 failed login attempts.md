

| ID number | D-9 |
| :---- | :---- |
| Name | Account does not lock or display CAPTCHA after 5 failed login attempts |
| Reporter | Radosław W. |
| Submit Date | 17/11/2024 |
| Summary |  The website does not lock the user account or display a CAPTCHA after 5 failed login attempts. According to the requirements, the system should block further login attempts for 24 hours after 5 consecutive failed attempts to prevent brute-force attacks. Currently, the system allows unlimited attempts, exposing it to potential security threats. |
| Environment | Browser: Chrome 131.0.6778.70 (64-bit) Platform: Windows 10 Device: Desktop Network: High-speed broadband connection PrestaShop Version: Demo version ([https://demo.prestashop.com/\#/en/front](https://demo.prestashop.com/#/en/front))  |
| Severity | **Critical** |
| Assigned to | / |
| Priority | **High** |

**Steps to Reproduce:**

1. Navigate to the login page of the Prestashop demo website ([https://demo.prestashop.com/\#/en/front](https://demo.prestashop.com/#/en/front)).   
2. Enter a valid email address but an incorrect password.  
3. Repeat step 2 five times consecutively without a successful login.  
4. Attempt to log in again with an incorrect password after the 5th failed attempt.

   

**Expected Result:** After 5 failed login attempts, the system should lock the account for 24 hours and display a message informing the user that their account is temporarily locked.

**Actual Result:** The account remains unlocked and allows unlimited login attempts after 5 failed attempts, violating the security requirements.

**Suggested Fix:** 

* Implement Account Lock Mechanism \- lock the account for 24 hours after 5 failed login attempts, store the count of failed attempts and the timestamp in the database.  
* Introduce CAPTCHA \- display a CAPTCHA after a specified number of failed attempts (e.g., 3).  
* Display Informative Message \- notify the user when the account is locked and provide guidance for unlocking (e.g., contact support or wait 24 hours).  
* Log Failed Attempts; ensure all failed login attempts are logged for monitoring and security purposes.
