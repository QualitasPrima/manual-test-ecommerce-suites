# Test Case Checklist for DemoQA Automation Practice Form

This checklist covers the key test scenarios to validate the form at https://demoqa.com/automation-practice-form.

Test cases are prioritized as High, Medium, Low based on impact and likelihood.

---

## 1. Personal Information Section

| Priority | Test Case Description                                          | Test Type          |
|----------|---------------------------------------------------------------|--------------------|
| High     | Submit form with all valid required fields filled correctly.  | Positive           |
| High     | Submit form leaving required fields empty (First Name, Last Name, Email). | Negative           |
| Medium   | Enter invalid email formats (missing '@', missing domain).    | Negative           |
| Medium   | Enter numeric/special characters in name fields.              | Negative           |
| Medium   | Enter boundary length values for First and Last Name fields.  | Edge / Boundary    |

---

## 2. Gender Selection

| Priority | Test Case Description                                  | Test Type       |
|----------|-------------------------------------------------------|-----------------|
| High     | Select each gender option individually and submit.   | Positive        |
| High     | Submit form without selecting gender.                 | Negative        |

---

## 3. Mobile Number

| Priority | Test Case Description                                  | Test Type       |
|----------|-------------------------------------------------------|-----------------|
| High     | Enter valid 10-digit mobile number and submit.        | Positive        |
| High     | Enter mobile number with less than or more than 10 digits. | Negative   |
| Medium   | Enter alphabetic or special characters in mobile field.| Negative       |
| Medium   | Boundary test: 10 digits, 9 digits, 11 digits.         | Edge / Boundary |

---

## 4. Date of Birth

| Priority | Test Case Description                                  | Test Type       |
|----------|-------------------------------------------------------|-----------------|
| Medium   | Select a valid date from date picker and submit.      | Positive        |
| Medium   | Enter invalid date manually if allowed or empty field. | Negative       |

---

## 5. Subjects Input

| Priority | Test Case Description                                  | Test Type       |
|----------|-------------------------------------------------------|-----------------|
| Medium   | Enter valid subject(s) and submit.                     | Positive        |
| Medium   | Enter invalid or unsupported subjects.                 | Negative        |

---

## 6. Hobbies Checkbox

| Priority | Test Case Description                                  | Test Type       |
|----------|-------------------------------------------------------|-----------------|
| High     | Select single hobby and submit.                        | Positive        |
| High     | Select multiple hobbies and submit.                    | Positive        |
| High     | Select multiple hobbies and observe form submission error (known bug). | Negative   |
| Low      | Submit without selecting any hobby.                    | Positive        |

---

## 7. Picture Upload

| Priority | Test Case Description                                  | Test Type       |
|----------|-------------------------------------------------------|-----------------|
| Medium   | Upload valid image file and submit.                    | Positive        |
| Medium   | Attempt to upload invalid file types (e.g., .txt).     | Negative        |
| Medium   | Upload large file and observe form behavior.           | Edge / Boundary |

---

## 8. Current Address

| Priority | Test Case Description                                  | Test Type       |
|----------|-------------------------------------------------------|-----------------|
| High     | Enter valid address text and submit.                   | Positive        |
| Medium   | Leave empty and submit.                                | Negative        |

---

## 9. State and City Dropdowns

| Priority | Test Case Description                                  | Test Type       |
|----------|-------------------------------------------------------|-----------------|
| High     | Select valid State and City and submit.                | Positive        |
| High     | Try submitting without selecting State and City.       | Negative        |

---

## Notes:

- Positive tests assume valid input data that meets field requirements.  
- Negative tests involve invalid, empty, or malformed inputs.  
- Boundary tests focus on minimum and maximum input lengths or limits.  
- Known bug: Multi-hobby selection prevents form submission (see bug report).

---
