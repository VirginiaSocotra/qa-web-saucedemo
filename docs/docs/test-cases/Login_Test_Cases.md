# Login Test Cases

## TC-LOGIN-001 — Login with valid credentials

**Related Scenario:** LS-01  
**Priority:** High  
**Type:** Functional / Positive

### Preconditions
- User is on the SauceDemo Login page.
- User account is active.

### Test Data
- Username: standard_user
- Password: secret_sauce

### Steps
1. Enter `standard_user` into the Username field.
2. Enter `secret_sauce` into the Password field.
3. Click the Login button.

### Expected Result
- User is successfully authenticated.
- User is redirected to the Products page.
- Product catalog is displayed.


## TC-LOGIN-002 — Login with valid username and invalid password

**Related Scenario:** LS-02  
**Priority:** High  
**Type:** Functional / Negative

### Preconditions
- User is on the SauceDemo Login page.

### Test Data
- Username: standard_user
- Password: wrong_password

### Steps
1. Enter `standard_user` into the Username field.
2. Enter `wrong_password` into the Password field.
3. Click the Login button.

### Expected Result
- Login is rejected.
- User remains on the Login page.
- An authentication error message is displayed.


## TC-LOGIN-003 — Login with invalid username and valid password

**Related Scenario:** LS-03  
**Priority:** High  
**Type:** Functional / Negative

### Preconditions
- User is on the SauceDemo Login page.

### Test Data
- Username: invalid_user
- Password: secret_sauce

### Steps
1. Enter `invalid_user` into the Username field.
2. Enter `secret_sauce` into the Password field.
3. Click the Login button.

### Expected Result
- Login is rejected.
- User remains on the Login page.
- An authentication error message is displayed.


## TC-LOGIN-004 — Login with empty username

**Related Scenario:** LS-05  
**Priority:** High  
**Type:** Validation / Negative

### Preconditions
- User is on the SauceDemo Login page.

### Test Data
- Username: empty
- Password: secret_sauce

### Steps
1. Leave the Username field empty.
2. Enter `secret_sauce` into the Password field.
3. Click the Login button.

### Expected Result
- Login is rejected.
- A validation message for the required username is displayed.


## TC-LOGIN-005 — Login with empty password

**Related Scenario:** LS-06  
**Priority:** High  
**Type:** Validation / Negative

### Preconditions
- User is on the SauceDemo Login page.

### Test Data
- Username: standard_user
- Password: empty

### Steps
1. Enter `standard_user` into the Username field.
2. Leave the Password field empty.
3. Click the Login button.

### Expected Result
- Login is rejected.
- A validation message for the required password is displayed.

  ## TC-LOGIN-006 — Login with empty username and empty password

**Related Scenario:** LS-07  
**Priority:** High  
**Type:** Validation / Negative

### Preconditions
- User is on the SauceDemo Login page.

### Test Data
- Username: empty
- Password: empty

### Steps
1. Leave the Username field empty.
2. Leave the Password field empty.
3. Click the Login button.

### Expected Result
- Login is rejected.
- User remains on the Login page.
- A validation message for the required username is displayed.


## TC-LOGIN-007 — Login with locked-out user

**Related Scenario:** LS-08  
**Priority:** High  
**Type:** Functional / Negative

### Preconditions
- User is on the SauceDemo Login page.
- The test account is locked.

### Test Data
- Username: locked_out_user
- Password: secret_sauce

### Steps
1. Enter `locked_out_user` into the Username field.
2. Enter `secret_sauce` into the Password field.
3. Click the Login button.

### Expected Result
- Login is rejected.
- User remains on the Login page.
- An error message indicating that the user is locked out is displayed.


## TC-LOGIN-008 — Login with uppercase username

**Related Scenario:** LS-09  
**Priority:** Medium  
**Type:** Functional / Negative

### Preconditions
- User is on the SauceDemo Login page.

### Test Data
- Username: STANDARD_USER
- Password: secret_sauce

### Steps
1. Enter `STANDARD_USER` into the Username field.
2. Enter `secret_sauce` into the Password field.
3. Click the Login button.

### Expected Result
- Login is rejected.
- User remains on the Login page.
- An authentication error message is displayed.


## TC-LOGIN-009 — Logout after successful authentication

**Related Scenario:** LS-10  
**Priority:** High  
**Type:** Functional / Positive

### Preconditions
- User is on the SauceDemo Login page.
- User account is active.

### Test Data
- Username: standard_user
- Password: secret_sauce

### Steps
1. Enter `standard_user` into the Username field.
2. Enter `secret_sauce` into the Password field.
3. Click the Login button.
4. Verify that the Products page is displayed.
5. Open the navigation menu.
6. Click the Logout option.

### Expected Result
- User is successfully logged out.
- User is redirected to the Login page.
- Authenticated content is no longer displayed.


## TC-LOGIN-010 — Login with uppercase password

**Related Scenario:** LS-11  
**Priority:** Medium  
**Type:** Functional / Negative

### Preconditions
- User is on the SauceDemo Login page.

### Test Data
- Username: standard_user
- Password: SECRET_SAUCE

### Steps
1. Enter `standard_user` into the Username field.
2. Enter `SECRET_SAUCE` into the Password field.
3. Click the Login button.

### Expected Result
- Login is rejected.
- User remains on the Login page.
- An authentication error message is displayed.
