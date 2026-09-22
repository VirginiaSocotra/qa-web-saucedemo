# Product Catalog Test Cases

## TC-PRODUCT-001 — Display Products page after successful login

**Related Scenario:** PS-01  
**Priority:** High  
**Type:** Functional / Positive

### Preconditions
- User is on the SauceDemo Login page.
- User account is active.

### Test Data
- Username: standard_user
- Password: secret_sauce

### Steps
1. Enter `standard_user` into the Username field.
2. Enter `secret_sauce` into the Password field.
3. Click the Login button.

### Expected Result
- User is successfully authenticated.
- Products page is displayed.
- Product catalog is visible.


## TC-PRODUCT-002 — Verify product information for all displayed products

**Related Scenarios:** PS-02, PS-03, PS-04, PS-05, PS-06  
**Priority:** High  
**Type:** Functional / UI

### Preconditions
- User is logged in.
- Products page is displayed.

### Steps
1. Review all products displayed in the catalog.
2. Verify that each product contains a product name.
3. Verify that each product contains a description.
4. Verify that each product contains a price.
5. Verify that each product contains an image.
6. Verify that each product contains an Add to cart button.

### Expected Result
- 6 products are displayed.
- Each product contains a name.
- Each product contains a description.
- Each product contains a price.
- Each product contains an image.
- Each product contains an Add to cart button.


## TC-PRODUCT-003 — Open product details by clicking product name

**Related Scenario:** PS-07  
**Priority:** Medium  
**Type:** Functional / Positive

### Preconditions
- User is logged in.
- Products page is displayed.

### Test Data
- Product: Sauce Labs Backpack

### Steps
1. Locate `Sauce Labs Backpack` in the product catalog.
2. Click the product name.

### Expected Result
- Product Details page is opened.
- Sauce Labs Backpack product information is displayed.


## TC-PRODUCT-004 — Open product details by clicking product image

**Related Scenario:** PS-08  
**Priority:** Medium  
**Type:** Functional / Positive

### Preconditions
- User is logged in.
- Products page is displayed.

### Test Data
- Product: Sauce Labs Backpack

### Steps
1. Locate `Sauce Labs Backpack` in the product catalog.
2. Click the product image.

### Expected Result
- Product Details page is opened.
- Sauce Labs Backpack product information is displayed.


## TC-PRODUCT-005 — Verify product information consistency

**Related Scenario:** PS-09  
**Priority:** High  
**Type:** Functional

### Preconditions
- User is logged in.
- Products page is displayed.

### Test Data
- Product: Sauce Labs Backpack

### Steps
1. Locate `Sauce Labs Backpack` on the Products page.
2. Note the product name.
3. Note the product description.
4. Note the product price.
5. Note the product image.
6. Open the Product Details page.
7. Compare the displayed product information with the information from the Products page.

### Expected Result
- Product name matches the Products page.
- Product description matches the Products page.
- Product price matches the Products page.
- Product image corresponds to the same product.


## TC-PRODUCT-006 — Return to Products page from Product Details

**Related Scenario:** PS-10  
**Priority:** Medium  
**Type:** Functional / Positive

### Preconditions
- User is logged in.
- Product Details page is displayed.

### Steps
1. Click the Back to products button.

### Expected Result
- User is returned to the Products page.
- Product catalog is displayed.


## TC-PRODUCT-007 — Add product to cart from Products page

**Related Scenario:** PS-11  
**Priority:** High  
**Type:** Functional / Positive

### Preconditions
- User is logged in.
- Products page is displayed.
- Shopping cart is empty.

### Test Data
- Product: Sauce Labs Backpack

### Steps
1. Locate `Sauce Labs Backpack`.
2. Click the Add to cart button.

### Expected Result
- Product is added to the shopping cart.
- Add to cart button changes to Remove.
- Cart badge displays `1`.


## TC-PRODUCT-008 — Remove product from cart from Products page

**Related Scenario:** PS-12  
**Priority:** High  
**Type:** Functional / Positive

### Preconditions
- User is logged in.
- Products page is displayed.
- Sauce Labs Backpack is added to the shopping cart.

### Test Data
- Product: Sauce Labs Backpack

### Steps
1. Locate `Sauce Labs Backpack`.
2. Click the Remove button.

### Expected Result
- Product is removed from the shopping cart.
- Remove button changes to Add to cart.
- Cart badge is no longer displayed when the cart becomes empty.


## TC-PRODUCT-009 — Sort products by name from A to Z

**Related Scenario:** PS-13  
**Priority:** Medium  
**Type:** Functional / Positive

### Preconditions
- User is logged in.
- Products page is displayed.

### Steps
1. Open the sorting dropdown.
2. Select `Name (A to Z)`.
3. Review the order of all displayed product names.

### Expected Result
- Products are displayed in alphabetical order from A to Z.
- All 6 products remain visible after sorting.


## TC-PRODUCT-010 — Sort products by name from Z to A

**Related Scenario:** PS-14  
**Priority:** Medium  
**Type:** Functional / Positive

### Preconditions
- User is logged in.
- Products page is displayed.

### Steps
1. Open the sorting dropdown.
2. Select `Name (Z to A)`.
3. Review the order of all displayed product names.

### Expected Result
- Products are displayed in reverse alphabetical order from Z to A.
- All 6 products remain visible after sorting.


## TC-PRODUCT-011 — Sort products by price from low to high

**Related Scenario:** PS-15  
**Priority:** Medium  
**Type:** Functional / Positive

### Preconditions
- User is logged in.
- Products page is displayed.

### Steps
1. Open the sorting dropdown.
2. Select `Price (low to high)`.
3. Review the prices of all displayed products from top to bottom.

### Expected Result
- Products are displayed in ascending order by price.
- Each next product price is greater than or equal to the previous product price.
- All 6 products remain visible after sorting.


## TC-PRODUCT-012 — Sort products by price from high to low

**Related Scenario:** PS-16  
**Priority:** Medium  
**Type:** Functional / Positive

### Preconditions
- User is logged in.
- Products page is displayed.

### Steps
1. Open the sorting dropdown.
2. Select `Price (high to low)`.
3. Review the prices of all displayed products from top to bottom.

### Expected Result
- Products are displayed in descending order by price.
- Each next product price is less than or equal to the previous product price.
- All 6 products remain visible after sorting.
