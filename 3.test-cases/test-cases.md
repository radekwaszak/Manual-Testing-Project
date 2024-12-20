# **TC-01 Verify successful registration with valid data**
Validate that a user can successfully register with valid details

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Critical | High | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User is on the registration page; registration form is visible.

## **Post-conditions**
A new account is created and the user is redirected to the dashboard, signed-in.

## **Steps**

### **Step	1**
Action: Select the appropriate social title radiobutton \- Mr. or Mrs.

Expected: result	The appropriate radiobutton is selected.

### **Step	2**
Action: Enter a valid first name, last name, and email.

Expected result: Text fields populate with the entered information.

### **Step	3**
Action: Enter a strong, valid password.

Expected result: Password is accepted and hidden behind asterisks or similar masking.

### **Step	4**
Action: Complete the optional field \- birthdate.

Expected result:	Text fields populate with the entered information.

### **Step	5**
Action: Accept terms and conditions.

Expected result:	Checkbox is selected.

### **Step	6**
Action: Accept customer data privacy.

Expected result:	Checkbox is selected.

### **Step	7**
Action: Click the "Save" button.

Expected result:	User is successfully registered and redirected to the dashboard, signed-in.

# **TC-02 Verify registration fails with invalid email format**
Validate that the system rejects registration attempts with an invalid email format.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Critical | High | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User is on the registration page.

## **Post-conditions**
No account is created; the user remains on the registration page with an error message.

## **Steps to reproduce**

### **Step	1**
Action: Select the appropriate social title radiobutton \- Mr. or Mrs.

Expected result: The appropriate radiobutton is selected.

### **Step	2**
Action: Enter a valid first name and last name.

Expected result: Text fields populate with the entered information.

### **Step	3**

Action:	Enter an invalid email format (e.g., "user@domain").

Expected result:	Email field accepts input, but format does not meet validation criteria.

### **Step	4**
Action: Enter a strong, valid password.

Expected result:	Password is accepted and hidden behind asterisks or similar masking.

### **Step	5**
Action:	Accept terms and conditions.

Expected result:	Checkbox is selected.

### **Step	6**
Action: Accept customer data privacy.

Expected result:	Checkbox is selected.

### **Step	7**

Action:	Click the "Save" button.

Expected result:	Registration fails; an error message indicating "Invalid email format" is displayed.

# **TC-03 Verify registration fails with unchecked mandatory checkbox**
Validate that the system rejects registration attempts with the “Customer Data Privacy” checkbox not checked.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Critical | High | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User is on the registration page.

## **Post-conditions**
No account is created; the user remains on the registration page with an information message “Check this box if you want to continue” displayed.

## **Steps**

### **Step	1**
Action:	Select the appropriate social title radiobutton \- Mr. or Mrs.

Expected result: The appropriate radiobutton is selected.

### **Step	2**
Action:	Enter a valid first name, last name, and email.

Expected result: Text fields populate with the entered information.

### **Step	3**
Action:	Enter a strong, valid password.

Expected result: Password is accepted and hidden behind asterisks or similar masking.

### **Step	4**
Action:	Accept terms and conditions.

Expected result: Checkbox is selected.

### **Step	5**
Action:	Click the "Save" button.

Expected result: Registration fails; an information message indicating “Check this box if you want to continue” is displayed.

# **TC-04 Successful login with valid credentials**
Verify that a user can successfully sign in with valid credentials.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Critical | High | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User has a registered account; login page is accessible.

## **Post-conditions**
User is signed-in and directed to the dashboard.

## **Steps**

### **Step	1**
Action:	Enter valid email and password.

Expected result:	Credentials are entered correctly and match stored user data.

### **Step	2**
Action:	Click the "Sign In" button.

Expected result:	Login is successful; user is redirected to the dashboard.

# **TC-05 Verify login fails with incorrect password**
Ensure login fails when an incorrect password is entered.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Critical | High | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User has a registered account; login page is accessible.

## **Post-conditions**
User remains on the login page with an error message indicating incorrect credentials.

## **Steps**

### **Step	1**
Action:	Enter a valid email but an incorrect password.

Expected result:	Incorrect password is accepted into the password field.

### **Step	2**
Action:	Click the "Sign In" button.

Expected result:	Login fails; an error message stating "Authentication failed" appears.

# **TC-06 Verify search functionality with valid product name (non-signed- in user)**

Confirm that searching with a valid product name returns relevant results for non-signed-in user.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Major | High | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User is not signed-in. Products are available in the system; search bar is accessible.

## **Post-conditions**
Search results page displays products matching the search term.

## **Steps**

### **Step	1**
Action:	Enter a specific product name (e.g., "T-shirt") into the search bar.

Expected result:	Product name is accepted and visible in the search bar.

### **Step	2**
Action:	Click 'Enter'.

