# SauceDemo Manual QA Portfolio Project

## Overview

This repository contains a manual QA testing project for the SauceDemo e-commerce web application.

The project demonstrates a complete manual testing workflow, including test planning, test analysis, test case design, test execution, exploratory testing, defect reporting, smoke testing, regression test preparation, and test summary reporting.

Application under test:  
https://www.saucedemo.com/

---

## Project Objectives

The main objectives of this project were to:

- Verify the critical user flows of the application.
- Validate login, product catalog, shopping cart, and checkout functionality.
- Perform positive and negative testing.
- Verify form validation and error handling.
- Perform exploratory testing using different test accounts.
- Identify and document functional, data, UI, and performance defects.
- Prepare reusable smoke and regression testing checklists.

---

## Test Environment

| Parameter | Value |
|---|---|
| Application | SauceDemo |
| Platform | Desktop Web |
| Browser | Google Chrome |
| Testing Type | Manual Testing |

---

## Functional Areas Covered

| Area | Coverage |
|---|---|
| Authentication | Login, logout, invalid credentials, locked user, required fields |
| Product Catalog | Product information, product details, navigation |
| Sorting | Name A–Z, Name Z–A, Price Low–High, Price High–Low |
| Shopping Cart | Add, remove, multiple products, cart badge, cart persistence |
| Checkout | Customer information, validation, overview, totals, order completion |
| Navigation | Menu, product navigation, cart navigation |
| Exploratory Testing | Functional, UI, data, performance and usability issues |

---

## Test Execution Summary

| Test Area | Test Cases | Result |
|---|---:|---|
| Login | 9 | Passed |
| Product Catalog | 12 | Passed |
| Shopping Cart | 7 | Passed |
| Checkout | 11 | Passed |
| **Total** | **39** | **Passed** |

Formal functional test cases were executed using the standard application flow.

---

## Smoke Testing

A smoke test was executed to verify the critical end-to-end flow:

**Login → Products → Add to Cart → Cart → Checkout → Complete Order → Logout**

| Result | Count |
|---|---:|
| Passed | 12 |
| Failed | 0 |
| Blocked | 0 |
| **Total** | **12** |

**Smoke Test Result: Passed**

---

## Regression Testing

A reusable regression checklist was prepared for future regression cycles.

It covers:

- Login and authentication
- Product catalog
- Product sorting
- Shopping cart
- Checkout
- Navigation

The regression checklist was prepared but was not executed as a separate full regression cycle during this project.

---

## Exploratory Testing

Exploratory testing was performed using multiple SauceDemo test accounts:

- `problem_user`
- `performance_glitch_user`
- `visual_user`
- `error_user`

The sessions revealed additional issues that were not identified through the standard functional flow, including:

- Incorrect product data mapping
- Shopping cart behavior issues
- Form input defects
- Sorting failures
- UI inconsistencies
- Pricing inconsistencies
- Performance delays
- Checkout issues

---

## Defects

**10 detailed bug reports** were documented.

The defects include different categories and severity levels, such as:

- Business logic defects
- Shopping cart defects
- Checkout failures
- Product data issues
- Product mapping issues
- Form input defects
- Sorting failures
- Pricing inconsistencies
- UI defects

Selected bug reports include screenshots as supporting evidence.

See:  
[Bug Reports](docs/bug-reports/Bug_Reports.md)

---

## Test Design and Testing Approaches

The following approaches and techniques were used:

- Positive Testing
- Negative Testing
- Equivalence Partitioning
- Input Validation Testing
- Functional Testing
- Exploratory Testing
- Smoke Testing
- Regression Testing
- Risk-based prioritization of critical user flows

---

## Test Documentation

### Test Planning

- [Test Plan](docs/Test_Plan.md)
- [Test Summary Report](docs/Test_Summary_Report.md)

### Test Scenarios

- [Login Test Scenarios](docs/test-scenarios/Login_Test_Scenarios.md)
- [Product Test Scenarios](docs/test-scenarios/Product_Test_Scenarios.md)
- [Shopping Cart Test Scenarios](docs/test-scenarios/Cart_Test_Scenarios.md)
- [Checkout Test Scenarios](docs/test-scenarios/Checkout_Test_Scenarios.md)

### Test Cases

- [Login Test Cases](docs/test-cases/Login_Test_Cases.md)
- [Product Test Cases](docs/test-cases/Product_Test_Cases.md)
- [Shopping Cart Test Cases](docs/test-cases/Cart_Test_Cases.md)
- [Checkout Test Cases](docs/test-cases/Checkout_Test_Cases.md)

### Test Execution Results

- [Login Test Execution](docs/test-results/Login_Test_Execution.md)
- [Product Test Execution](docs/test-results/Product_Test_Execution.md)
- [Shopping Cart Test Execution](docs/test-results/Cart_Test_Execution.md)
- [Checkout Test Execution](docs/test-results/Checkout_Test_Execution.md)

### Checklists

- [Smoke Testing Checklist](docs/checklists/Smoke_Checklist.md)
- [Regression Testing Checklist](docs/checklists/Regression_Checklist.md)

### Exploratory Testing

- [Exploratory Testing Sessions](docs/exploratory-testing/Exploratory_Testing.md)

### Defect Reporting

- [Bug Reports](docs/bug-reports/Bug_Reports.md)

---

## Repository Structure

```text
qa-web-saucedemo/
│
├── README.md
│
└── docs/
    ├── Test_Plan.md
    ├── Test_Summary_Report.md
    │
    ├── test-scenarios/
    │   ├── Login_Test_Scenarios.md
    │   ├── Product_Test_Scenarios.md
    │   ├── Cart_Test_Scenarios.md
    │   └── Checkout_Test_Scenarios.md
    │
    ├── test-cases/
    │   ├── Login_Test_Cases.md
    │   ├── Product_Test_Cases.md
    │   ├── Cart_Test_Cases.md
    │   └── Checkout_Test_Cases.md
    │
    ├── test-results/
    │   ├── Login_Test_Execution.md
    │   ├── Product_Test_Execution.md
    │   ├── Cart_Test_Execution.md
    │   └── Checkout_Test_Execution.md
    │
    ├── checklists/
    │   ├── Smoke_Checklist.md
    │   └── Regression_Checklist.md
    │
    ├── exploratory-testing/
    │   └── Exploratory_Testing.md
    │
    ├── bug-reports/
    │   └── Bug_Reports.md
    │
    └── evidence/
        └── screenshots/
