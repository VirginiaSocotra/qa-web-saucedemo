# Checkout Test Cases

## TC-CHECKOUT-001 — Open Checkout Information page

**Related Scenario:** CHS-01  
**Priority:** High  
**Type:** Functional / Positive

### Preconditions
- User is logged in.
- Shopping cart contains at least one product.
- Shopping Cart page is displayed.

### Steps
1. Click the Checkout button.

### Expected Result
- Checkout Information page is opened.
- First Name field is displayed.
- Last Name field is displayed.
- Postal Code field is displayed.


## TC-CHECKOUT-002 — Continue checkout with valid customer information

**Related Scenario:** CHS-02  
**Priority:** High  
**Type:** Functional / Positive

### Preconditions
- Checkout Information page is displayed.
- Shopping cart contains at least one product.

### Test Data
- First Name: Anna
- Last Name: Test
- Postal Code: 81101

### Steps
1. Enter `Anna` into the First Name field.
2. Enter `Test` into the Last Name field.
3. Enter `81101` into the Postal Code field.
4. Click the Continue button.

### Expected Result
- Customer information is accepted.
- Checkout Overview page is displayed.


## TC-CHECKOUT-003 — Verify Checkout Overview information

**Related Scenarios:** CHS-03, CHS-04  
**Priority:** High  
**Type:** Functional

### Preconditions
- User has entered valid customer information.
- Checkout Overview page is displayed.

### Steps
1. Review the product displayed on the Checkout Overview page.
2. Verify the product name.
3. Verify the product description.
4. Verify the product price.
5. Compare the information with the product added to the cart.

### Expected Result
- Checkout Overview page is displayed correctly.
- Product name matches the product in the cart.
- Product description matches the product in the cart.
- Product price matches the product in the cart.


## TC-CHECKOUT-004 — Verify checkout totals

**Related Scenarios:** CHS-05, CHS-06, CHS-07  
**Priority:** High  
**Type:** Functional / Calculation

### Preconditions
- Checkout Overview page is displayed.
- At least one product is included in the order.

### Steps
1. Review the Item total.
2. Compare the Item total with the sum of product prices.
3. Verify that Tax is displayed.
4. Review the Total amount.
5. Verify that the Total amount includes the Item total and Tax.

### Expected Result
- Item total matches the sum of product prices.
- Tax is displayed.
- Total amount is calculated correctly from the displayed Item total and Tax.


## TC-CHECKOUT-005 — Complete checkout successfully

**Related Scenarios:** CHS-08, CHS-09  
**Priority:** High  
**Type:** Functional / Positive

### Preconditions
- Checkout Overview page is displayed.
- Order information is valid.

### Steps
1. Click the Finish button.
2. Review the resulting page.

### Expected Result
- Checkout is completed successfully.
- Order confirmation page is displayed.
- A confirmation message is displayed.


## TC-CHECKOUT-006 — Cancel checkout from Checkout Information page

**Related Scenario:** CHS-10  
**Priority:** Medium  
**Type:** Functional

### Preconditions
- Checkout Information page is displayed.

### Steps
1. Click the Cancel button.

### Expected Result
- Checkout process is cancelled.
- User is returned to the Shopping Cart page.


## TC-CHECKOUT-007 — Cancel checkout from Checkout Overview page

**Related Scenario:** CHS-11  
**Priority:** Medium  
**Type:** Functional

### Preconditions
- Checkout Overview page is displayed.

### Steps
1. Click the Cancel button.

### Expected Result
- Checkout process is cancelled.
- User is returned to the Products page.


## TC-CHECKOUT-008 — Continue checkout with empty First Name

**Related Scenario:** CHS-12  
**Priority:** High  
**Type:** Validation / Negative

### Preconditions
- Checkout Information page is displayed.

### Test Data
- First Name: empty
- Last Name: Test
- Postal Code: 81101

### Steps
1. Leave the First Name field empty.
2. Enter `Test` into the Last Name field.
3. Enter `81101` into the Postal Code field.
4. Click the Continue button.

### Expected Result
- Checkout does not continue.
- User remains on the Checkout Information page.
- Validation error indicating that First Name is required is displayed.


## TC-CHECKOUT-009 — Continue checkout with empty Last Name

**Related Scenario:** CHS-13  
**Priority:** High  
**Type:** Validation / Negative

### Preconditions
- Checkout Information page is displayed.

### Test Data
- First Name: Anna
- Last Name: empty
- Postal Code: 81101

### Steps
1. Enter `Anna` into the First Name field.
2. Leave the Last Name field empty.
3. Enter `81101` into the Postal Code field.
4. Click the Continue button.

### Expected Result
- Checkout does not continue.
- User remains on the Checkout Information page.
- Validation error indicating that Last Name is required is displayed.


## TC-CHECKOUT-010 — Continue checkout with empty Postal Code

**Related Scenario:** CHS-14  
**Priority:** High  
**Type:** Validation / Negative

### Preconditions
- Checkout Information page is displayed.

### Test Data
- First Name: Anna
- Last Name: Test
- Postal Code: empty

### Steps
1. Enter `Anna` into the First Name field.
2. Enter `Test` into the Last Name field.
3. Leave the Postal Code field empty.
4. Click the Continue button.

### Expected Result
- Checkout does not continue.
- User remains on the Checkout Information page.
- Validation error indicating that Postal Code is required is displayed.


## TC-CHECKOUT-011 — Continue checkout with all customer information fields empty

**Related Scenario:** CHS-15  
**Priority:** High  
**Type:** Validation / Negative

### Preconditions
- Checkout Information page is displayed.

### Test Data
- First Name: empty
- Last Name: empty
- Postal Code: empty

### Steps
1. Leave the First Name field empty.
2. Leave the Last Name field empty.
3. Leave the Postal Code field empty.
4. Click the Continue button.

### Expected Result
- Checkout does not continue.
- User remains on the Checkout Information page.
- Validation error indicating that First Name is required is displayed.
