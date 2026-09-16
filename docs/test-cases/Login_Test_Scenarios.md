# Login Test Scenarios

## Feature
User Authentication

## Objective
Verify that users can log in with valid credentials and that the application correctly handles invalid or restricted login attempts.

## Positive Scenarios

1. Login with valid username and valid password.
2. Logout after successful authentication.

## Negative Scenarios

3. Login with valid username and invalid password.
4. Login with invalid username and valid password.
5. Login with invalid username and invalid password.
6. Login with empty username.
7. Login with empty password.
8. Login with both username and password empty.
9. Login using a locked-out user.

## Input Validation Scenarios

10. Verify username case sensitivity.
11. Verify password case sensitivity.
12. Verify username field behavior with leading spaces.
13. Verify username field behavior with trailing spaces.
14. Verify password field behavior with leading spaces.
15. Verify password field behavior with trailing spaces.

## UI Scenarios

16. Verify username field is visible.
17. Verify password field is visible.
18. Verify Login button is visible and enabled.
19. Verify password characters are masked.
20. Verify error message is displayed after unsuccessful login.

| ID | Scenario | Expected Result | Actual Result | Status |
|---|---|---|---|---|
| LS-01 | Valid username + valid password | User is successfully logged in and redirected to the Products page | User is redirected to the Products page | Pass |
| LS-02 | Valid username + invalid password | Login is rejected and an authentication error message is displayed | Login is rejected. Error message is displayed: "Epic sadface: Username and password do not match any user in this service" | Pass |
| LS-03 | Invalid username + valid password | Login is rejected and an authentication error message is displayed | Login is rejected. Error message is displayed: "Epic sadface: Username and password do not match any user in this service" | Pass |
| LS-04 | Invalid username + invalid password | Login is rejected and an authentication error message is displayed | Login is rejected. Error message is displayed: "Epic sadface: Username and password do not match any user in this service" | Pass |
| LS-05 | Empty username + valid password | Login is rejected and username validation message is displayed | Error message is displayed: "Epic sadface: Username is required" | Pass |
| LS-06 | Valid username + empty password | Login is rejected and password validation message is displayed | Error message is displayed: "Epic sadface: Password is required" | Pass |
| LS-07 | Empty username + empty password | Login is rejected and validation message is displayed | Error message is displayed: "Epic sadface: Username is required" | Pass |
| LS-08 | Locked user + valid password | Login is rejected and locked-user message is displayed | Error message is displayed: "Epic sadface: Sorry, this user has been locked out." | Pass |
| LS-09 | Uppercase username + valid password | Behavior to be explored because username case-sensitivity is not specified | Login is rejected and authentication error message is displayed | N/A |
| LS-10 | Login with valid credentials and log out | User can log in and then successfully log out | User is successfully logged in. After Logout, user is redirected to the Login page | Pass |
