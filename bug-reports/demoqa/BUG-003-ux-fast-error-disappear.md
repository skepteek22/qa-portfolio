# [BUG-003] UI/UX: Registration error message disappears too quickly

**Status:** 🔴 Open  
**Severity:** S4 (Minor)  
**Priority:** P3 (Low)  
**Project:** DemoQA  

---

## 📝 Description
During the registration process in the Book Store Application, if a user provides invalid data (e.g., a weak password), an error message appears at the bottom of the form. However, this message disappears in less than a second, preventing the user from reading and understanding the feedback.

## 💻 Environment
- **URL:** [https://demoqa.com/register](https://demoqa.com/register)
- **Browser:** Tested on Chrome & Firefox (Latest)
- **Device:** Desktop

## 🐾 Steps to Reproduce
1. Open the **Book Store Application** -> **Register** page.
2. Fill in the "First Name", "Last Name", and "Username" fields with valid data.
3. Enter a short/invalid password (e.g., `123`).
4. Click the **"Register"** button.
5. Watch the red error message that appears at the bottom of the form.

## ❌ Actual Result
The error message appears but disappears almost instantly (approx. 500ms–800ms). The user does not have enough time to identify the specific input error.

## ✅ Expected Result
The error message should remain visible for a sufficient amount of time (at least 5–7 seconds) or until the user starts interacting with the form again, ensuring the "Visibility of System Status" principle is met.

---

### 💡 Rationale
* **Severity S4:**
* **Priority P3:**
