# Test Cases - Registration

## TC001 - Registration with valid data

**Objective:**
Validate whether a new user can successfully create an account using valid information.

**Precondition:**
The user must not have an account registered with the email address being used.

**Steps:**

1. Access the registration page.
2. Enter a valid first name.
3. Enter a valid last name.
4. Enter a valid email address.
5. Enter a valid password.
6. Confirm the password.
7. Click the "Create Account" button.

**Expected Result:**
The system should successfully create the account and display a confirmation message.

---

## TC002 - Registration with invalid email

**Objective:**
Validate whether the system prevents registration with an invalid email address.

**Steps:**

1. Access the registration page.
2. Enter a valid first name.
3. Enter a valid last name.
4. Enter an invalid email address.
5. Enter a valid password.
6. Confirm the password.
7. Click the "Create Account" button.

**Expected Result:**
The system should reject the registration and display a message informing the user that the email address is invalid.

---

## TC003 - Registration with an already registered email

**Objective:**
Validate whether the system prevents registration using an email address that is already registered.

**Precondition:**
The email address must already be registered in the system.

**Steps:**

1. Access the registration page.
2. Enter a valid first name.
3. Enter a valid last name.
4. Enter an email address that is already registered.
5. Enter a valid password.
6. Confirm the password.
7. Click the "Create Account" button.

**Expected Result:**
The system should prevent the registration and inform the user that the email address is already registered.

---

## TC004 - Registration with empty required fields

**Objective:**
Validate whether the system prevents registration when required fields are empty.

**Steps:**

1. Access the registration page.
2. Leave the required fields empty.
3. Click the "Create Account" button.

**Expected Result:**
The system should display validation messages for the required fields and should not create the account.

---

## TC005 - Registration with an invalid password

**Objective:**
Validate whether the system prevents registration when the password does not meet the security requirements.

**Steps:**

1. Access the registration page.
2. Enter valid personal information.
3. Enter a password that does not meet the minimum security requirements.
4. Confirm the password.
5. Click the "Create Account" button.

**Expected Result:**
The system should reject the password and display a message explaining the password requirements.
