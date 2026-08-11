# 🐞 Bug Reports

This section contains sample bug reports created based on test scenarios for an e-commerce application.

---

## BUG-001 - Login accepts an incorrect password

**Severity:** High
**Priority:** High
**Module:** Login
**Environment:** Web Application - Chrome - Windows 11

### Preconditions

The user must have a registered account.

### Steps to Reproduce

1. Access the login page.
2. Enter a valid registered email address.
3. Enter an incorrect password.
4. Click the **"Login"** button.

### Expected Result

The system should deny access and display a message informing the user that the credentials are invalid.

### Actual Result

The system allows the user to log in even though an incorrect password was entered.

### Status

**Open**

### Impact

This issue may allow unauthorized users to access registered accounts, creating a security risk.

---

## BUG-002 - Login is performed with empty required fields

**Severity:** High
**Priority:** High
**Module:** Login
**Environment:** Web Application - Chrome - Windows 11

### Steps to Reproduce

1. Access the login page.
2. Leave the email field empty.
3. Leave the password field empty.
4. Click the **"Login"** button.

### Expected Result

The system should prevent the login attempt and display validation messages informing the user that the required fields must be filled in.

### Actual Result

The system performs the login attempt without properly validating the required fields.

### Status

**Open**

### Impact

The lack of required-field validation may allow unexpected behavior in the login process.

---

## BUG-003 - Registration accepts an invalid email address

**Severity:** High
**Priority:** High
**Module:** Registration
**Environment:** Web Application - Chrome - Windows 11

### Steps to Reproduce

1. Access the registration page.
2. Enter a valid first name.
3. Enter a valid last name.
4. Enter an invalid email address.
5. Enter a valid password.
6. Confirm the password.
7. Click the **"Create Account"** button.

### Expected Result

The system should reject the registration and display a message informing the user that the email address is invalid.

### Actual Result

The system accepts the invalid email address and successfully creates the account.

### Status

**Open**

### Impact

Users may create accounts with invalid email addresses, affecting account verification, password recovery, and communication.

---

## BUG-004 - Registration allows duplicate email addresses

**Severity:** High
**Priority:** High
**Module:** Registration
**Environment:** Web Application - Chrome - Windows 11

### Preconditions

The email address must already be registered in the system.

### Steps to Reproduce

1. Access the registration page.
2. Enter a valid first name.
3. Enter a valid last name.
4. Enter an email address that is already registered.
5. Enter a valid password.
6. Confirm the password.
7. Click the **"Create Account"** button.

### Expected Result

The system should prevent the registration and inform the user that the email address is already registered.

### Actual Result

The system allows the user to create another account using the same email address.

### Status

**Open**

### Impact

Duplicate accounts can cause data inconsistencies and problems with authentication, order history, and account recovery.

---

## BUG-005 - Registration accepts a weak password

**Severity:** High
**Priority:** High
**Module:** Registration
**Environment:** Web Application - Chrome - Windows 11

### Steps to Reproduce

1. Access the registration page.
2. Enter valid personal information.
3. Enter a password that does not meet the minimum security requirements.
4. Confirm the password.
5. Click the **"Create Account"** button.

### Expected Result

The system should reject the password and display a message explaining the password requirements.

### Actual Result

The system accepts the weak password and successfully creates the account.

### Status

**Open**

### Impact

Weak passwords may reduce account security and increase the risk of unauthorized access.

---

## BUG-006 - Order total is not recalculated after changing quantity

**Severity:** High
**Priority:** High
**Module:** Shopping Cart / Checkout
**Environment:** Web Application - Chrome - Windows 11

### Steps to Reproduce

1. Access the shopping cart.
2. Change the quantity of the product.
3. Verify the updated quantity.
4. Check the order total.

### Expected Result

The system should update the product quantity and recalculate the order total correctly.

### Actual Result

The product quantity is updated, but the order total remains unchanged.

### Status

**Open**

### Impact

Incorrect order totals can result in customers being charged the wrong amount.

---

## BUG-007 - Removed product remains in the shopping cart

**Severity:** High
**Priority:** High
**Module:** Shopping Cart
**Environment:** Web Application - Chrome - Windows 11

### Steps to Reproduce

1. Access the shopping cart.
2. Select a product.
3. Click the **"Remove"** button.
4. Check the shopping cart.

### Expected Result

The selected product should be removed from the shopping cart and the order total should be updated.

### Actual Result

The product remains displayed in the shopping cart and the order total is not updated.

### Status

**Open**

### Impact

Users may accidentally purchase products they intended to remove.

---

## BUG-008 - Checkout allows order placement with incomplete shipping information

**Severity:** Critical
**Priority:** High
**Module:** Checkout
**Environment:** Web Application - Chrome - Windows 11

### Steps to Reproduce

1. Access the shopping cart.
2. Click the **"Checkout"** button.
3. Leave one or more required shipping fields empty.
4. Select a payment method.
5. Click the **"Place Order"** button.

### Expected Result

The system should display validation messages for the required shipping fields and should not complete the order.

### Actual Result

The system completes the order even though required shipping information is missing.

### Status

**Open**

### Impact

Orders may be created without sufficient information for delivery, potentially resulting in failed shipments and customer complaints.

---

## BUG-009 - Checkout accepts invalid payment information

**Severity:** Critical
**Priority:** Critical
**Module:** Checkout / Payment
**Environment:** Web Application - Chrome - Windows 11

### Steps to Reproduce

1. Access the shopping cart.
2. Click the **"Checkout"** button.
3. Enter valid shipping information.
4. Enter invalid payment information.
5. Click the **"Place Order"** button.
6. Check the order status.

### Expected Result

The system should reject the payment and display an appropriate error message. The order should not be completed.

### Actual Result

The system accepts the invalid payment information and completes the order.

### Status

**Open**

### Impact

This is a critical payment-related issue because orders may be created without a valid payment transaction.
