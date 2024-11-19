

| ID number | D-4 |
| :---- | :---- |
| Name | Unable to complete checkout as non-signed-in user: missing payment fields |
| Reporter | Radosław W. |
| Submit Date | 09/11/2024 |
| Summary | During the checkout process for a non-signed-in user, after entering personal information, address, and selecting the shipping method, the payment section fails to display fields for card details (card number, security code, expiration date). The “Place Order” button remains grayed out even after accepting the Terms and Conditions, preventing order completion. |
| Environment | Chrome 131.0.6778.70 (64-bit), OS: Windows 10, Device: Desktop, Network: High-speed broadband connection, PrestaShop Version: Demo ([https://demo.prestashop.com/\#/en/front](https://demo.prestashop.com/#/en/front))  |
| Severity | **Blocker** |
| Assigned to | / |
| Priority | **Major** |

**Steps to Reproduce:**

1. Navigate to the cart and click "Proceed to Checkout."  
2. Enter valid personal information (first name, last name, email). Check mandatory checkboxes (Terms and Conditions, Data Privacy). Click “Continue.”  
3. Enter valid address information (address, Zip/Postal Code, City, Country). Optional fields may remain blank. Click “Continue.”  
4. Click “Continue” on the Shipping Method section.

**Expected Result:** The “Shipping Method” section closes with a green checkmark, indicating completion. The "Payment" section opens with fields for card details (card number, security code, expiration date).

**Actual Result:** 

In the Payment section:

* No fields for entering card details (card number, security code, expiration date) are available.  
* Only a checkbox to accept the Terms and Conditions appears.  
* The “Place Order” button remains grayed out and disabled, even after checking the Terms and Conditions checkbox, making it impossible to place the order.

**DevTools Information:**

* HTML Snippet of Disabled Button:

```
<button type="submit" class="btn btn-primary center-block disabled" disabled="disabled">
    Place order
</button>
```

**Suggested Fix:**

* Ensure that the payment fields (card number, security code, expiration date) are correctly displayed for all users at the payment step.  
* Verify that the “Place Order” button is enabled after the Terms and Conditions checkbox is selected, assuming all required fields are filled.

**Attachments:**

[**See video showing defect**](https://jam.dev/c/1ea3c5ab-22a8-46af-ad51-c44bd40408b1)

![image1](https://d2cxucsjd6xvsd.cloudfront.net/public/team/014f16759dade12d4b9249822f2a05736e0ee69b/attachment/a111249a338e9a0d1e0f9dbf24ea8fa51377b01b/1.0.JPG)
![image2](https://d2cxucsjd6xvsd.cloudfront.net/public/team/014f16759dade12d4b9249822f2a05736e0ee69b/attachment/6d83c636caf3c16c52b1a8430072da658043c701/2.0.JPG)
![image3](https://d2cxucsjd6xvsd.cloudfront.net/public/team/014f16759dade12d4b9249822f2a05736e0ee69b/attachment/402952d234611d1d69abc7ad583f0d1dcd97361f/placeorder1.JPG)
![image4](https://d2cxucsjd6xvsd.cloudfront.net/public/team/014f16759dade12d4b9249822f2a05736e0ee69b/attachment/1e3e0095a395eecd51302108079f00a2ee31b52c/placeorder2.JPG)
