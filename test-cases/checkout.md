# Test Cases - Checkout

## TC001 - Checkout with a valid product

**Objective:**
Validate whether the user can successfully complete a purchase with a valid product.

**Precondition:**
The user must be logged in and have at least one available product in the shopping cart.

**Steps:**

1. Access the shopping cart.
2. Verify that the selected product is displayed.
3. Click the "Checkout" button.
4. Enter valid shipping information.
5. Select a valid payment method.
6. Review the order information.
7. Click the "Place Order" button.

**Expected Result:**
The system should successfully process the order and display an order confirmation message.

---

## TC002 - Change product quantity

**Objective:**
Validate whether the user can change the quantity of a product in the shopping cart.

**Precondition:**
The user must have a product in the shopping cart.

**Steps:**

1. Access the shopping cart.
2. Change the product quantity.
3. Verify the updated quantity.
4. Verify the order total.

**Expected Result:**
The system should update the product quantity and recalculate the order total correctly.

---

## TC003 - Remove product from cart

**Objective:**
Validate whether the user can remove a product from the shopping cart.

**Precondition:**
The shopping cart must contain at least one product.

**Steps:**

1. Access the shopping cart.
2. Select a product.
3. Click the "Remove" button.

**Expected Result:**
The selected product should be removed from the shopping cart and the order total should be updated.

---

## TC004 - Checkout with incomplete shipping information

**Objective:**
Validate whether the system prevents checkout when required shipping information is missing.

**Steps:**

1. Access the shopping cart.
2. Click the "Checkout" button.
3. Leave one or more required shipping fields empty.
4. Select a payment method.
5. Click the "Place Order" button.

**Expected Result:**
The system should display validation messages for the required shipping fields and should not complete the order.

---

## TC005 - Checkout with invalid payment information

**Objective:**
Validate whether the system prevents an order from being completed with invalid payment information.

**Precondition:**
The user must have a product in the shopping cart.

**Steps:**

1. Access the shopping cart.
2. Click the "Checkout" button.
3. Enter valid shipping information.
4. Enter invalid payment information.
5. Click the "Place Order" button.

**Expected Result:**
The system should reject the payment and display an appropriate error message. The order should not be completed.
