# **Business Requirements Document for Prestashop Demo**

## **Overview**

The Prestashop demo website must deliver a seamless, functional, secure, and efficient user experience while adhering to performance and usability benchmarks. The requirements outlined here encompass functional workflows, security protocols, usability, and performance criteria. These will serve as a baseline for evaluating the platform during the testing phase.

### **1\. Functional Requirements**

#### **1.1 Cart Management**

1.1.1. Users (both signed-in and non-signed-in) can add products to the shopping cart. The cart icon must update to reflect the number of items, and a green toast message confirming the addition must appear.  
1.1.2. The maximum quantity of any product in the cart is 400\. If the quantity exceeds this limit, the user should see the red toast message: *“The available purchase order quantity for this product is 400”*.  
1.1.3. Both signed-in and non-signed-in users can modify product size and quantity directly from the cart view.  
1.1.4. Both signed-in and non-signed-in users can proceed to checkout directly from the cart view.

#### **1.2 Wishlist Functionality**

1.2.1. Signed-in users can create and manage multiple wishlists.  
1.2.2. Products added to a wishlist must display a success green toast message: *“Product Added”*. A dialog box should appear allowing users to select the list to save the product in.  
1.2.3. Non-signed-in users can add products to their wishlist. Wishlists persist for 24 hours for temporary lists unless explicitly saved.  
1.2.4. Users can remove products from a wishlist. Clicking the trash icon prompts a confirmation window with the message: *“The product will be removed from My Wishlist”*. Upon confirmation, a green toast message: *“Product successfully removed”* appears.

#### **1.3 Search Functionality**

1.3.1. Users can search for products using the search bar.  
1.3.2. If the search query does not match any items in the inventory, the platform must suggest alternative products based on relevance.

#### **1.4 Filtering and Sorting Requirements**

1.4.1. Users can filter products by single criteria such as category, price, or composition.  
1.4.2. Users can apply multiple filters simultaneously.   
1.4.3. Filters must update dynamically without requiring a page refresh.

#### **1.5 Registration and Authentication**

1.5.1. Registration:

* If an incorrect email format is provided, a red toast message must appear indicating the issue.  
* If required fields or checkboxes are left unfilled, appropriate validation messages should guide the user to complete them.  
* Weak passwords must be rejected with a message prompting the user to create a stronger password. Passwords must be between 8 and 72 characters long.

1.5.2. Signing In:

* Invalid email or password inputs must result in an error message.  
* After five failed login attempts, the account must be locked for 24 hours, with a message informing the user of the temporary lock.


#### **1.6 Checkout Process**

1.6.1. Payment Options:

* Non-signed-in users can pay only via credit/debit card, with fields available for entering card details.  
* Signed-in users have access to the following payment methods: "Pay by bank wire," "Pay by cash on delivery," and "Pay by check." Debit/credit card payment is unavailable for signed-in users.  
* To place an order, users must first check the checkbox confirming the Terms and Conditions. After clicking "Place an order", the page displays an appropriate message and a summary of the order.

1.6.2. Shipping Options:

* Non-signed-in users can use only the "My Carrier" shipping method, selected by default.  
* Signed-in users can choose between "Click and Collect" (Pick-up in store) and "My Carrier."

### **2\. Performance Requirements**

#### 2.1 Homepage must load fully within 3 seconds under normal internet conditions.  
#### 2.2 Time to Interactive (TTI) should not exceed 5 seconds.  
#### 2.3 CSS rendering must complete within 2 seconds after HTML load.  
#### 2.3 JavaScript execution time must remain below 1 second.  
#### 2.4 CPU and memory usage should stay under 50% during peak operations.

### **3\. Security Requirements**

#### 3.1. Input fields across the platform must be sanitized to prevent SQL Injection and Cross-Site Scripting (XSS) attacks.  
#### 3.2. User authentication mechanisms must ensure secure password storage and hashing.  
#### 3.3. Session management must protect against session hijacking or fixation attacks.  
#### 3.4. Sensitive data (e.g., passwords, card details) must be transmitted over HTTPS.  
#### 3.5. Password policies must enforce strong passwords and prevent reusing old passwords.

### **4\. Usability Requirements**

#### 4.1. Navigation: The platform must provide an intuitive user interface, ensuring key sections (e.g., cart, wishlist, search) are easily accessible within three clicks from the homepage.  
#### 4.2. Error Messages: Validation and error messages must be clear, concise, and context-specific.  
#### 4.3. Mobile Responsiveness: The platform must be fully responsive and optimized for mobile devices.  
#### 4.4. JAM integration must support visual test recordings to facilitate usability assessment.

### **5\. Additional Requirements**

#### 6.1. Accessibility: The platform must adhere to WCAG 2.1 guidelines for accessibility, ensuring usability for all users, including those with disabilities.  
#### 6.2. Language Support: The website must support at least two languages (e.g., English and French) with a toggle feature for users.  
#### 6.3. Logging: Key user actions (e.g., login, checkout, and wishlist updates) must be logged for auditing and troubleshooting purposes.  
#### 6.4. Support for Scalability: The platform should be easily scalable to handle increased traffic and users.

