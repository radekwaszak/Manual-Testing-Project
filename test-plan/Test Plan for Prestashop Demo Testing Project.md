### **Test Plan for Prestashop Demo Testing Project**

---

### **1\. Project Overview**

The purpose of this project is to assess the quality and functionality of the Prestashop demo e-commerce platform by conducting tests in areas such as functionality, usability, performance, and security. The testing process is focused on identifying bugs, ensuring compliance with specified requirements, and improving system behavior. Testing will include both manual and automation strategies, with adjustments based on the tools and scope available.

---

### **2\. Audience**

This test plan is intended for the following stakeholders:

* **Test Team**: Manual testers, usability testers, and security specialists.  
* **Development Team**: Addressing defects identified during testing.  
* **Project Managers**: Ensuring testing aligns with the timeline and project goals.  
* **Product Owners**: Validating that the platform meets business requirements.

---

### **3\. Test Assumptions**

* The demo version of Prestashop is a representative environment for production use.  
* All required tools (e.g., Newest versions of Google Chrome & Microsoft Edge browsers, built-in browser developer tools, Lighthouse, Qase, JAM, Dr Link Check, Google Docs) will be accessible.  
* Stakeholders will provide timely responses to queries related to requirements or functionality.

---

### **4\. Levels and Types of Testing**

**Levels of Testing**:

1. **Unit Testing**: Conducted by developers (not covered in this plan).  
2. **Integration Testing**: Verify interactions between modules.  
3. **System Testing**: Evaluate the entire Prestashop platform.  
4. **User Acceptance Testing (UAT)**: Final validation before deployment.

**Types of Testing**:

1. **Functional Testing**: Focus on user workflows (e.g., registration, sign-in process, cart management, wishlist management, searching and filtering products, checkout process).  
2. **Usability Testing**: Evaluate ease of use and user experience.  
3. **Performance Testing**: Measure page load time, TTI, and resource performance for single-user scenarios.  
4. **Security Testing**: Identify vulnerabilities such as SQL Injection, XSS, and session management issues.

---

### **5\. Scope of Testing**

* **In-Scope**:  
  * Core functionalities like registration, login, shopping cart, and checkout processes.  
  * Usability aspects such as navigation and ease of interaction.  
  * Performance tests focusing on metrics like page load time, JavaScript execution, and CSS rendering for a single user.  
  * Security tests targeting common vulnerabilities without requiring database access.  
* **Out-of-Scope**:  
  * Backend/database testing (e.g., database queries, server-side logs).  
  * Integration with third-party services.  
  * Multi-user load testing or concurrency testing.

---

### **6\. Test Deliverables**

1. **Test Plan Document** (this document).  
2. **Test Cases**: Detailed manual test scripts for usability, performance, and security tests.  
3. **Test Execution Reports**: Results of executed test cases.  
4. **Defect Reports**: Logs of identified bugs, their severity, and priority.  
5. **Performance and Security Reports**: Single-user analysis and vulnerability assessments.  
6. **Test Summary Report**: Consolidated findings and recommendations.

---

### **7\. Test Effort Estimation**

* **Functional Testing**: 1 functional tester, \~3 working days for 26 planned tests.  
* **Performance Testing**: 1 performance engineer, \~1 working day for 5 tests.  
* **Security Testing**: 1 security specialist, \~1 working day for 6 planned tests.  
* **Usability Testing**: 1 usability tester, \~1 working day for 2 planned tests.  
* **Automation Testing**: To be planned after manual testing is completed.

---

### **8\. Entry and Exit Criteria**

**Entry Criteria**:

* Test environment is fully set up and accessible.  
* Business documentation is available.  
* All necessary tools and test data are available.  
* Approved test cases are documented and reviewed.

**Exit Criteria**:

* All planned tests are executed.  
* Retests have been completed  
* All critical and high-priority defects are resolved or mitigated.  
* Test summary report is submitted to stakeholders.

---

### **9\. Validation and Defect Management**

* **Validation**: Test execution results will be validated against the requirements to ensure the system behaves as expected.  
* **Defect Management**:  
  * Defects will be logged in the defect-tracking tool (Qase).  
  * Each defect will include detailed reproduction steps, severity, priority, and supporting artifacts (e.g., screenshots, screen recordings, code snippets, HAR files).  
  * Each defect report will be forwarded to the development team.  
  * Defects will be fixed by developers and forwarded to retest.  
  * Retests will be performed.  
  * Error occurs \= back to debugging / error fixed \= closing the defect report.

---

### **10\. Test Metrics**

|  Metric |  Formula |
| :---: | :---: |
| Percentage test cases executed | No of test cases executed/ Total no of test cases written X 100 |
| Passed Test Cases Percentage | Number of Passed Tests/Total number of tests executed X 100 |
| Failed Test Cases Percentage | Number of Failed Tests/Total number of tests executed X 100 |

---

### **11\. Test Risks and Mitigation Factors**

**Risks**:

* Limited access to backend systems may restrict test coverage.  
* Unclear or incomplete requirements could lead to misaligned testing.  
* Performance issues during testing may delay timelines.  
* Testing single-user scenarios may not fully represent real-world performance.

**Mitigation**:

* Collaborate with developers to simulate backend scenarios.  
* Seek clarifications on requirements before testing.

---

### **12\. Test Responsibility**

1. **QA team**  
* Developing a test plan  
* Executing tests  
* Analyzing requirements  
* Creating test cases  
* Reporting (defects, summary)  
* Retesting  
* Monitoring the test process  
2.  **Development team**  
* Fixing defects  
* Writing code  
* Writing unit tests  
* Debugging  
* Code review  
3. **Test Manager**  
* Oversee test planning, execution, and reporting

**13\. Test Environment**

1. **Functional and Usability Testing**:  
   * Tools: Newest versions of Google Chrome and Microsoft Edge, DevTools, JAM for test recordings, Qase for reporting test results, defects.  
   * Devices: Windows 10 desktop.  
2. **Performance Testing**:  
   * Tools: Newest version of Google Chrome, DevTools, Lighthouse, Qase for reporting test results, defects.  
   * Focused on single-user scenarios.  
   * Devices: Windows 10 desktop.  
3. **Security Testing**:  
   * Tools: Newest version of Google Chrome, DevTools, Qase for reporting test results, defects.  
   * Devices: Windows 10 desktop.

---

### **14\. Test Execution Plan**

* Functional Testing: Validate major workflows, including signed-in and non-signed-in scenarios.  
* Usability Testing: Evaluate the website's ease of use and navigation.  
* Performance Testing: Assess key metrics (e.g., page load time, TTI, JavaScript execution).  
* Security Testing: Perform SQL injection, XSS, and password security assessments without backend access.

**15\. Testing Tools**  
 

| Area | Tool |
| ----- | ----- |
| Creating documentation \- test plan, test cases, test run reports, defect report, final report | Qase, Google Docs |
| Performance and accessibility audits | Lighthouse |
| Broken links checker | Dr. Link Check |
| Test execution | Google Chrome (version 131.0.6778.70, 64-bit) Microsoft Edge (version 131.0.2903.51, 64-bit) Developer Tools |
| Screen recording | JAM |
| Screenshots | Windows Snipping Tool |

