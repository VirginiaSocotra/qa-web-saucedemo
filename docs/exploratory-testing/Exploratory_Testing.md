# Exploratory Testing

## Objective

Explore SauceDemo beyond predefined test cases in order to identify unexpected functional, UI, usability, data, and performance issues.

## Session 1 — Problem User

### Findings

#### EX-PU-01 — Incorrect product images are displayed in the catalog

**Area:** Product Catalog

**Observation:** Product images displayed on the Products page do not correspond to the actual products.

**Potential Impact:** Users receive misleading visual information while browsing the product catalog.

**Needs Bug Report:** Yes


#### EX-PU-02 — Product card opens a different product on the Product Details page

**Area:** Product Catalog / Product Details

**Observation:** A product card on the Products page displays the name and price of one product, but after opening the product, the Product Details page displays the name and price of a different product.

The image displayed on the Product Details page corresponds to the product shown in the details.

**Potential Impact:** Users may select one product from the catalog but be redirected to a different product with different information and price.

**Needs Bug Report:** Yes


#### EX-PU-03 — Only specific products can be added to the shopping cart

**Area:** Product Catalog / Product Details / Shopping Cart

**Observation:** Only three specific products can be successfully added to the shopping cart. Other products do not respond correctly to the Add to cart action.

**Potential Impact:** Users cannot purchase all products available in the catalog.

**Needs Bug Report:** Yes


#### EX-PU-04 — Invalid data is displayed for Sauce Labs Fleece Jacket

**Area:** Product Details

**Observation:** Sauce Labs Fleece Jacket displays invalid product information:
- Name: `ITEM NOT FOUND`
- Unexpected error text is displayed as the description
- Price: `$√-1`

**Potential Impact:** Product information is unusable and misleading.

**Needs Bug Report:** Yes


#### EX-PU-05 — Remove action does not work correctly outside the Shopping Cart

**Area:** Product Catalog / Product Details / Shopping Cart

**Observation:** For products that can be successfully added to the cart, the Add to cart button changes to Remove.

However, clicking Remove on the Products page or Product Details page does not correctly remove the product, the button does not change back to Add to cart, and the cart badge is not updated correctly.

The same products can be removed successfully from inside the Shopping Cart page.

**Potential Impact:** Users cannot reliably manage shopping cart contents from the Products page or Product Details page.

**Needs Bug Report:** Yes


#### EX-PU-06 — Product sorting does not work

**Area:** Product Catalog

**Observation:** Changing the sorting option does not correctly reorder the products.

**Potential Impact:** Users cannot sort products as expected.

**Needs Bug Report:** Yes


#### EX-PU-07 — Add to Cart action fails for some products on Product Details page

**Area:** Product Details / Shopping Cart

**Observation:** For some products, clicking the Add to cart button on the Product Details page does not add the product to the shopping cart.

**Potential Impact:** Users cannot add some products to the cart from the Product Details page.

**Needs Bug Report:** Yes


#### EX-PU-08 — Last Name input is entered into First Name field

**Area:** Checkout Information

**Observation:** Characters entered into the Last Name field appear in the First Name field while the Last Name field remains empty.

**Potential Impact:** Users cannot correctly enter checkout information.

**Needs Bug Report:** Yes

## Session 2 — Performance Glitch User

### Finding EX-PG-01 — Noticeable delays during common user actions

**Area:** Application Performance

**Observation:** Noticeable delays occur during multiple user actions:
- After login before the Products page appears
- After clicking Back to products
- After changing the sorting option
- After clicking Continue Shopping

**Potential Impact:** Slow application response negatively affects user experience and navigation efficiency.

**Needs Bug Report:** Yes

## Session 3 — Visual User

### Findings

#### EX-VU-01 — Product image is not loaded correctly
**Area:** Product Catalog  
**Observation:** A product image placeholder is displayed instead of the expected product image.  
**Needs Bug Report:** Yes

#### EX-VU-02 — Product prices change after page refresh
**Area:** Product Catalog  
**Observation:** Product prices change unexpectedly when the Products page is refreshed.  
**Potential Impact:** Users may see inconsistent pricing information.  
**Needs Bug Report:** Yes

#### EX-VU-03 — Shopping cart icon is incorrectly positioned
**Area:** Header / Navigation  
**Observation:** The shopping cart icon is visually misaligned.  
**Needs Bug Report:** Yes

#### EX-VU-04 — Menu icon is misaligned
**Area:** Header / Navigation  
**Observation:** The menu icon is not aligned correctly with the surrounding UI elements.  
**Needs Bug Report:** Yes

#### EX-VU-05 — Checkout button is incorrectly positioned
**Area:** Shopping Cart  
**Observation:** The Checkout button is displayed in an incorrect position on the Shopping Cart page.  
**Needs Bug Report:** Yes

## Session 4 — Error User

### Findings

#### EX-EU-01 — Add to Cart works only for some products
**Area:** Product Catalog  
**Observation:** The Add to Cart button works only for three products; other products cannot be added to the cart.  
**Potential Impact:** Users cannot purchase all available products.  
**Needs Bug Report:** Yes

#### EX-EU-02 — Remove button does not work
**Area:** Product Catalog / Shopping Cart  
**Observation:** The Remove button cannot be clicked for selected products and does not change back to Add to cart.  
**Potential Impact:** Users cannot remove selected products from the cart.  
**Needs Bug Report:** Yes

#### EX-EU-03 — Product sorting returns an error
**Area:** Product Catalog  
**Observation:** None of the sorting options work. The application displays: `Sorting is broken! This error has been reported to Backtrace.`  
**Potential Impact:** Product sorting functionality is unavailable.  
**Needs Bug Report:** Yes

#### EX-EU-04 — Product description is missing
**Area:** Product Details  
**Observation:** Product description is not displayed on the Product Details page.  
**Potential Impact:** Users cannot view complete product information.  
**Needs Bug Report:** Yes

#### EX-EU-05 — Last Name field does not accept input
**Area:** Checkout Information  
**Observation:** Characters cannot be entered into the Last Name field.  
**Potential Impact:** Users cannot complete the required checkout information.  
**Needs Bug Report:** Yes

#### EX-EU-06 — Finish button does not work
**Area:** Checkout  
**Observation:** Clicking the Finish button does not complete the checkout process.  
**Potential Impact:** Users cannot complete an order.  
**Needs Bug Report:** Yes

## General Findings — All Users

### EX-GEN-01 — Cancel button arrow is misaligned

**Area:** Checkout Information  
**Observation:** The arrow/icon associated with the Cancel button is visually misaligned.  
**Potential Impact:** Minor visual inconsistency.  
**Needs Bug Report:** Yes


### EX-GEN-02 — Checkout can be completed with an empty cart

**Area:** Checkout

**Observation:** A user can proceed through checkout with an empty shopping cart and receive a successful purchase confirmation.

**Potential Impact:** The application allows an invalid order with no products to be completed.

**Needs Bug Report:** Yes
