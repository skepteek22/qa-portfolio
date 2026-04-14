# 🐞 Bug Reports: Promo Code Module

This document outlines the defects discovered during the testing of the Promo Code functional module. Each bug is documented with clear steps to reproduce, actual vs. expected results, and severity.

---

### 🔴 [KAN-1] Promo code field accepts more than 12 characters in the Cart
**Status:** `IN PROGRESS` | **Severity:** `Medium` | **Priority:** `Medium`

#### **Description**
The system fails to enforce the 12-character limit on the promo code input field, allowing users to enter longer strings.

#### **Steps to Reproduce**
1. Navigate to the Shopping Cart page.
2. Locate the "Enter code" input field.
3. Type or paste a string longer than 12 characters (e.g., `PROMOCODE2026_EXTRA`).
4. Observe the input field.

#### **Actual Result**
The field accepts all characters (19 characters in the example).

#### **Expected Result**
The field should restrict input to a maximum of 12 characters. User should not be able to type more than the limit.

---

### 🟡 [KAN-2] "Apply" button remains disabled after entering valid characters
**Status:** `TO DO` | **Severity:** `High` | **Priority:** `High`

#### **Description**
The "Apply" button does not change its state to "Enabled" even when the user provides input, preventing the discount from being processed.

#### **Steps to Reproduce**
1. Open the Shopping Cart.
2. Enter a valid character (e.g., "A") into the promo code field.
3. Observe the "Apply" button state.

#### **Actual Result**
The "Apply" button remains greyed out and unclickable.

#### **Expected Result**
The "Apply" button must become active/enabled immediately after at least one (1) character is entered into the field.

---

## 🛠 Project Board Status
| Task ID | Summary | Status |
| :--- | :--- | :--- |
| KAN-1 | Character limit bypass | 🚧 In Progress |
| KAN-2 | Button activation failure | 📝 To Do |
| TC-07 | Verify Button state and Input Limit | ✅ Done |




<img width="1478" height="240" alt="image" src="https://github.com/user-attachments/assets/66ec352b-305f-42ec-9657-2d04ceddfb20" />


---
