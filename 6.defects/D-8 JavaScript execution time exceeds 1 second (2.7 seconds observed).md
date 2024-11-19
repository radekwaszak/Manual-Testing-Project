

| ID number | D-8 |
| :---- | :---- |
| Name | JavaScript execution time exceeds 1 second (2.7 seconds observed) |
| Reporter | Radosław W. |
| Submit Date | 17/11/2024 |
| Summary | The JavaScript execution time on the Prestashop demo homepage is 2.7 seconds, exceeding the acceptable threshold of 1 second. This prolonged execution time negatively impacts page load performance and user experience, particularly during initial interactions. |
| Environment | Browser: Chrome 131.0.6778.70 (64-bit) Platform: Windows 10 Device: Desktop Network: High-speed broadband connection PrestaShop Version: Demo version ([https://demo.prestashop.com/\#/en/front](https://demo.prestashop.com/#/en/front))  |
| Severity | **Normal** |
| Assigned to | / |
| Priority | **Medium** |

**Steps to Reproduce:**

1. Navigate to homepage ([https://demo.prestashop.com/\#/en/front](https://demo.prestashop.com/#/en/front)).   
2. Open DevTools and Navigate to the Performance tab, click Record, and reload the page.  
3. Stop recording after the page fully loads.  
4. Look for the JavaScript execution time in the "Main Thread" section of the timeline.  
5. Observe the execution time of JavaScript processes.  
   

**Expected Result:** JavaScript execution time should be less than or equal to 1 second to ensure optimal page performance.

**Actual Result:** JavaScript execution time is 2.7 seconds, exceeding the acceptable threshold by 1.7 seconds.

**Suggested Fix:** 

* Optimize JavaScript code; minify and bundle JavaScript files to reduce their size or remove or defer non-essential scripts during page load.  
* Implement code splitting; break large JavaScript files into smaller chunks and load them as needed.  
* Use asynchronous or deferred loading; ensure JavaScript files that are not critical to the page's initial rendering are loaded asynchronously or deferred.  
* Review third-party libraries; audit external scripts and remove or replace any inefficient or unnecessary libraries.  
* Enable caching; cache JavaScript resources to minimize repeated loading.

**Attachments:**