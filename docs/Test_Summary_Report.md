# Test Summary Report

## Project

SauceDemo Web Application Testing

## Objective

The purpose of this testing project was to evaluate the main functionality of the SauceDemo web application using manual testing techniques.

The testing covered authentication, product catalog functionality, shopping cart behavior, checkout flow, exploratory testing, smoke testing, and regression test preparation.

---

## Test Environment

- Application: SauceDemo
- Platform: Desktop Web
- Browser: Google Chrome
- Testing Type: Manual Testing

---

## Functional Areas Tested

- Login and Logout
- Product Catalog
- Product Details
- Product Sorting
- Shopping Cart
- Checkout
- Form Validation
- Navigation

---

## Test Execution Summary

| Test Area | Test Cases | Result |
|---|---:|---|
| Login | 9 | Passed |
| Product Catalog | 12 | Passed |
| Shopping Cart | 7 | Passed |
| Checkout | 11 | Passed |
| **Total** | **39** | **Passed** |

The formal test cases were executed against the main functional flow of the application.

---

## Smoke Testing

A smoke testing checklist was created to verify the critical user flow:

Login → Products → Add to Cart → Cart → Checkout → Complete Order → Logout

### Result

- Total checks: 12
- Passed: 12
- Failed: 0
- Blocked: 0

Smoke testing passed successfully.

---

## Regression Testing

A reusable regression checklist was prepared covering:

- Login
- Product Catalog
- Product Sorting
- Shopping Cart
- Checkout
- Navigation

The checklist is intended for future regression test cycles.

---

## Exploratory Testing

Exploratory testing was performed using multiple SauceDemo test accounts:

- problem_user
- performance_glitch_user
- visual_user
- error_user

The exploratory sessions focused on:

- Functional issues
- Product data consistency
- Shopping cart behavior
- UI issues
- Form input behavior
- Performance delays
- Checkout functionality

---

## Defects

A total of 10 detailed bug reports were documented.

The identified defects included:

- Business logic issues
- Shopping cart defects
- Incorrect product data
- Product mapping issues
- Sorting failures
- Checkout failures
- Form input defects
- Pricing inconsistencies
- UI and image issues

Selected defects include screenshots as supporting evidence.

---

## Test Design Techniques

The following testing approaches and techniques were used during the project:

- Positive Testing
- Negative Testing
- Equivalence Partitioning
- Input Validation Testing
- Exploratory Testing
- Functional Testing
- Smoke Testing
- Regression Testing

---

## Overall Result

The main functional flow using the standard user account worked successfully during formal testing.

Exploratory testing with additional test accounts revealed multiple functional, data, UI, and performance defects.

The project demonstrates the complete manual testing workflow from test planning and test design through execution, exploratory testing, defect reporting, and test summary reporting.
