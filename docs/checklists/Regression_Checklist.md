# Regression Testing Checklist

## Objective

Verify that existing SauceDemo functionality continues to work correctly after application changes.

## Test Environment

- Application: SauceDemo
- Platform: Desktop Web
- Browser: Google Chrome
- Test Type: Manual Regression Testing

## Login

| ID | Check | Expected Result | Status |
|---|---|---|---|
| RG-LOGIN-01 | Login with valid credentials | User is redirected to the Products page | Not Run |
| RG-LOGIN-02 | Login with invalid password | Login is rejected and error message is displayed | Not Run |
| RG-LOGIN-03 | Login with invalid username | Login is rejected and error message is displayed | Not Run |
| RG-LOGIN-04 | Login with empty username | Required username validation message is displayed | Not Run |
| RG-LOGIN-05 | Login with empty password | Required password validation message is displayed | Not Run |
| RG-LOGIN-06 | Login using locked-out user | Login is rejected and locked-out message is displayed | Not Run |

## Product Catalog

| ID | Check | Expected Result | Status |
|---|---|---|---|
| RG-PRODUCT-01 | Verify product catalog is displayed | All expected products are visible | Not Run |
| RG-PRODUCT-02 | Verify product information | Name, description, price and image are displayed | Not Run |
| RG-PRODUCT-03 | Open product using product name | Correct Product Details page is opened | Not Run |
| RG-PRODUCT-04 | Open product using product image | Correct Product Details page is opened | Not Run |
| RG-PRODUCT-05 | Verify product details consistency | Product information matches the catalog | Not Run |
| RG-PRODUCT-06 | Return from Product Details | User returns to the Products page | Not Run |

## Product Sorting

| ID | Check | Expected Result | Status |
|---|---|---|---|
| RG-SORT-01 | Sort Name A to Z | Products are displayed alphabetically A to Z | Not Run |
| RG-SORT-02 | Sort Name Z to A | Products are displayed alphabetically Z to A | Not Run |
| RG-SORT-03 | Sort Price low to high | Products are displayed in ascending price order | Not Run |
| RG-SORT-04 | Sort Price high to low | Products are displayed in descending price order | Not Run |

## Shopping Cart

| ID | Check | Expected Result | Status |
|---|---|---|---|
| RG-CART-01 | Add one product to cart | Product is added and badge is updated | Not Run |
| RG-CART-02 | Add multiple products | All selected products are added and badge count is correct | Not Run |
| RG-CART-03 | Verify product information in cart | Product information matches the catalog | Not Run |
| RG-CART-04 | Remove one product | Product is removed and badge count decreases | Not Run |
| RG-CART-05 | Remove all products | Cart becomes empty and badge disappears | Not Run |
| RG-CART-06 | Continue Shopping | User returns to Products page and cart contents are preserved | Not Run |
| RG-CART-07 | Open Checkout | Checkout Information page is displayed | Not Run |

## Checkout

| ID | Check | Expected Result | Status |
|---|---|---|---|
| RG-CHECKOUT-01 | Continue with valid customer information | Checkout Overview page is displayed | Not Run |
| RG-CHECKOUT-02 | Submit empty First Name | First Name validation message is displayed | Not Run |
| RG-CHECKOUT-03 | Submit empty Last Name | Last Name validation message is displayed | Not Run |
| RG-CHECKOUT-04 | Submit empty Postal Code | Postal Code validation message is displayed | Not Run |
| RG-CHECKOUT-05 | Verify checkout product information | Product data matches shopping cart | Not Run |
| RG-CHECKOUT-06 | Verify item total | Item total matches product prices | Not Run |
| RG-CHECKOUT-07 | Verify tax and total | Tax is displayed and final total is calculated correctly | Not Run |
| RG-CHECKOUT-08 | Complete checkout | Order is completed successfully | Not Run |
| RG-CHECKOUT-09 | Verify confirmation message | Order confirmation message is displayed | Not Run |
| RG-CHECKOUT-10 | Cancel from Checkout Information | User returns to the Shopping Cart page | Not Run |
| RG-CHECKOUT-11 | Cancel from Checkout Overview | User returns to the Products page | Not Run |

## Navigation

| ID | Check | Expected Result | Status |
|---|---|---|---|
| RG-NAV-01 | Open navigation menu | Navigation menu is displayed | Not Run |
| RG-NAV-02 | Logout | User is redirected to the Login page | Not Run |
