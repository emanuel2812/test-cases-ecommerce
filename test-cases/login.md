# Test Cases - Login

## TC001 - Login with valid credentials

**Objective:**
Validate whether the user can access their account using a valid email address and password.

**Precondition:**
The user must have a registered account.

**Steps:**

1. Access the login page.
2. Enter a valid email address.
3. Enter a valid password.
4. Click the "Login" button.

**Expected Result:**
The system should authenticate the user and redirect them to their account's home page.

---

## TC002 - Login with invalid password

**Objective:**
Validate the system behavior when an incorrect password is entered.

**Precondition:**
The user must have a registered account.

**Steps:**

1. Access the login page.
2. Enter a valid email address.
3. Enter an incorrect password.
4. Click the "Login" button.

**Expected Result:**
The system should deny access and display a message informing the user that the credentials are invalid.

---

## TC003 - Login with empty fields

**Objective:**
Validate whether the system prevents login when required fields are left empty.

**Steps:**

1. Access the login page.
2. Leave the email field empty.
3. Leave the password field empty.
4. Click the "Login" button.

**Expected Result:**
The system should inform the user that the required fields must be filled in and should not perform the login.
