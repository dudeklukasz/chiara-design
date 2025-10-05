<h1 id="Test-report">Test Summary Report.</h1>

1. **Descripton**: Tests were conducted to ensure the quality and reliability of the web application functionalitys.
2. **Test Period**: Beginning of Sprint 7 - End of Sprint 7
3. **Test Coverage** : 95% test coverage, remaining 5% contained edge cases with low risk
4. **Test Execution Summary:** 
* Total Test Cases: 110
* Passed: 94
* Failed: 16
* Blocked: 0
* Not Executed: 6
* Total bugs found: 20


5. **Key Findings**:

 + **Core Functionality Issues:**
   + Incorrect error messages and unexpected behavior in search results.
   + Issues with product filtering and sorting functionality.
   + Problems with adding and removing items from the cart.
   + Incorrect calculations and display of order totals.
  
+ **User Interface and Experience Issues:**
   + Inconsistent layout and design elements.
   + Misaligned or missing UI elements.
   +  Slow page loading times and unresponsive behavior.
   + Inefficient navigation and user flow.
   + 6 performance tests were not executed due to a lack of a performance tester.

6. **Recommendations**:

* **Prioritize Bug Fixes:** Address the identified functional and usability issues.
* **Consider Additional Testing:** Conduct further exploratory testing to uncover additional issues.
* **Enhance Performance Testing:** Allocate resources to perform comprehensive performance testing to identify and resolve performance bottlenecks.

<br></br>

<h1 id="Qase-Main">Bug reports</h1>

<h2 id="Bug-Reports">1. Favorite button redirects to 404 error page.</h2>

**Description**: When a user clicks on the "Favorite" button on any page, they are unexpectedly redirected to a 404 error page instead of being directed to a list of their favorite items.

**Expected result**: Be redirected to a "Favorites" page or section where all favorited items are listed. 

**Actual result**: The user is redirected to a 404 error page.

<p align="center">
  <img src="https://github.com/dudekluk/Portfolio/blob/main/img/BR15.png" alt="Image" width="70%" height="70%">
</p>


<h2 id="Bug-Reports">2. Missing account icon on certain pages.</h2>

**Description**: The account icon, typically located in the top right corner of the page, is missing on specific pages within the application. This prevents users from accessing their account settings.

**Expected result**: The account icon should be visible on all pages, allowing users to access their account information and settings.

**Actual result**:  The account icon is absent from certain pages, limiting user functionality and creating a suboptimal user experience.

<p align="center">
  <img src="https://github.com/dudekluk/Portfolio/blob/main/img/BR1.png" alt="Image" width="70%" height="70%">
</p>


<h2 id="Bug-Reports">3. Quick cart view UI layout issues.</h2>

**Description**: The quick cart view is not displaying correctly, with elements extending beyond the screen boundaries. Additionally, some buttons within the quick cart are misaligned, leading to an inconsistent user experience.

**Expected result**: The quick cart view should be contained within the screen boundaries, and all elements should be properly aligned. Buttons should be consistently positioned and easy to interact with.

**Actual result**: Elements in the quick cart view are overflowing the screen, and buttons are not aligned correctly. This makes it difficult for users to interact with the cart and complete their purchases. 

<p align="center">
  <img src="https://github.com/dudekluk/Portfolio/blob/main/img/BR4.png" alt="Image" width="70%" height="70%">
</p>

<h2 id="Bug-Reports">4. Incorrect free shipping calculation.</h2>

**Description**: The system is not accurately calculating the free shipping threshold. Users are able to receive free shipping for orders below the 500zł threshold or are not receiving free shipping for orders exceeding 1000zł. Additionally, the missing amount for free shipping is sometimes displayed as a negative value.

**Expected result**: The system should correctly calculate the total order amount and apply free shipping when the threshold of 500zł is met. The missing amount for free shipping should be displayed as a positive value.

**Actual result**: The system is either applying free shipping for orders below the threshold or failing to apply it for orders exceeding the threshold. In some cases, the missing amount for free shipping is displayed as a negative value.

<p align="center">
  <img src="https://github.com/dudekluk/Portfolio/blob/main/img/BR6.png" alt="Image" width="70%" height="70%">
</p>


<h2 id="Bug-Reports">5. Excessive quantity addition in quick cart.</h2>

**Description**: Users are able to add an excessive quantity of items to the quick cart, exceeding the available stock.

**Expected result**: The system should limit the quantity of items added to the cart to the available stock. 

**Actual result**: Users can input values exceeding the available stock in the quick cart.

<p align="center">
  <img src="https://github.com/dudekluk/Portfolio/blob/main/img/BR13.png" alt="Image" width="70%" height="70%">
</p>


<h2 id="Bug-Reports">6. Incorrect order processing for out of stock items.</h2>

**Description**: When placing an order for items that exceed the available stock, the system displays a message indicating that the quantity will be automatically reduced. However, the order does not reflect this reduction, leading to potential order fulfillment issues.

**Expected result**: If an item's quantity exceeds available stock, the system should:
1. Reduce the order quantity to the available stock.
2. Display a clear notification to the user about the quantity adjustment.
3. Update the order summary to reflect the reduced quantity.

**Actual result**: The system displays a message indicating quantity reduction but does not adjust the final order quantity. This can lead to discrepancies between the order and the actual inventory.

<p align="center">
  <img src="https://github.com/dudekluk/Portfolio/blob/main/img/BR14.png" alt="Image" width="70%" height="70%">
</p>

