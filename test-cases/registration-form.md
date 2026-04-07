# Registration Form Test Cases

| ID | Summary | Step-by-Step Instruction | Expected Result |
| :-- | :--- | :--- | :--- |
| 1 | Registration with valid data | 1. Enter `testuser@example.com` in the Email field.<br>2. Enter `Password123!` in the Password field.<br>3. Click the "Sign Up" button. | Account created successfully; user redirected to the "Welcome" page or Dashboard. |
| 2 | Registration with empty fields | 1. Leave Email and Password fields blank.<br>2. Click the "Sign Up" button. | Error message displayed: "Fields are required." Registration is not processed. |
| 3 | Registration with invalid Email format | 1. Enter `invalid-email.com` (no @) in the Email field.<br>2. Enter a valid password.<br>3. Click the "Sign Up" button. | Error message displayed: "Please enter a valid email address." |
| 4 | Password length validation (Too short) | 1. Enter a valid Email.<br>2. Enter "123" in the Password field.<br>3. Click the "Sign Up" button. | Error message displayed: "Password must be at least 6 characters long." |
| 5 | Password masking check (Security) | 1. Enter any characters into the Password field.<br>2. Observe the input. | Password characters are hidden (replaced by dots or asterisks); plain text is not visible. |
