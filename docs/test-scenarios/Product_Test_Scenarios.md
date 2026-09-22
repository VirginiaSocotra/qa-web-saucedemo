# Product Catalog Test Scenarios

## Feature

Product Catalog

## Objective

Verify that the product catalog displays product information correctly and allows the user to interact with products as expected.

## Functional Scenarios

| ID | Test Scenario |
|---|---|
| PS-01 | Verify that the Products page is displayed after successful login |
| PS-02 | Verify that the product list is displayed |
| PS-03 | Verify that each product has a name |
| PS-04 | Verify that each product has a description |
| PS-05 | Verify that each product has a price |
| PS-06 | Verify that each product has an image |
| PS-07 | Open product details by clicking the product name |
| PS-08 | Open product details by clicking the product image |
| PS-09 | Verify product information on the product details page |
| PS-10 | Return from the product details page to the product catalog |
| PS-11 | Add a product to the cart from the product catalog |
| PS-12 | Remove a product from the cart from the product catalog |

## Sorting Scenarios

| ID | Test Scenario |
|---|---|
| PS-13 | Sort products by name from A to Z |
| PS-14 | Sort products by name from Z to A |
| PS-15 | Sort products by price from low to high |
| PS-16 | Sort products by price from high to low |

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
