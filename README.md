### Name: Parwiz Khan

### Check your understanding questions

### 1) Where would you fit your automated tests in your Recipe project development pipeline?
**Answer:**  
**Within a GitHub action that runs whenever code is pushed.**
**Explanation:**  
Automated tests should be triggered on every push to the repository. This helps catch bugs early and ensures that bad code doesn’t get merged into the main branch. Manually running tests is error-prone and easy to skip, and waiting until the end of development defeats the purpose of testing. Continuous Integration (CI) setups like GitHub Actions enforce testing automatically, making the workflow more reliable and scalable for teams.



### 2) Would you use an end-to-end test to check if a function is returning the correct output?
**Answer:**  
**No.**
**Explanation:**  
E2E tests check full user flows, not single functions. To test a function’s output, use a unit test instead.


### 3) What is the difference between navigation and snapshot mode?

**Navigation mode** reloads the page from scratch and measures load-time metrics (FCP, LCP, TBT, etc.) as if it’s a first visit.  
**Snapshot mode** runs audits on the page in its current state (no reload), focusing on accessibility, best practices and SEO.

### 4) Name three things we could do to improve the CSE 110 shop site based on the Lighthouse results.
**1 Viewport**  
   ```html
   <meta name="viewport" content="width=device-width, initial-scale=1">
   ```
**2 Images**
 resize to display size, convert to WebP/AVIF, and add loading="lazy".

 **3 JS**
 remove unused code, minify bundles, and Code split for faster startup