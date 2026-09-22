# Shopping Cart Test Execution Results

## Test Environment

- Application: SauceDemo
- Platform: Desktop Web
- Browser: Google Chrome
- Test Type: Manual Testing

## Execution Results

| Test Case | Actual Result | Status |
|---|---|---|
| TC-CART-001 | Shopping Cart page opened successfully from the Products page. | Pass |
| TC-CART-002 | Added product was displayed in the cart. Product name, description, and price matched the Products page. | Pass |
| TC-CART-003 | Three products were successfully added to the cart. Cart badge displayed `3` and all three products were present in the cart. | Pass |
| TC-CART-004 | One product was successfully removed. Two products remained in the cart and the cart badge changed from `3` to `2`. | Pass |
| TC-CART-005 | All products were successfully removed from the cart. The cart became empty and the cart badge disappeared. | Pass |
| TC-CART-006 | Continue Shopping returned the user to the Products page. Previously added product remained in the cart and the cart count was preserved. | Pass |
| TC-CART-007 | Checkout button successfully opened the Checkout Information page. | Pass |
