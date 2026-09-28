# Bug Reports

## BUG-001 — Checkout can be completed with an empty cart

**Severity:** High  
**Priority:** High  
**Type:** Functional / Business Logic

### Environment
- Application: SauceDemo
- Platform: Desktop Web
- Browser: Google Chrome
- Test Account: standard_user

### Preconditions
- User is logged in.
- Shopping cart is empty.

### Steps to Reproduce
1. Open the shopping cart.
2. Click the Checkout button.
3. Enter valid customer information.
4. Click Continue.
5. Click Finish.

### Actual Result
Checkout is completed successfully and a purchase confirmation message is displayed even though the shopping cart is empty.

### Expected Result
Checkout should not be completed when the shopping cart contains no products.

### Impact
The application allows an invalid order with no products to be completed.


## BUG-002 — Invalid product data is displayed for Sauce Labs Fleece Jacket

**Severity:** High  
**Priority:** High  
**Type:** Functional / Data

### Environment
- Application: SauceDemo
- Platform: Desktop Web
- Browser: Google Chrome
- Test Account: problem_user

### Preconditions
- User is logged in as `problem_user`.
- Products page is displayed.

### Steps to Reproduce
1. Locate `Sauce Labs Fleece Jacket`.
2. Open the Product Details page.

### Actual Result
Invalid product information is displayed:
- Product name: `ITEM NOT FOUND`
- Unexpected system text is displayed as the description
- Product price is displayed as `$√-1`

### Expected Result
The Product Details page should display the correct product name, description, and price for Sauce Labs Fleece Jacket.

### Impact
Users receive invalid and misleading product information.


## BUG-003 — Shopping cart contains products different from those selected

**Severity:** High  
**Priority:** High  
**Type:** Functional / Shopping Cart

### Environment
- Application: SauceDemo
- Platform: Desktop Web
- Browser: Google Chrome
- Test Account: problem_user

### Preconditions
- User is logged in as `problem_user`.
- Products page is displayed.
- Shopping cart is empty.

### Steps to Reproduce
1. Add one or more products to the shopping cart.
2. Open the shopping cart.
3. Compare the cart contents with the products selected on the Products page.

### Actual Result
The shopping cart contains products that do not correspond to the products selected by the user.

### Expected Result
The shopping cart should contain exactly the products selected by the user.

### Impact
Users may purchase unintended products.


## BUG-004 — Last Name input appears in First Name field

**Severity:** High  
**Priority:** High  
**Type:** Functional / Form Input

### Environment
- Application: SauceDemo
- Platform: Desktop Web
- Browser: Google Chrome
- Test Account: problem_user

### Preconditions
- User is logged in as `problem_user`.
- Checkout Information page is displayed.

### Steps to Reproduce
1. Click the Last Name field.
2. Enter text into the Last Name field.

### Actual Result
Entered characters appear in the First Name field.
The Last Name field remains empty.

### Expected Result
Entered characters should appear only in the Last Name field.

### Impact
Users cannot correctly enter customer information required for checkout.


## BUG-005 — Add to Cart button does not work on Product Details page

**Severity:** High  
**Priority:** High  
**Type:** Functional / Shopping Cart

### Environment
- Application: SauceDemo
- Platform: Desktop Web
- Browser: Google Chrome
- Test Account: problem_user

### Preconditions
- User is logged in as `problem_user`.
- Product Details page is displayed.

### Steps to Reproduce
1. Open any product details page.
2. Click the Add to Cart button.
3. Check the cart badge.

### Actual Result
The product is not added to the shopping cart and the cart badge is not updated.

### Expected Result
The selected product should be added to the cart and the cart badge should be updated.

### Impact
Users cannot add products to the cart from the Product Details page.


## BUG-006 — Product sorting displays an application error

**Severity:** Medium  
**Priority:** High  
**Type:** Functional / Sorting

### Environment
- Application: SauceDemo
- Platform: Desktop Web
- Browser: Google Chrome
- Test Account: error_user

### Preconditions
- User is logged in as `error_user`.
- Products page is displayed.

### Steps to Reproduce
1. Open the product sorting dropdown.
2. Select any sorting option.
3. Observe the application behavior.

### Actual Result
Products are not sorted and the application displays the error:

`Sorting is broken! This error has been reported to Backtrace.`

### Expected Result
Products should be reordered according to the selected sorting option without displaying an error.

### Impact
Users cannot use product sorting functionality.


## BUG-007 — Product prices change after page refresh

**Severity:** High  
**Priority:** High  
**Type:** Functional / Data

### Environment
- Application: SauceDemo
- Platform: Desktop Web
- Browser: Google Chrome
- Test Account: visual_user

### Preconditions
- User is logged in as `visual_user`.
- Products page is displayed.

### Steps to Reproduce
1. Note the displayed product prices.
2. Refresh the Products page.
3. Compare the prices before and after the refresh.
4. Repeat the refresh if necessary.

### Actual Result
Product prices change unexpectedly after refreshing the page.

### Expected Result
Product prices should remain consistent after page refresh unless the product data has intentionally changed.

### Impact
Users receive inconsistent pricing information and may not know the actual product price.


## BUG-008 — Remove action does not update cart state

**Severity:** Medium  
**Priority:** High  
**Type:** Functional / Shopping Cart

### Environment
- Application: SauceDemo
- Platform: Desktop Web
- Browser: Google Chrome
- Test Account: problem_user

### Preconditions
- User is logged in as `problem_user`.
- At least one product has been added to the shopping cart.

### Steps to Reproduce
1. Add a product to the shopping cart.
2. Click the Remove button.
3. Observe the button state.
4. Check the cart badge.

### Actual Result
The Remove button does not change back to Add to cart and the cart badge is not updated correctly.

### Expected Result
The product should be removed.
The button should change back to Add to cart.
The cart badge should update to reflect the current number of products.

### Impact
The interface displays an incorrect shopping cart state.


## BUG-009 — Finish button does not complete checkout

**Severity:** High  
**Priority:** High  
**Type:** Functional / Checkout

### Environment
- Application: SauceDemo
- Platform: Desktop Web
- Browser: Google Chrome
- Test Account: error_user

### Preconditions
- User is logged in as `error_user`.
- At least one product is in the shopping cart.
- User has reached the Checkout Overview page.

### Steps to Reproduce
1. Complete the checkout information with valid data.
2. Continue to Checkout Overview.
3. Click the Finish button.

### Actual Result
Clicking the Finish button does not complete the checkout process.

### Expected Result
Checkout should be completed and the order confirmation page should be displayed.

### Impact
Users cannot complete their purchase.


## BUG-010 — Product images are not loaded correctly

**Severity:** Medium  
**Priority:** Medium  
**Type:** UI / Data

### Environment
- Application: SauceDemo
- Platform: Desktop Web
- Browser: Google Chrome
- Test Account: problem_user

### Preconditions
- User is logged in as `problem_user`.
- Products page is displayed.

### Steps to Reproduce
1. Review the product cards on the Products page.
2. Observe the product images.

### Actual Result
Product image placeholders or incorrect images are displayed instead of the correct product images.

### Expected Result
Each product card should display the image corresponding to that product.

### Impact
Users cannot visually identify products correctly.
