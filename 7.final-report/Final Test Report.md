### **Final Test Report for Prestashop Demo Testing Project**

---

#### **1\. Introduction**

The purpose of this document is to summarize the results, findings, and insights gained during the testing of the Prestashop e-commerce demo website ([https://demo.prestashop.com/\#/en/front](https://demo.prestashop.com/#/en/front)). The primary objective was to evaluate the functionality, usability, performance, and security of the system to ensure it meets business requirements and provides a seamless user experience.

---

#### **2\. Scope of Testing**

The testing scope included the following:

1. **Functional Testing**:  
   * Registration and Sign-in workflows for signed-in and non-signed-in users.  
   * Shopping cart, wishlist, and checkout processes.  
   * Filters and search functionalities.  
2. **Usability Testing**:  
   * Homepage navigation and ease of performing core workflows.  
3. **Performance Testing**:  
   * Evaluated page load time, Time to Interactive (TTI), JavaScript execution time, CSS rendering time, and browser resource completion.  
4. **Security Testing**:  
   * Tested client-side vulnerabilities like SQL Injection, Cross-Site Scripting (XSS), authentication security, and sensitive data handling.

---

#### **3\. Summary of Testing Activities**

* **Total Test Cases Executed**: 39  
  * 5 Registration/Sign-in Functional Tests  
  * 11 Non-signed-in User Functional Tests  
  * 10 Signed-in User Functional Tests  
  * 2 Usability Tests  
  * 5 Performance Tests  
  * 6 Security Tests  
* **Tools Used**:  
  * **Test Management**: Qase (test case creation, execution, and defect tracking)  
  * **Documentation**: Google Docs  
  * **Web Browsers**: Google Chrome (latest version), Microsoft Edge (latest version)  
  * **Performance Tools**: DevTools, Lighthouse  
  * **Usability**: JAM extension for test recordings  
  * **Accessibility and Audit Reports**: Lighthouse

**4\. Test Results**

#### 

| Test Type | Total Tests | Passed | Blocked | Failed | Defects Identified |
| :---- | :---- | :---- | :---- | :---- | :---- |
| Functional (Registration) | 5 | 5 | 0 | 0 | 0 |
| Functional (Signed-in) | 10 | 8 | 0 | 2 | 2 |
| Functional (Non-signed-in) | 11 | 5 | 2 | 4 | 4 |
| Usability | 2 | 2 | 0 | 0 | 0 |
| Performance | 5 | 3 | 0 | 2 | 2 |
| Security | 6 | 5 | 0 | 1 | 1 |
| Total | 39 | 28 | 2 | 9 | 9 |

#### 

#### Percentage test cases executed – 95%

#### Passed Test Cases Percentage – 72%

#### Failed Test Cases Percentage – 23%

**Note**:

A total of **6 test runs** were performed to ensure consistency and to validate test outcomes across multiple attempts. Screenshots from run reports exported from Qase will be included as part of this report for reference.

#### ---

#### **5\. Key Findings**

1. **Functional Defects**:  
   * **Shopping Cart**: Both signed-in and non-signed-in users encountered issues modifying product sizes from the cart level.  
   * **Wishlist**: Temporary wishlist functionality was unavailable for non-signed-in users.  
   * **Checkout**: Non-signed-in users could not complete the payment process due to missing fields for card details.  
2. **Usability Defects**:  
   * The homepage exceeded the 3-second load time requirement (observed 14.5 seconds), impacting user experience.  
3. **Performance Defects**:  
   * JavaScript execution exceeded the 1-second limit (observed 2.7 seconds).  
4. **Security Defects**:  
   * Account locking and CAPTCHA functionality were missing after five failed login attempts, leading to potential brute-force vulnerability.  
   * 

**6\. Test Coverage and Effectiveness**

* **Coverage**: Achieved comprehensive testing across the core functionalities, performance metrics, and security requirements as per business requirements.  
* **Effectiveness**: Successfully identified 9 critical defects, with focus areas for improvement being performance and security.

---

#### **7\. Defect Details**

#### 

| Defect ID | Title | Severity | Priority | Status |
| :---- | :---- | :---- | :---- | :---- |
| D-1 | Incorrect error message for maximum purchase order quantity (non-signed-in user) | Normal | Medium | Open |
| D-2 | Non-signed-in user unable to change product size from the cart level | Normal | Medium | Open |
| D-3 | Non-signed-in user cannot add products to a temporary wishlist | Normal | Medium | Open |
| D-4 | Unable to complete checkout as non-signed-in user: missing payment fields | Blocker | High | Open |
| D-5 | Incorrect error message for maximum purchase order quantity (signed-in user) | Normal | Medium | Open |
| D-6 | Signed-in user unable to change product size from the cart level | Major | High | Open |
| D-7 | Homepage loads in more than 3 seconds | Major | High | Open |
| D-8 | JavaScript execution time exceeds 1 second (2.7 seconds observed) | Normal | Medium | Open |
| D-9 | Account does not lock or display CAPTCHA after 5 failed login attempts | Critical | High | Open |

#### ---

#### **8\. Test Deliverables**

* Test Cases: Created and managed in Qase.  
* Defect Reports: Logged in Qase with detailed descriptions, steps to reproduce, and screenshots/recordings.  
* Performance Reports: Generated using Lighthouse and Chrome DevTools.  
* Accessibility Reports: Produced using Lighthouse for audit compliance.

**9\. Observations and Recommendations**

* **Functional Improvements**: Resolve cart and wishlist issues for non-signed-in users to ensure feature parity with signed-in workflows.  
* **Performance Optimization**: Optimize JavaScript execution and homepage load times.  
* **Security Enhancements**: Implement account locking and CAPTCHA after failed login attempts.  
* **Testing Gaps**: Future testing should include multi-user performance scenarios and deeper database-level security assessments.

---

#### **10\. Conclusion**

The Prestashop demo platform exhibits several critical defects that need immediate attention, especially in the areas of performance and security. While usability and functionality were adequately validated, further rounds of testing are recommended after defect resolution to ensure a production-ready system.