<h2 id="Bug-Reports">7. Multiple free promotion items added to cart.</h2>

**Description**: The system allows users to add multiple free promotional items to their cart, even if the promotion terms only allow for one free item per order.

**Expected result**: The system should limit the number of free promotional items added to the cart to the specified limit. A clear message should be displayed to the user if they attempt to add more than the allowed quantity.

**Actual result**: Users can add multiple free promotional items to their cart, potentially leading to incorrect order processing and fulfillment issues. 


<p align="center">
  <img src="https://github.com/dudekluk/Portfolio/blob/main/img/BR12.png" alt="Image" width="70%" height="70%">
</p>


<h2 id="Bug-Reports">8. Missing margin in order details input form.</h2>

**Description**: The input fields in the order details section are too close to the screen edge.

**Expected result**: The input fields should have appropriate spacing and margins between screen edge to improve readability and usability.

**Actual result**: The input fields are to close to the edge, making it challenging for users to enter information accurately.

<p align="center">
  <img src="https://github.com/dudekluk/Portfolio/blob/main/img/BR3.png" alt="Image" width="70%" height="70%">
</p>

<h2 id="Bug-Reports">9. Inconsistent product item box sizes.</h2>

**Description**: The product item boxes on the product listing page are not consistently sized, making it difficult to compare products and navigate the page. 

**Expected result**: Product item boxes should have consistent sizes to improve visual clarity and user experience.

**Actual result**: Product item boxes vary in size, leading to a cluttered and disorganized appearance. 

<p align="center">
  <img src="https://github.com/dudekluk/Portfolio/blob/main/img/BR2.png" alt="Image" width="70%" height="70%">
</p>

<h2 id="Bug-Reports">10. Comparison feature not functioning.</h2>

**Description**: When attempting to compare two products, the comparison feature initiates but fails to load the comparison page. The page remains in a loading state indefinitely.
 
**Expected result**: Upon selecting two products for comparison, the system should display a comparison page highlighting the key differences and similarities between the products.

**Actual result**: The comparison page fails to load, leaving the user unable to make informed purchasing decisions.

<p align="center">
  <img src="https://github.com/dudekluk/Portfolio/blob/main/img/BR5.png" alt="Image" width="70%" height="70%">
</p>

<h2 id="Bug-Reports">11. Incorrect and unwanted UI elements on product page.</h2>

**Description**: When a user clicks on an item from the order page, they are redirected to the correct product page. However, the page displays multiple unexpected messages and buttons, interfering with the user experience. 

**Expected result**: Upon clicking an item from the order page, the user should be redirected to the correct product page, displaying the product information without any additional, irrelevant elements.

**Actual result**: The user is redirected to the product page, but the page displays multiple unexpected messages and buttons, making it difficult to view product details and take further actions.


<p align="center">
  <img src="https://github.com/dudekluk/Portfolio/blob/main/img/BR7.png" alt="Image" width="70%" height="70%">
</p>
<h2 id="Bug-Reports">12. Incorrect search results.</h2>

**Description**:  When searching for a fraze, such as "Chiara Sta," the search results include irrelevant items that do not match the search query.

**Expected result**: The search results should only display items that match the search query. In this case, the results should be related to "Chiara Sta" and not include unrelated items.

**Actual result**: The search results include items that are not relevant to the search query, making it difficult for users to find the desired information.

<p align="center">
  <img src="https://github.com/dudekluk/Portfolio/blob/main/img/BR9.png" alt="Image" width="70%" height="70%">
</p>

<h2 id="Bug-Reports">13. Duplicate items added to cart. </h2>

**Description**: When a user adds an item to the cart multiple times, the item is duplicated in the cart instead of increasing the quantity of the existing item. 

**Expected result**: Adding the same item multiple times should increase the quantity of that item in the cart, rather than creating multiple entries.

**Actual result**: The system adds multiple instances of the same item to the cart, leading to incorrect calculations of the total price and potential issues during checkout.


<p align="center">
  <img src="https://github.com/dudekluk/Portfolio/blob/main/img/BR10.png" alt="Image" width="70%" height="70%">
</p>
<h2 id="Bug-Reports">14. Incorrect error message during product filtering.</h2>

**Description**: When applying filters to a product list, and products match the criteria, the system displays an incorrect error message stating "Brak produktów spełniających wybrane kryteria."

**Expected result**: When products match the applied filters, the system should not display any errors.

**Actual result**: The system displays an incorrect error message creating a confusing and misleading user experience. 

<p align="center">
  <img src="https://github.com/dudekluk/Portfolio/blob/main/img/BR11.png" alt="Image" width="70%" height="70%">
</p>

<h2 id="Bug-Reports">15.Page refresh on quantity change </h2>

**Description**: When a user adjusts the quantity of an item in the cart using the "+" or "-" buttons, the entire page refreshes, interrupting the user experience.

**Expected result**: The quantity should be updated without a full page refresh. The cart total and other relevant information should be updated dynamically.

**Actual result**: The page refreshes, potentially causing the user to lose their place or disrupting their shopping experience.






<h2 id="Bug-Reports">16. Filter reset on brand filter application</h2>

**Description**: When a user applies a filter by brand, other previously selected filters (e.g., price range, category) are unexpectedly reset. 
 

**Expected result**: Applying a brand filter should not clear other active filters. Users should be able to combine multiple filters to refine their search results.


**Actual result**: The system resets all other filters when a brand filter is applied, limiting the user's ability to refine the search results.


