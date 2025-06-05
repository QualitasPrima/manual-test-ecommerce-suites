# Test Case: TC_UAM_001 - Create Account - Positive Scenario

**Module:** User Account Management
**Feature:** Create Account
**Objective:** Verify that a new user can successfully create an account with valid credentials.
**Priority:** Critical

**Preconditions:**
1.  User is not logged in.
2.  User has a unique, valid email address not already registered.
3.  User has chosen a password meeting the site's complexity requirements.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|
| 1      | Navigate to the Luma homepage.                                                        | URL: `https://magento.softwaretestingboard.com/` | Luma homepage loads successfully.                                                                                                             |
| 2      | Click on the "Create an Account" link in the header.                                  | -                                             | User is redirected to the "Create New Customer Account" page.                                                                                 |
| 3      | Enter valid data in the "First Name" field.                                           | First Name: `Test`                            | "Test" is entered into the First Name field.                                                                                                  |
| 4      | Enter valid data in the "Last Name" field.                                            | Last Name: `User`                             | "User" is entered into the Last Name field.                                                                                                   |
| 5      | Enter a unique, valid email address in the "Email" field.                             | Email: `testuser[random_number]@example.com`   | Email address is entered into the Email field.                                                                                                |
| 6      | Enter a strong password in the "Password" field.                                      | Password: `Password123!`                      | Password is entered and masked in the Password field.                                                                                         |
| 7      | Re-enter the same password in the "Confirm Password" field.                           | Confirm Password: `Password123!`                | Password is entered and masked in the Confirm Password field.                                                                               |
| 8      | Click the "Create an Account" button.                                                 | -                                             | 1. User is redirected to the "My Dashboard" page. <br> 2. Success message "Thank you for registering..." is displayed. <br> 3. User is logged in. |

---
**Actual Result:** (To be filled during execution)
**Status:** (Pass/Fail/Blocked)
**Notes:**
