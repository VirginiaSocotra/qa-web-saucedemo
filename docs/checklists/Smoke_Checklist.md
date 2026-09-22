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
| SM-01 | Open SauceDemo Login page | Login page is loaded successfully | Not Run |
| SM-02 | Login with valid credentials | User is redirected to the Products page | Not Run |
| SM-03 | Verify Products page is displayed | Product catalog is visible | Not Run |
| SM-04 | Add one product to the cart | Product is added and cart badge displays `1` | Not Run |
| SM-05 | Open shopping cart | Shopping Cart page is displayed | Not Run |
| SM-06 | Verify added product is present in the cart | Selected product is displayed in the cart | Not Run |
| SM-07 | Proceed to checkout | Checkout Information page is displayed | Not Run |
| SM-08 | Enter valid checkout information and continue | Checkout Overview page is displayed | Not Run |
| SM-09 | Complete the order | Order is completed successfully | Not Run |
| SM-10 | Verify order confirmation | Confirmation message is displayed | Not Run |
| SM-11 | Return to Products page | Products page is displayed | Not Run |
| SM-12 | Logout | User is redirected to the Login page | Not Run |
