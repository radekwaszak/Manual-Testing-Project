

| ID number | D-1 |
| :---- | :---- |
| Name | Incorrect error message for maximum purchase order quantity (non-signed-in user) |
| Reporter | Radosław W. |
| Submit Date | 09/11/2024 |
| Summary | When attempting to change the product quantity in the cart to 401, an error message appears. The message content is correct, but it does not follow the required phrasing as specified in the requirements. |
| Environment | Browser: Chrome 131.0.6778.70  (64-bit) Platform: Windows 10 PrestaShop Version: Demo version ([https://demo.prestashop.com/\#/en/front](https://demo.prestashop.com/#/en/front))  |
| Severity | **Normal** |
| Assigned to | / |
| Priority | **Medium** |

**Steps to Reproduce:**

1. As a non-signed-in user, go to the product page and add a product to the cart.  
2. Navigate to the cart and update the product quantity to 401\.  
3. Observe the error message that appears below the product or at the top of the cart.

**Expected Result:** The error message should say: "The available purchase order quantity for this product is 400."

**Actual Result:** The error message displayed is: "The available purchase order quantity for this product is 300." This message is shown in the wrong phrasing as per requirements.  

**DevTools Information:**

* **Console Output:** No JavaScript errors were observed related to this message.  
* **Network Response**: No server-side API errors returned.  
* **DOM Structure:**
  
```
<article class="alert alert-danger" role="alert" data-alert="danger">
    <ul>
        <li>The available purchase order quantity for this product is 300.</li>
    </ul>
</article>
```

**Suggested Fix:** Update the error message to be compliant with the requirements.

**Attachments:**

![image1](https://d2cxucsjd6xvsd.cloudfront.net/public/team/014f16759dade12d4b9249822f2a05736e0ee69b/attachment/04fc0ba1df8e5ceed998bbb37b14c436b5b96bcf/screen2.JPG)