Expected result:	Relevant search results matching the product name are displayed.

# **TC-07 Verify adding a single product to the cart (non-signed-in user)**

Validate that a non-signed-in user can add a single item to the shopping cart.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Major | High | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User is not signed-in and has navigated to the random product page.

## **Post-conditions**
Product is added to the cart, and cart count updates accordingly.

## **Steps**

### **Step	1**
Action:	Search for the product and navigate to its product page.

Expected result:	Product page for the selected book is displayed.

### **Step	2**
Action:	Click the "Add to Cart" button.

Expected result:	Product is added to the cart; cart icon updates to reflect the added item.

# **TC-08 Verify adding products to the cart in different variants and quantities (non-signed-in user)**
Validate that a non-signed-in user can add different products to the cart after changing their details such as size, color, quantity.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Critical | High | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User is not signed-in and has navigated to the random product page.

## **Post-conditions**
Products are added to the cart in the appropriate variants that the user has selected.

## **Steps**

## **Step	1**
Action:	Search for the product and navigate to its product page.

Expected result:	Product page for the selected item is displayed.

## **Step	2**
Action:	Change product size, color and quantity (for example to 15).

Expected result:	Product details changed accordingly.

## **Step	3**
Action:	Click the "Add to Cart" button.

Expected result:	Product is added to the cart; cart icon updates to reflect the added item.

## **Step	4**
Action:	Search for another product and navigate to it's page.

Expected result:	Product page for the selected item is displayed.

## **Step	5**
Action:	Change product size, color and quantity (for example to 15).

Expected result:	Product details changed accordingly.

## **Step	6**
Action:	Click the "Add to Cart" button.

Expected result:	Product is added to the cart; cart icon updates to reflect the added item.

# **TC-09 Verify product quantity change from the cart level (non-signed- in user)**
Validate that a non-signed-in user can change product quantity in the “Shopping Cart” page.

| Severity | Priority | Behavior | Type |
| :---- | ----- | :---- | :---- |
| Normal | Medium | Not set | Other |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User is not signed-in and has navigated to the “Shopping Cart” page. There is a clothing product in the cart, e.g. a T-shirt.

## **Post-conditions**
The product with the changed quantity is in the cart.

## **Steps**

### **Step 1**
Action:	Change the number of products in the cart, e.g. to 20\.

Expected result:	Product number changed to 20, price recalculated according to the new quantity.

### **Step 2**
Action:	Change the number of products in the cart to 401\.

Expected result:	An error message appears “The available purchase order quantity for this product is 400".

# **TC-10 Verify product size change from the cart level (non-signed-in user)**
Validate that a non-signed-in user can change product size in the “Shopping Cart” page.

| Severity | Priority | Behavior | Type |
| :---- | ----- | :---- | :---- |
| Normal | Medium | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User is not signed-in and has navigated to the “Shopping Cart” page. There is a clothing product in the cart, e.g. a T-shirt.

## **Post-conditions**
The product with the changed size is in the cart

## **Steps**

### **Step 1**
Action:	Change the product size, using drop-down list for the product.

Expected result	Product size has changed.

# **TC-11 Verify adding a product to wishlist (non-signed-in user)**
Verify that a non-signed-in user can add products to the wishlist.

| Severity | Priority | Behavior | Type |
| :---- | ----- | :---- | :---- |
| Normal | Medium | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User is not signed-in; they are on the product page of an item they want to add to the wishlist.

## **Post-conditions**
Product is added to the temporary wishlist. The wishlist is cleared later after 24 hours.

## **Steps to reproduce**

### **Step 1**
Action:	Navigate to a product page (e.g., "T-shirt") without signing in.

Expected result: Product page is displayed with all product information and options, including the "Add to Wishlist" heart-sha ped button.

### **Step 1**
Action:	Click the "Add to Wishlist" button.

Expected result: The product is added to a temporary wishlist that will be cleared after 24 hours.

# **TC-12 Verify removing a product from wishlist (non-signed-in user)**
Verify that a non-signed-in user can remove products from the wishlist.

| Severity | Priority | Behavior | Type |
| :---- | ----- | :---- | :---- |
| Normal | Medium | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User is not signed-in; they are on the temporary wishlist page with the product added to this list.

## **Post-conditions**
Product is removed from the temporary wishlist.

## **Steps**

### **Step 1**
Action:	Click on the button in the shape of trash can in the product preview image.

Expected result: A window appears to confirm the execution of the action "The product will be removed from wishlist".

### **Step 2**
Action:	Click “Remove”.

Expected result: A green toast message "Product successfully removed" appears on the screen.

# **TC-13 Verify filter by singe criteria (non-signed-in user)**
Verify that applying single filter displays only products that belong to the selected criteria for non-signed-in user.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Normal | High | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User is not signed-in. Multiple products are available across different categories, and the user is on the product search or category page.

