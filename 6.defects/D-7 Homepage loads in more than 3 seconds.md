

| ID number | D-7 |
| :---- | :---- |
| Name | Homepage loads in more than 3 seconds |
| Reporter | Radosław W. |
| Submit Date | 17/11/2024 |
| Summary | The homepage takes 14.5 seconds to fully load, significantly exceeding the expected load time of 3 seconds. |
| Environment | Browser: Chrome 131.0.6778.70 (64-bit) Platform: Windows 10 Device: Desktop Network: High-speed broadband connection PrestaShop Version: Demo version ([https://demo.prestashop.com/\#/en/front](https://demo.prestashop.com/#/en/front))  |
| Severity | **Major** |
| Assigned to | / |
| Priority | **High** |

**Steps to Reproduce:**

1. Navigate to homepage ([https://demo.prestashop.com/\#/en/front](https://demo.prestashop.com/#/en/front)).   
2. Open DevTools.  
3. Go to the Performance tab, click Record, and reload the page.  
4. Stop the recording once the page has fully loaded.  
5. Observe the timeline and note the Total Load Time.

**Expected Result:** The homepage should fully load within 3 seconds or less, providing a seamless user experience.

**Actual Result:** The homepage takes approximately 14.5 seconds to load, which is 11.5 seconds longer than the expected time.

**Suggested Fix:** 

* Optimize server response times; review server-side performance and database queries.  
* Reduce asset load; compress large images, minify CSS and JavaScript files, and enable lazy loading for non-critical assets.  
* Optimize third-party scripts: identify and minimize external resources causing delays (e.g., fonts, analytics, or ads).  
* Implement caching: use browser caching and CDN caching to improve resource delivery speeds.

**Attachments:**