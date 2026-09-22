# Smoke Testing Checklist

## Objective

Verify that the critical functionality of the SauceDemo application is working and that the application is stable enough for further testing.

## Test Environment

- Application: SauceDemo
- Platform: Desktop Web
- Browser: Google Chrome
- Test Type: Manual Smoke Testing

## Smoke Checklist

| ID | Check | Expected Result | Status |
|---|---|---|---|
| SM-01 | Open SauceDemo Login page | Login page is loaded successfully | Pass |
| SM-02 | Login with valid credentials | User is redirected to the Products page | Pass |
| SM-03 | Verify Products page is displayed | Product catalog is visible | Pass |
| SM-04 | Add one product to the cart | Product is added and cart badge displays `1` | Pass |
| SM-05 | Open shopping cart | Shopping Cart page is displayed | Pass |
| SM-06 | Verify added product is present in the cart | Selected product is displayed in the cart | Pass |
| SM-07 | Proceed to checkout | Checkout Information page is displayed | Pass |
| SM-08 | Enter valid checkout information and continue | Checkout Overview page is displayed | Pass |
| SM-09 | Complete the order | Order is completed successfully | Pass |
| SM-10 | Verify order confirmation | Confirmation message is displayed | Pass |
| SM-11 | Return to Products page | Products page is displayed | Pass |
| SM-12 | Logout | User is redirected to the Login page | Pass |

## Summary

- Total checks: 12
- Passed: 12
- Failed: 0
- Blocked: 0

### Result

Smoke testing passed. Critical application functionality is working and the application is stable for further testing.
