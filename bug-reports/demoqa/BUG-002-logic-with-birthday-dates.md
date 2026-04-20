# [BUG-002] Logic: User can select a future date of birth in Practice Form

**Status:** 🔴 Open  
**Severity:** S2/S3 (Major)  
**Priority:** P2 (Medium)  
**Project:** DemoQA  

---

## 📝 Description
The "Date of Birth" input field in the Practice Form does not have restrictive validation. It allows users to select and successfully submit a date that is later than the current system date (e.g., year 2026). This violates the business logic of personal data entry.

## 💻 Environment
- **URL:** [https://demoqa.com/automation-practice-form](https://demoqa.com/automation-practice-form)
- **Browser:** Chrome v120.0+ (Desktop)
- **Current Date (System Time):** April 20, 2026

## 🐾 Steps to Reproduce
1. Navigate to the **Practice Form** page.
2. Click on the **"Date of Birth"** input field to trigger the calendar picker.
3. Use the navigation arrows or dropdowns to select a **future year/month** (e.g., August 2026).
4. Select any day (e.g., 25).
5. Fill in all other required fields with valid data.
6. Click the **"Submit"** button.

## ❌ Actual Result
The system accepts the future date without any warning. After clicking "Submit", the confirmation modal displays the invalid date (e.g., `25 Aug 2026`).

## ✅ Expected Result
The calendar picker should prevent the selection of any dates beyond the current date (future dates should be disabled/grayed out). If entered manually, the system should return a validation error: *"Date of birth cannot be in the future"*.

---

### 💡 Rationale
* **Severity S2:** 
* **Priority P2:** 
