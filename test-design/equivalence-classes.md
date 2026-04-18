## 🧪 Practical Task: Equivalence Partitioning & Boundary Value Analysis

**Task:** Test a "Age" input field that accepts integers from **1 to 120**.

### 1. Logical Classes
* **Valid Class:** [1...120] — system should accept these values.
* **Invalid Class (Low):** < 1 — system should reject (e.g., 0, -5).
* **Invalid Class (High):** > 120 — system should reject (e.g., 121, 150).

### 2. Test Cases Table

| TC ID | Summary | Input Value | Expected Result | Testing Technique |
| :--- | :--- | :--- | :--- | :--- |
| **TC-01** | Valid minimum boundary value | `1` | Value accepted | Boundary Value Analysis |
| **TC-02** | Valid maximum boundary value | `120` | Value accepted | Boundary Value Analysis |
| **TC-03** | Valid middle value | `45` | Value accepted | Equivalence Partitioning |
| **TC-04** | Invalid value below minimum | `0` | Error: "Age must be at least 1" | Boundary Value Analysis |
| **TC-05** | Invalid value above maximum | `121` | Error: "Age cannot exceed 120" | Boundary Value Analysis |
| **TC-06** | Invalid negative value | `-5` | Error: "Invalid input" | Equivalence Partitioning |

---
