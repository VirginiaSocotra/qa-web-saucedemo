# Shopping Cart Test Cases

## TC-CART-001 — Open shopping cart from Products page

**Related Scenario:** CS-01  
**Priority:** High  
**Type:** Functional / Positive

### Preconditions
- User is logged in.
- Products page is displayed.

### Steps
1. Click the shopping cart icon.

### Expected Result
- Shopping Cart page is opened.
- Cart content area is displayed.


## TC-CART-002 — Verify added product in shopping cart

**Related Scenarios:** CS-02, CS-03  
**Priority:** High  
**Type:** Functional / Positive

### Preconditions
- User is logged in.
- Products page is displayed.
- Shopping cart is empty.

### Test Data
- Product: Sauce Labs Backpack

### Steps
1. Add `Sauce Labs Backpack` to the cart.
2. Open the shopping cart.
3. Verify that the product is displayed.
4. Compare the product name with the Products page.
5. Compare the product description with the Products page.
6. Compare the product price with the Products page.

### Expected Result
- Sauce Labs Backpack is displayed in the shopping cart.
- Product name matches the Products page.
- Product description matches the Products page.
- Product price matches the Products page.


## TC-CART-003 — Add multiple products to shopping cart

**Related Scenarios:** CS-04, CS-05  
**Priority:** High  
**Type:** Functional / Positive

### Preconditions
- User is logged in.
- Products page is displayed.
- Shopping cart is empty.

### Test Data
- Three different products

### Steps
1. Add the first product to the cart.
2. Add the second product to the cart.
3. Add the third product to the cart.
4. Check the cart badge.
5. Open the shopping cart.

### Expected Result
- All three products are added to the shopping cart.
- Cart badge displays `3`.
- All three selected products are displayed in the cart.
- No unexpected duplicate products are displayed.


## TC-CART-004 — Remove one product from a cart containing multiple products

**Related Scenarios:** CS-06, CS-07  
**Priority:** High  
**Type:** Functional / Positive

### Preconditions
- User is logged in.
- Shopping cart contains 3 different products.

### Steps
1. Open the shopping cart.
2. Remove one product.
3. Review the remaining products.
4. Check the cart badge.

### Expected Result
- Selected product is removed from the cart.
- Two products remain in the cart.
- Remaining products are unchanged.
- Cart badge changes from `3` to `2`.


## TC-CART-005 — Remove all products from shopping cart

**Related Scenarios:** CS-08, CS-09  
**Priority:** High  
**Type:** Functional / Positive

### Preconditions
- User is logged in.
- Shopping cart contains one or more products.

### Steps
1. Open the shopping cart.
2. Remove all products one by one.
3. Review the shopping cart.
4. Check the cart badge.

### Expected Result
- All products are removed from the cart.
- Shopping cart contains no products.
- Cart badge is no longer displayed.


## TC-CART-006 — Continue shopping from shopping cart

**Related Scenarios:** CS-10, CS-11  
**Priority:** Medium  
**Type:** Functional / Positive

### Preconditions
- User is logged in.
- Shopping cart contains at least one product.
- Shopping Cart page is displayed.

### Steps
1. Click the Continue Shopping button.
2. Verify the displayed page.
3. Check the cart badge.
4. Open the shopping cart again.

### Expected Result
- User is returned to the Products page.
- Previously added product remains in the cart.
- Cart badge retains the correct product count.
- Previously added product is still displayed after reopening the cart.


## TC-CART-007 — Proceed to checkout with product in cart

**Related Scenario:** CS-12  
**Priority:** High  
**Type:** Functional / Positive

### Preconditions
- User is logged in.
- Shopping cart contains at least one product.
- Shopping Cart page is displayed.

### Steps
1. Click the Checkout button.

### Expected Result
- Checkout page is opened.
- Checkout information form is displayed.
