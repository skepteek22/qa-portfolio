# Test Cases: Promo Code Module

This document contains test cases for validating the Promo Code functionality in the shopping cart.

| ID | Title | Pre-conditions | Test Steps | Expected Result |
| :--- | :--- | :--- | :--- | :--- |
| **TC-01** | Apply valid Fixed Amount promo code | Cart total is $20.00. Valid code "SAVE10" exists ($10 discount). | 1. Enter "SAVE10" in the input field.<br>2. Click "Apply". | Price updates to $10.00. Message "Discount $10.00 applied" and "Remove" (X) button appear. |
| **TC-02** | Apply promo code with cart total below MOV | Cart total is $10.00 (Minimum Order Value is $15.00). | 1. Enter a valid code "PROMO15".<br>2. Click "Apply". | Error message: "Minimum order value for this code is $15.00" is displayed. Price remains $10.00. |
| **TC-03** | Apply an expired promo code | Code "EXPIRED20" has an expiration date in the past. | 1. Enter "EXPIRED20".<br>2. Click "Apply". | Error message: "Promo code has expired" is displayed. |
| **TC-04** | Apply a non-existent promo code | Code "GHOST" does not exist in the database. | 1. Enter "GHOST".<br>2. Click "Apply". | Error message: "Promo code does not exist" is displayed. |
| **TC-05** | Re-apply a previously used promo code | User has already redeemed code "WELCOME" in a previous order. | 1. Enter "WELCOME".<br>2. Click "Apply". | Error message: "You have already used this promo code" is displayed. |
| **TC-06** | Verify Maximum Discount Cap (90%) | Cart total is $100.00. Code "BIGGIFT" gives $95.00 discount. | 1. Enter "BIGGIFT".<br>2. Click "Apply". | Final price is $10.00 (10% of total) because the discount cannot exceed 90% of the order value. |
| **TC-07** | Verify "Apply" button state and Input Limit | User is on the cart page. | 1. Observe "Apply" button when field is empty.<br>2. Enter 1 character.<br>3. Try to enter 13 characters. | 1. Button is Disabled.<br>2. Button becomes Enabled.<br>3. Field limits input to 12 characters max. |