## **Post-conditions**
The page should display only products in the selected criteria or reset to the default product view if filters are cleared.

## **Steps**

### **Step 1**
Action:	Select “Clothes” category and then apply a specific filter (e.g., "Men").

Expected result: The filter is selected, and the page shows a loading spinner or indicator that the filter is being applied. The page automatically reloads and shows clothes only from the “Men” category. No products from other categories are sho wn.

# **TC-14 Verify filter by multiple criteria (non-signed-in user)**
Validate that applying multiple filters together narrows down the product search results to meet all selected criteria for non- signed-in user.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Normal | High | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User is not signed-in. Products are available across different categories and price ranges.

## **Post-conditions**
The page should display only products that match the applied criteria or reset to the default product view if filters are cleared.

## **Steps**

### **Step 1**
Action:	Select “Accessories” category and then apply a specific filter (e.g., Composition “Polyester”).

Expected result: The filter is selected, and the page shows a loading spinner or indicator that the filter is being applied. The page automatically reloads and shows Polyester accessories.  No accessories of other composition are shown.

### **Step 2**
Action:	Apply an additional filer e.g., Composition “Recycled cardboard”.

Expected result: The page shows a loading spinner or indicator that the filter is being applied. The page automatically reloads and shows accessories made of polyester and recycled cardboard. No accessories of other composition are shown.

# **TC-15 Verify checkout process with valid data (non-signed-in user)**
Ensure that the checkout process for non-signed-in user completes successfully with valid user details and payment information.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Critical | High | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User is not signed-in with items in their cart.

## **Post-conditions**
Order is successfully placed, and an order confirmation page is displayed.

## **Steps**

### **Step 1**
Action:	Navigate to the cart and click "Proceed to Checkout."

Expected result: User is taken to the checkout page with a summary of items.

### **Step 2**
Action: Enter valid personal information – first name, last name, email. Check mandatory checkboxes – Terms and Con ditions agreement and Data Privacy. Click “continue”.

Expected result: The personal information section closes \- an icon with a green tick appears next to it, indicating that the section has been completed correctly. The "addresses" section opens with first and last name fields filled automatically.

### **Step 3**
Enter valid address information – address, Zip/Postal Code, City and Country. The remaining fields are optional \- they may or may not be filled. Click “continue”.

Expected result: The address information section closes \- an icon with a green tick appears next to it, indicating that the section has been completed correctly. The "Shipping Method" section opens. Only “My Carrier” option is available. Radiobutt on next to it is automatically selected.

### **Step 4**
Action:	Click “Continue”.

Expected result: The “Shipping Method” section closes \- an icon with a green tick appears next to it, indicating that the section has been completed correctly. The "Payment" section opens with fillable fields for entering debit/credit card details.

### **Step 5**
Action: Provide information about card details \- number, security code and card expiration date. Accept Terms & Conditi ons and click “Place Order”.

Expected result: Order is successfully placed; confirmation page with order details appears.  

# **TC-16 Verify checkout fails with invalid credit card information (non- signed-in user)**
Confirm that the checkout process for non-signed-in user fails when invalid credit card information is entered.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Critical | High | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User is not signed-in with items in the cart; checkout page is accessible.

## **Post-conditions**
Order is not placed; error message indicates invalid payment details.

## **Steps**

### **Step 1**
Action	Navigate to the cart and click "Proceed to Checkout."

Expected result: User is taken to the checkout page with a summary of items.

### **Step 2**
Action: Enter valid personal information – first name, last name, email. Check mandatory checkboxes – Terms and Con ditions agreement and Data Privacy. Click “Continue”.

Expected result: The personal information section closes \- an icon with a green tick appears next to it, indicating that the section has been completed correctly. The "addresses" section opens with first and last name fields filled automatically.

### **Step 3**
Action: Enter valid address information – address, Zip/Postal Code, City and Country. The remaining fields are optional \- they may or may not be filled.

Expected result: The address information section closes \- an icon with a green tick appears next to it, indicating that the section has been completed correctly. The "Shipping Method" section opens. Only “My Carrier” option is available. Radiobutt on next to it is automatically selected.

### **Step 4**
Action:	Click “Continue”.

Expected result: The “Shipping Method” section closes \- an icon with a green tick appears next to it, indicating that the section has been completed correctly. The "Payment" section opens with fillable fields for entering debit/credit card details.

### **Step 5**
Action: Provide incorrect card details \- e.g. the card number should be in the wrong format \- instead of 12 characters, m ake it 9\. Accept Terms & Conditions and click “Place Order”.

Expected result: Order is not placed; error message indicates invalid payment details.  

# **TC-17 Verify search functionality with valid product name (signed-in user)**
Confirm that searching with a valid product name returns relevant results for signed-in user.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Major | High | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User is signed-in. Products are available in the system; search bar is accessible.

