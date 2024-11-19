

| ID number | D-3 |
| :---- | :---- |
| Name | Non-signed-in user cannot add products to a temporary wishlist |
| Reporter | Radosław W. |
| Submit Date | 09/11/2024 |
| Summary | When a non-signed-in user attempts to add a product to the wishlist, a modal appears, prompting the user to sign in. However, according to the requirements, non-logged-in users should be able to add products to a temporary wishlist without needing to sign in. |
| Environment | Browser: Chrome 131.0.6778.70 (64-bit), OS: Windows 10, Device: Desktop, Network: High-speed broadband connection, PrestaShop Version: Demo ([https://demo.prestashop.com/\#/en/front](https://demo.prestashop.com/#/en/front))  |
| Severity | **Normal** |
| Assigned to | / |
| Priority | **Medium** |

**Steps to Reproduce:**

1. Navigate to a product page while signed-out.  
2. Attempt to add the product to the wishlist.  
3. Observe the modal that appears, instructing the user to sign-in to save items to the wishlist.

**Expected Result:** 

* Non-signed-in users should be able to add products to a temporary wishlist without requiring a login.  
* No login prompt should appear. Instead, the product should be successfully added to a temporary wishlist, which should persist for 24 hours.


**Actual Result:** 

* A modal dialog appears with the following message: "You need to be logged in to save products in your wishlist."  
* The user is unable to add products to the wishlist without logging in, which is inconsistent with the requirement for a temporary wishlist for non-signed-in users.

**DevTools Information:**

* DOM Structure of the Modal:

```
<div role="document" class="modal-dialog modal-dialog-centered">
    <div class="modal-content">
        <div class="modal-header">
            <h5 class="modal-title">Sign in</h5>
            <button type="button" data-dismiss="modal" aria-label="Close" class="close">
                <span aria-hidden="true">×</span>
            </button>
        </div>
        <div class="modal-body">
            <p class="modal-text">You need to be logged in to save products in your wishlist.</p>
        </div>
        <div class="modal-footer">
            <button type="button" data-dismiss="modal" class="modal-cancel btn btn-secondary">
                Cancel
            </button>
            <a type="button" href="https://rough-yard.demo.prestashop.com/en/login" class="btn btn-primary">
                Sign in
            </a>
        </div>
    </div>
</div>
```

**Suggested Fix:** Update the wishlist logic so that non-logged-in users can add items to a temporary session-based wishlist.

**Attachments:**  
![image1](https://d2cxucsjd6xvsd.cloudfront.net/public/team/014f16759dade12d4b9249822f2a05736e0ee69b/attachment/54150b751e221c1175c4cb27b098c25a47961fd5/Przechwytywanie.JPG)
