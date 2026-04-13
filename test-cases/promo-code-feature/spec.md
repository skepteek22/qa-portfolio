# Project: E-commerce Promo Code Module
## Software Requirements Specification (SRS)

### 1. Introduction
This document outlines the functional requirements and business logic for the Promo Code module in the shopping cart. The goal is to provide users with a seamless way to apply discounts while ensuring all business constraints are met.

---

### 2. Functional Requirements

#### 2.1 Input Field
* **Placeholder:** Display "Enter code".
* **Character Limit:** Maximum length of **12 characters**.
* **Input Type:** Alphanumeric (letters and numbers).

#### 2.2 "Apply" Button
* **Initial State:** Disabled (Greyed out).
* **Behavior:** Automatically enabled as soon as the user enters at least **one (1) character**.

#### 2.3 Discount Logic
The system supports two types of discounts:
1. **Fixed Amount:** A flat deduction (e.g., $10.00).
2. **Percentage:** A percentage-based deduction (e.g., 10%).

#### 2.4 Business Rules & Constraints
* **Minimum Order Value (MOV):** The promo code can only be applied if the cart subtotal is **≥ $15.00**.
* **Expiration:** Codes must be checked against the current server date.
* **Usage Limit:** Restricted to **one-time use** per unique User ID.
* **Discount Cap:** To protect profit margins, the total discount cannot exceed **90%** of the order value. If the discount exceeds this limit, the final price is set to exactly 10% of the original subtotal.

---

### 3. Error Handling & Validation
The system must provide clear feedback for invalid inputs:

| Scenario | Error Message |
| :--- | :--- |
| Code not found in DB | "Promo code does not exist" |
| Current date > Expiry date | "Promo code has expired" |
| Cart total < $15.00 | "Minimum order value for this code is $15.00" |
| Code already used by user | "You have already used this promo code" |

---

### 4. UI/UX Requirements
* **Success State:** Upon successful application, the price must update instantly.
* **Confirmation:** Display a message: `"Discount [X] applied"`.
* **Cancellation:** A **"Remove" (X icon)** must appear next to the applied code to allow the user to revert the discount.

---