## **Post-conditions**
Search results page displays products matching the search term.

## **Steps**

### **Step 1**
Action:	Enter a specific product name (e.g., "T-shirt") into the search bar.

Expected result:	Product name is accepted and visible in the search bar.

### **Step 2**
Action:	Click “Enter”.

Expected result:	Relevant search results matching the product name are displayed.

# **TC-18 Verify adding a single product to the cart (signed-in user)**
Validate that a signed-in user can add a single item to the shopping cart.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Critical | High | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User is signed-in and has navigated to the random product page.

## **Post-conditions**
Product is added to the cart, and cart count updates accordingly.

## **Steps**

### **Step 1**
Action:	Search for the product and navigate to its product page.

Expected result:	Product page for the selected item is displayed.

### **Step 2**
Action:	Click the "Add to Cart" button.

Expected result:	Product is added to the cart; cart icon updates to reflect the added item.

# **TC-19 Verify adding products to the cart in different variants and quantities (signed-in user)**
Validate that a signed-in user can add different products to the cart after changing their details such as size, color, quantity.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Major | High | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User is signed-in and has navigated to the random product page.

## **Post-conditions**
Products are added to the cart in the appropriate variants that the user has selected.

## **Steps**

### **Step 1**
Action:	Search for the product and navigate to its product page.

Expected result:	Product page for the selected item is displayed.

### **Step 2**
Action:	Change product size, color and quantity (for example to 15).

Expected result:	Product details changed accordingly.

### **Step 3**
Action:	Click the "Add to Cart" button.

Expected result:	Product is added to the cart; cart icon updates to reflect the added item.

### **Step 4**
Action:	Search for another product and navigate to its product page.

Expected result:	Product page for the selected item is displayed.

### **Step 5**
Action:	Change product size, color and quantity (for example to 15).

Expected result:	Product details changed accordingly.

### **Step 6**
Action:	Click the "Add to Cart" button.

Expected result:	Product is added to the cart; cart icon updates to reflect the added item.

# **TC-20 Verify product quantity change from the cart level (signed-in user)**
Validate that a signed-in user can change product quantity in the “Shopping Cart” page.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Normal | High | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User is signed-in and has navigated to the “Shopping Cart” page. There is a clothing product in the cart, e.g. a T-shirt.

## **Post-conditions**
The product with the changed quantity is in the cart.

## **Steps**

### **Step 1**
Action:	Change the number of products in the cart, e.g. to 20.

Expected result:	Product number changed to 20, price recalculated according to the new quantity.

### **Step 2**
Action:	Change the number of products in the cart to 401.

Expected result:	An error message appears “The available purchase order quantity for this product is 400\.

# **TC-21 Verify product size change from the cart level (signed-in user)**
Validate that a signed-in user can change product size in the “Shopping Cart” page.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Normal | High | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User is signed-in and has navigated to the “Shopping Cart” page. There is a clothing product in the cart, e.g. a T-shirt.

## **Post-conditions**
The product with the changed size is in the cart

## **Steps**

### **Step 1**
Action:	Change the product size, using drop-down list for the product.

Expected result:	Product size has changed.

# **TC-22 Verify adding a product to wishlist (signed-in user)**
Ensure that a signed-in user can successfully add a product to their wishlist.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Major | High | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User is signed-in and on the product page of an item they want to add to the wishlist.

## **Post-conditions**
The product is added to the user's wishlist, which is accessible from their account.

## **Steps**

### **Step 1**
Action:	Navigate to a product page (e.g., "T-shirt").

Expected result: Product page is displayed with all product information and options, including the "Add to Wishlist" heart-sha ped button.

### **Step 2**

Action:	Click the "Add to Wishlist" button.

Expected result: A window appears in which the user can select the list in which he wants to save the product.

### **Step 3**
Action:	Click on “My wishlist”.

Expected result: The list selection window closes. A green toast message "Product Added" appears on the screen.

### **Step 4**
Action:	Go to the "Wishlist" section under the user account.

Expected result: The product appears in the wishlist with an option to view, add to cart, edit or remove it.

# **TC-23 Verify removing a product from wishlist (signed-in user)**
Verify that a signed-in user can remove product from wishlist.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Normal | High | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User is signed-in; they are on the wishlist page with the product added to this list.

## **Post-conditions**
Product is removed from the wishlist.

## **Steps**

### **Step 1**
Action:	Click on the button in the shape of trash can in the product preview image.

Expected result: A window appears to confirm the execution of the action "The product will be removed from My wishlist".

### **Step 2**
Action:	Click “Remove”.

Expected result: A green toast message "Product successfully removed" appears on the screen.

