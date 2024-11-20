# Manual-Testing-Project

## Overview

This repository documents the manual testing efforts for the [Prestashop demo e-commerce platform](https://demo.prestashop.com/#/en/front). The project focuses on validating the core functionalities, usability, performance, and security aspects of the application within the scope of a front-end, client-side perspective. 

## Scope and Limitations

### Scope
The tests performed in this project include:
- **Functional Tests**: Registration, sign-in, checkout processes, cart operations, and wishlist functionality.
- **Usability Tests**: Evaluating user interface elements, navigation, and responsiveness.
- **Performance Tests**: Measuring page load times, Time to Interactive (TTI), JavaScript execution, and CSS rendering times under normal conditions.
- **Security Tests**: Client-side security checks, including SQL injection attempts, cross-site scripting (XSS), and user authentication mechanisms.

### Limitations
- **No Database Access**: Tests are limited to client-side interactions; backend database operations were not tested.
- **No Backend-Level Operations**: Server-side validations and API interactions were not directly tested.
- **No Multi-User Workload Simulations**: Performance tests were conducted as a single user and did not simulate concurrent user activity or server load.
- **Security Tests**: Limited to surface-level vulnerabilities and client-side validations.

## Tools Used
- **Browser Testing**: Google Chrome (latest), Microsoft Edge (latest).
- **Test Case Management**: Qase.
- **Test Documentation**: Google Docs.
- **Recording and Debugging**: JAM extension, Chrome Developer Tools.
- **Performance Analysis**: Lighthouse, Chrome Developer Tools.

## Test Types and Results
### Test Types
1. **Manual Functional Testing**: 26 test cases for both signed-in and non-signed-in user workflows.
2. **Usability Testing**: 2 test cases for homepage navigation in Google Chrome and Microsoft Edge.
3. **Performance Testing**: 5 test cases measuring page load speed, TTI, and other client-side performance metrics.
4. **Security Testing**: 6 test cases covering client-side vulnerabilities such as XSS, SQL injection, and password security.

### Defects Identified
A total of **9 defects** were reported, including:
- Incorrect error messages for purchase limits.
- Missing functionalities (e.g., wishlist for non-signed-in users).
- Suboptimal performance metrics (e.g., homepage load time exceeding 3 seconds).
- Security vulnerabilities such as unlimited login attempts without a CAPTCHA or lockout.

Detailed defect reports and test cases can be found in this repository and in the linked [Qase Project](https://app.qase.io/defect/DEMO?status=%5B0%5D).

## Key Achievements
- Comprehensive manual testing of critical workflows and surface-level vulnerabilities.
- Identified performance bottlenecks in page load time and JavaScript execution.
- Highlighted areas requiring improvements in user authentication and security.

## Contribution
This project is currently closed for contributions as it represents a testing effort for a specific demo environment. However, feedback and suggestions are welcome!

---
