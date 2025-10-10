# 🧪 GitHub Login & Dashboard – QA Manual Testing Project 
## 📋 Project Overview

This project is a dummy Quality Assurance (QA) testing project focused on functional testing of the login, dashboard, and user profile features on GitHub.

The main objective of this project is to document the manual testing process and ensure that the core features work as expected through both positive and negative test cases.

It also serves as a professional simulation to demonstrate skills in test case design, analysis, test execution, and test documentation.


## 🧰 Tools & Technologies
- Browser: Google Chrome
- Platform: [GitHub Login Page](https://github.com/login)
- Testing Type: Manual Testing
- Testing Tools: Excel/Google Sheet (for test case documentation)
- Testing Techniques: Functional Testing, Positive & Negative Testing


## 🧩 Test Modules

This project covers three main modules:

1. Login Module
- Verify the presence of username and password input fields, and the login button
- Test scenarios with empty username or password fields

2. Dashboard Module
- Verify main elements on the dashboard page
- Navigate to other pages from the dashboard
- Test unauthorized access to the dashboard (without login)
- Test the logout functionality

3. Profile Module
- Update full name with valid data
- Attempt to save an empty name field
- Update profile picture

## 🧾 Test Summary

| No | Test Case ID | Test Scenario                    | Type     | Expected Result                                    | Actual Result    | Status    | Notes                          |
| -- | ------------ | -------------------------------- | -------- | -------------------------------------------------- | ---------------- | --------- | ------------------------------ |
| 1  | TC01         | Verify login form display        | Positive | Username box & login button appear                 | AsExpected       | ✅ Passed  | -                              |
| 2  | TC02         | Login with valid credentials     | Positive | Successfully logged in and redirected to dashboard | AsExpected       | ✅ Passed  | -                              |
| 3  | TC03         | Login with wrong password        | Negative | Login fails                                        | AsExpected       | ✅ Passed  | -                              |
| 4  | TC04         | Login with unregistered username | Negative | Login fails                                        | AsExpected       | ✅ Passed  | -                              |
| 5  | TC05         | Login with empty username        | Negative | Login fails                                        | AsExpected       | ✅ Passed  | -                              |
| 6  | TC06         | Login with empty password        | Negative | Login fails                                        | AsExpected       | ✅ Passed  | -                              |
| 7  | TC07         | Verify dashboard elements        | Positive | Dashboard page displayed                           | AsExpected       | ✅ Passed  | -                              |
| 8  | TC08         | Navigate to another page         | Positive | Project page displayed                             | AsExpected       | ✅ Passed  | -                              |
| 9  | TC09         | Access dashboard without login   | Negative | Access denied                                      | AsExpected       | ✅ Passed  | -                              |
| 10 | TC10         | Logout                           | Positive | Redirected to login page                           | AsExpected       | ✅ Passed  | -                              |
| 11 | TC11         | Update full name with valid data | Positive | Full name updated                                  | AsExpected       | ✅ Passed  | -                              |
| 12 | TC12         | Try saving empty name field      | Negative | Name not updated                                   | AsExpected       | ✅ Passed  | -                              |
| 13 | TC13         | Update profile picture           | Positive | Profile picture updated                            | ❌ Not AsExpected | ⚠️ Failed | Delay ±3 minutes before update |


## 📆 Execution Details

Date of Execution: 7 October 2025
Executed by: Chesya Ivana Sitorus
Testing Status: 12 Test Cases Passed, 1 Failed (TC13 – Profile Picture Delay)


## 🧠 Key Findings

1. Login functionality works correctly across all test scenarios.
2. Input validation functions properly for empty fields.
3. Navigation and logout features perform as expected.
4. One issue found: profile picture updates take approximately 3 minutes to appear after upload.