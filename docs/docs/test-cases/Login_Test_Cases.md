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