# **TC-24 Verify filter by single criteria (signed-in user)**
Verify that applying single filter displays only products that belong to the selected criteria for signed-in user.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Normal | High | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions** 
User is signed-in. Multiple products are available across different categories, and the user is on the product search or category page.

## **Post-conditions**
The page should display only products in the selected criteria or reset to the default product view if filters are cleared.

## **Steps**

### **Step 1**
Action:	Select “Clothes” category and then apply a specific filter (e.g., "Men").

Expected result: The filter is selected, and the page shows a loading spinner or indicator that the filter is being applied. The page automatically reloads and shows clothes only from the “Men” category. No products from other categories are sho wn.

# **TC-25 Verify filter by multiple criteria (signed-in user)**
Validate that applying multiple filters together narrows down the product search results to meet all selected criteria for signed-in user.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Normal | High | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions** 
User is signed-in. Products are available across different categories and price ranges.

## **Post-conditions**
The page should display only products that match the applied criteria or reset to the default product view if filters are cleared.

## **Steps**

### **Step 1**
Action:	Select “Accessories” category and then apply a specific filter (e.g., Composition “Polyester”).

Expected result: The filter is selected, and the page shows a loading spinner or indicator that the filter is being applied. The page automatically reloads and shows Polyester accessories.  No accessories of other composition are shown.

### **Step 2**
Action:	Apply an additional filer e.g., Composition “Recycled cardboard”.

Expected result: The page shows a loading spinner or indicator that the filter is being applied. The page automatically reloads and shows accessories made of polyester and recycled cardboard. No accessories of other composition are shown.

# **TC-26 Verify checkout process with valid data (signed-in user)**
Ensure that the checkout process for signed-in user completes successfully with valid user details and payment information.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Critical | High | Not set | Functional |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
User is signed-in with items in their cart.

## **Post-conditions**
Order is successfully placed, and an order confirmation page is displayed.

## **Steps**

### **Step 1**
Action:	Navigate to the cart and click "Proceed to Checkout."

Expected result: User is taken to the checkout page with a summary of items. Personal information is automatically completed. The "addresses" section opens with first, last name and country fields filled automatically.

### **Step 2**
Action: Enter valid address information – Address, Zip/Postal Code and City. The remaining fields are optional \- they ma y or may not be filled. Click “Continue”.

Expected result: The address information section closes \- an icon with a green tick appears next to it, indicating that the section has been completed correctly. The "Shipping Method" section opens. Two options are available – “Click and Collect” (Pick-up in store) and “My Carrier”.

### **Step 3**
Action:	Select option “Click and Collect” then click “Continue”.

Expected result: The “Shipping Method” section closes \- an icon with a green tick appears next to it, indicating that the section has been completed correctly. The "Payment" section opens with three available payment methods: “Pay by bank wire”, “Pay by cash and delivery” and “Pay by check”. There is no option for adding debit/credit card details for sign ed-in users.

### **Step 4**
Action:	Choose any option, e.g. “Pay by cash and delivery”. Accept Terms & Conditions and click “Place Order”.

Expected result: Order is successfully placed; confirmation page with order details appears.  

# **TC-27 Homepage Navigation (Chrome)**
Ensuring that the homepage is functional, user-friendly, and that all navigation elements (links, menus, banners, etc.) are accessible and lead to the correct destinations in the newest version of Google Chrome. It will also assess the responsiveness and accessibility of the homepage across different screen sizes.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Major | High | Not set | Usability |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
1. The demo Prestashop site is live and accessible from the browser.
2. The user has appropriate permissions to view and interact with the website. The browser is up-to-date.

## **Post-conditions**
1. The homepage should be fully accessible with no broken links or navigation issues.
2. All pages that are linked from the homepage should function correctly and load with the expected content.

## **Steps**

### **Step 1**
Action:	Navigate to the homepage of the site in the browser.

Expected result: The homepage loads fully, with no errors or broken images. It should display the main menu, featured products, banners, footer, and the search bar.

### **Step 2**
Action:	Click on each category link in the main menu ("Clothes", "Accessories", "Art").

Expected result: Each category should load the correct page with the expected product list or category content. There should be no errors or 404 pages. All links should be functional and redirect to the appropriate pages.

### **Step 3**
Action:	Scroll down to the footer and click on links such as "Contact Us" and "Terms and conditions of use".

Expected result: Footer links should lead to the correct pages without any broken links. The pages should load promptly and display the appropriate content.

### **Step 4**
Action:	Click on one or more featured products displayed on the homepage.

Expected result: The product detail page should load correctly, showing the relevant product information (e.g., price, description, product details, images, and "Add to Cart" & "Add to Wishlist buttons). There should be no broken images or missin g content.

### **Step 5**
Action:	Click on any promotional banners or sliders located on the homepage.

Expected result: The linked page should load and display content relevant to the promotion (e.g., discounts, sales pages). The banner should redirect to the correct page without errors.

### **Step 6**
Action:	Enter a product name or keyword into the search bar and press "Enter."

Expected result: The search results should display relevant products or categories based on the search term. If no results are found, a friendly "no results" message should be shown. The results should load without significant delays.

### **Step 7**
Action:	Test the homepage on multiple screen sizes (e.g., desktop, tablet, and mobile). This can be done using function in the homepage header or developer tools.

Expected result: The homepage should be responsive, with all elements adjusting to fit the screen size. The navigation, images, and text should be clear, and clickable elements should be appropriately sized for mobile use. No layout or functiona lity issues should occur.

# **TC-28 Homepage Navigation (Microsoft Edge)**
Ensuring that the homepage is functional, user-friendly, and that all navigation elements (links, menus, banners, etc.) are accessible and lead to the correct destinations in the newest version of Microsoft Edge. It will also assess the responsiveness and accessibility of the homepage across different screen sizes.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Major | High | Not set | Usability |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
1. The demo Prestashop site is live and accessible from the browser.
2. The user has appropriate permissions to view and interact with the website. The browser is up-to-date.

## **Post-conditions**
1. The homepage should be fully accessible with no broken links or navigation issues.
2. All pages that are linked from the homepage should function correctly and load with the expected content.

## **Steps**

### **Step 1**
Action:	Navigate to the homepage of the site in the browser.

Expected result: The homepage loads fully, with no errors or broken images. It should display the main menu, featured products, banners, footer, and the search bar.

### **Step 2**
Action:	Click on each category link in the main menu ("Clothes", "Accessories", "Art").

Expected result: Each category should load the correct page with the expected product list or category content. There should be no errors or 404 pages. All links should be functional and redirect to the appropriate pages.

### **Step 3**
Action:	Scroll down to the footer and click on links such as "Contact Us" and "Terms and conditions of use".

Expected result: Footer links should lead to the correct pages without any broken links. The pages should load promptly and display the appropriate content.

### **Step 4**
Action:	Click on one or more featured products displayed on the homepage.

Expected result: The product detail page should load correctly, showing the relevant product information (e.g., price, description, product details, images, and "Add to Cart" & "Add to Wishlist buttons). There should be no broken images or missin g content.

### **Step 5**
Action:	Click on any promotional banners or sliders located on the homepage.

Expected result: The linked page should load and display content relevant to the promotion (e.g., discounts, sales pages). The banner should redirect to the correct page without errors.

### **Step 6**
Action:	Enter a product name or keyword into the search bar and press "Enter."

Expected result: The search results should display relevant products or categories based on the search term. If no results are found, a friendly "no results" message should be shown. The results should load without significant delays.

### **Step 7**
Action:	Test the homepage on multiple screen sizes (e.g., desktop, tablet, and mobile). This can be done using function in the homepage header or developer tools.

Expected result: The homepage should be responsive, with all elements adjusting to fit the screen size. The navigation, images, and text should be clear, and clickable elements should be appropriately sized for mobile use. No layout or functiona lity issues should occur.

# **TC-29 Page Load Time**
Ensure that the page load time meets the expected performance standards.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Normal | High | Not set | Performance |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
1. Newest version of Google Chrome is installed, network connection is stable. The demo Prestashop site is live and accessible from the browser.  
2. The user has appropriate permissions to view and interact with the website.

## **Post-conditions**
The page load time has been documented.

## **Steps**

### **Step 1**
Action:	Open Prestashop homepage.

Expected result: The browser opens the homepage successfully without errors.

### **Step 2**
Action:	Open Developer Tools.

Expected result: Developer Tools window opens with tabs like Network, Performance, Console, etc.

### **Step 3**
Action:	Go to the **Network** tab and reload the page.

Expected result: The page reloads, and network requests are captured in the Network tab.

### **Step 4**
Action: Monitor the **Load Time** (total time for the page to load). Look at the **Total Duration** at the bottom of the Network tab.

Expected result: The total page load time should be less than **3 seconds**.

# **TC-30 Time to Interactive (TTI)**
Measure how quickly the page becomes interactive and usable by the user after loading.

| Severity | Priority | Behavior | Type |
| :---- | ----- | :---- | :---- |
| Major | Medium | Not set | Performance |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
1. Newest version of Google Chrome is installed, network connection is stable. The demo Prestashop site is live and accessible from the browser.  
2. The user has appropriate permissions to view and interact with the website.

## **Post-conditions**
TTI measurement has been recorded.

## **Steps**

### **Step 1**
Action:	Open Prestashop homepage in Google Chrome.

Expected result:	The homepage is loaded in the browser.

### **Step 2**
Action:	Open Developer Tools.

Expected result:	Developer Tools window opens with the Performance tab.

### **Step 3**
Action:	Go to the **Performance** tab.

Expected result:	The Performance tab is selected, and recording options are visible.

### **Step 4**
Action:	Click **Record** and reload the page.

Expected result:	Recording starts, and the page is reloaded for performance tracking.

### **Step 5**
Action:	Wait for the page to load completely, then stop the recording.

Expected result: The recording stops once the page is fully loaded.

### **Step 6**
Action:	Look for **Time to Interactive (TTI)** in the summary.

Expected result:	TTI is under **5 seconds.**

# **TC-31 JavaScript Execution Performance**
Test the performance impact of JavaScript execution on page loading and responsiveness.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Major | High | Not set | Performance |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions** 
1. Newest version of Google Chrome is installed, network connection is stable. 
2. The demo Prestashop site is live and accessible from the browser.  
3. The user has appropriate permissions to view and interact with the website.
4. Developer Tools are accessible.

## **Post-conditions**
JavaScript execution time has been reviewed.

## **Steps**

### **Step 1**
Action:	Open Prestashop homepage in Google Chrome.

Expected result: The homepage loads successfully.

### **Step 2**
Action:	Open Developer Tools.

Expected result: Developer Tools window opens with various tabs.

### **Step 3**
Action:	Go to the **Performance** tab.

Expected result: The Performance tab is selected and ready to record.

### **Step 4**
Action:	Record a page load while monitoring JavaScript execution time.

Expected result: Recording starts, capturing JavaScript execution metrics.

### **Step 5**
Action:	Once the recording is complete, review the **JavaScript execution time** (listed under “Scripting”).

Expected result:  JavaScript execution should take less than **1 second**.

# **C-32 CSS Rendering Performance**
Measure how quickly the site renders CSS styles after the initial HTML load.

| Severity | Priority | Behavior | Type |
| :---- | ----- | :---- | :---- |
| Normal | Medium | Not set | Performance |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
1. Newest version of Google Chrome is installed, network connection is stable. 
2. The demo Prestashop site is live and accessible from the browser.  
3. The user has appropriate permissions to view and interact with the website. 
4. Developer Tools are accessible.

## **Post-conditions**
CSS rendering performance data documented.

## **Steps**

### **Step 1**
Action:	Open Prestashop homepage in Google Chrome.

Expected result:	Homepage opens in the browser.

### **Step 2**
Action:	Open Developer Tools.

Expected result:	Developer Tools open with multiple tabs.

### **Step 3**
Action: Go to the **Performance** tab.

Expected result:	The Performance tab is selected for performance monitoring.

### **Step 4**
Action: Record the page load while monitoring CSS rendering time.

Expected result:	Recording starts, capturing rendering details.

### **Step 5**
Action:	Review the **CSS Rendering Time** in the timeline of the performance recording.

Expected result:	CSS rendering time should be under **2 seconds** after HTML load.

# **C-33 Browser Resource Consumption**
Test how efficiently the website uses browser resources (e.g., CPU, memory) during typical browsing.

| Severity | Priority | Behavior | Type |
| :---- | ----- | :---- | :---- |
| Normal | Medium | Not set | Performance |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
1. Newest version of Google Chrome is installed, network connection is stable. 
2. The demo Prestashop site is live and accessible from the browser.  
3. The user has appropriate permissions to view and interact with the website. 
4. Developer Tools are accessible.

## **Post-conditions**
Browser resource usage data has been reviewed.

## **Steps**

### **Step 1**
Action:	Open Prestashop homepage in Google Chrome.

Expected result: The homepage is loaded without errors.

### **Step 2**
Action:	Open Developer Tools and go to Performance tab.

Expected result: The Performance tab opens, ready for recording.

### **Step 3**
Action:	Record the page load and navigate around the site (e.g., add items to the cart, browse categories).

Expected result: Page load and navigation events are captured for resource monitoring.

### **Step 4**
Action:	Observe the **CPU and memory usage** during navigation and interactions.

Expected result: CPU and memory usage should remain**under 50%** CPU utilization.

# **C-34 SQL Injection**
Ensure the application is not vulnerable to SQL injection attacks.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Critical | High | Not set | Security |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
1. Newest version of Google Chrome is installed, network connection is stable. 
2. The demo Prestashop is open in browser.
3. The user has appropriate permissions to view and interact with the website.

## **Post-conditions**
Any SQL injection vulnerabilities are documented.

## **Steps**

### **Step 1**
Action:	Identify a form or input field (e.g., login form, search bar, contact form).

Expected result: Input field is accessible and functional.

### **Step 2**
Action:	Enter a malicious SQL query into the field (e.g.,'; DROP TABLE users; \--).

Expected result: The application should display an error or handle the input gracefully without breaking or exposing data.

### **Step 3**
Action:	Monitor the application’s behavior (e.g., error messages or unexpected results).

Expected result: No sensitive data is exposed (e.g., "SQL syntax error") or unauthorized actions performed.

# **C-35 Cross-Site Scripting (XSS)**
Ensure the application is protected against XSS attacks.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Critical | High | Not set | Security |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
1. Newest version of Google Chrome is installed, network connection is stable. 
2. The demo Prestashop is open in browser.
3. The user has appropriate permissions to view and interact with the website.

## **Post-conditions**
Application handles potentially malicious input securely.

## **Steps**

### **Step 1**
Action:	Identify any input fields or content sections (e.g., order tracking).

Expected result: Input fields are functional.

### **Step 2**
Action:	Input a script tag (e.g., \<script\>alert('XSS');\</script\>).

Expected result: The input should be sanitized or rejected.

### **Step 3**
Action: Submit the input and observe the behavior of the page.

Expected result: The script should not execute, and no unauthorized actions (e.g., pop-ups or alerts) should occur.

# **C-36 User Authentication Security**
Verify that user authentication is secure and prevents unauthorized access.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Critical | High | Not set | Security |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
1. Newest version of Google Chrome is installed, network connection is stable. 
2. The demo Prestashop is open in browser.  
3. The user has appropriate permissions to view and interact with the website. 
4. User account exists.

## **Post-conditions**
Authentication mechanisms function securely.

## **Steps**

### **Step 1**
Action:	Log in to Prestashop with valid credentials.

Expected result:	Login is successful and redirects to the appropriate user dashboard.

### **Step 2**
Action:	Attempt to log in with incorrect credentials multiple times.

Expected result:	Account should lock or display a CAPTCHA after 5 failed attempts.

### **Step 3**
Action:	Observe error messages for failed logins.

Expected result:	Generic error message "Authentication failed." is displayed without revealing specific details.

# **C-37 Session Management**

Test the security of session handling.

| Severity | Priority | Behavior | Type |
| :---- | ----- | :---- | :---- |
| Normal | Medium | Not set | Security |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions** 
1. Newest version of Google Chrome is installed, network connection is stable. 
2. The demo Prestashop is open in browser.
3. The user has appropriate permissions to view and interact with the website. 
4. User account exists.

## **Post-conditions**
Session-related vulnerabilities are identified.

## **Steps**

### **Step 1**
Action:	Log in to the application and perform standard actions.

Expected result: Actions are executed without session issues.

### **Step 2**
Action:	Log out and attempt to use the browser’s back button to access a restricted page.

Expected result: Access is denied or redirected to the login page.

### **Step 3**
Action:	Inspect cookies using browser tools (e.g., Chrome DevTools) and note their attributes (e.g.,Secure, HttpOnly)

Expected result: Cookies are flagged as Secure and HttpOnly, and sensitive data is not exposed.

# **C-38 Sensitive Data Exposure**
Ensure sensitive information is not exposed in the frontend or network traffic.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Critical | High | Not set | Security |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions**
1. Newest version of Google Chrome is installed, network connection is stable. 
2. The demo Prestashop is open in browser.
3. The user has appropriate permissions to view and interact with the website.

## **Post-conditions**
Potential data exposure risks are documented.

## **Steps**

### **Step 1**
Action: Log in and navigate through the application, performing standard actions (e.g., checkout, viewing user d etails).

Expected result: Application behaves as expected without exposing sensitive information.

### **Step 2**
Action:	Use DevTools to inspect network requests during actions.

Expected result: Sensitive data (e.g., passwords, payment details) is not visible in plaintext.

### **Step 3**
Action:	Inspect page source and console logs for any sensitive data.

Expected result: No sensitive data is exposed in HTML or JavaScript logs.

# **C-39 Password Security**
Verify the robustness of password policies.

| Severity | Priority | Behavior | Type |
| :---- | :---- | :---- | :---- |
| Major | High | Not set | Security |
| **Layer** | **Is Flaky** | **Milestone** | **Automation** |
| Not set | No | \- | Manual |
| **Status** | **Is Muted** |  |  |
| Actual | No |  |  |

## **Pre-conditions** 
1. Newest version of Google Chrome is installed, network connection is stable. 
2. The demo Prestashop is open in browser.
3. The user has appropriate permissions to view and interact with the website.

## **Post-conditions**
Password policies and mechanisms are validated.

## **Steps**

### **Step 1**
Action:	Attempt to register a new account using a weak password (e.g., "12345").

Expected result:  Registration is denied with a message requiring stronger passwords.

### **Step 2**
Action:	Attempt to reset a password using the "Forgot Password" feature.

Expected resultL  A password reset link is sent to the registered email; the password is never exposed.

### **Step 3**
Action:	Inspect password change requests using browser tools to ensure data is transmitted securely.

Expected result:  Passwords are never transmitted in plaintext over the network.
