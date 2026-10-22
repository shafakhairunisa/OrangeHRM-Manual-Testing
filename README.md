# OrangeHRM-Manual-Testing

## 🔎 Project Overview

This repository contains my personal manual testing project on the [OrangeHRM open-source demo](https://opensource-demo.orangehrmlive.com/web/index.php/auth/login), a web-based Human Resource Management system. The project focuses on validating four core modules: **Login, Employee Management (PIM), Leave, and Attendance (Time)**.

## 🎯 Objectives

- Validate that core HR workflows behave as expected.
- Cover positive, negative, and edge-case scenarios for each module.
- Compare expected and actual results to find defects and inconsistencies.
- Practice writing clear, traceable test documentation.

## 🛠️ Tools & Environment

| Item | Detail |
|---|---|
| Test management | Google Sheets / Excel |
| Browser | Google Chrome 155 |
| OS | Windows 11 |
| Application under test | OrangeHRM 5 demo (`opensource-demo.orangehrmlive.com`) |
| Test credentials | Public demo account shown on the login page |

## 📦 Scope

| Module | Areas Covered | Test Cases |
|---|---|---|
| Login | Valid/invalid credentials, required fields, SQL injection & XSS input, session/logout, forgot password | 24 |
| Employee Management (PIM) | Add/edit/delete employee, login details, photo upload, field limits, search & filters | 30 |
| Leave | Entitlements, apply leave, date validation, balance & overlap rules, approve/reject/cancel | 25 |
| Attendance | Punch in/out, time validation, overlapping records, employee records, summary report | 18 |
| **Total** | | **97** |

Scenario mix: 32 Positive, 41 Negative, 24 Edge.

## 🧪 Testing Techniques Applied

1. **Functional testing**: verifying forms, buttons, menus, and workflows against expected behavior.
2. **Negative testing**: invalid, empty, and malicious input (e.g. SQL injection, script tags).
3. **Boundary value analysis**: field length limits (e.g. 30/31 characters), comment limits, decimal precision.
4. **Edge-case testing**: overlapping records, weekend-only leave, midnight punch records, expired sessions.

## 🔄 STLC Implementation

- **Requirement analysis**: explored each module to understand the expected behavior.
- **Test planning**: defined scope, modules, and test environment.
- **Test case design**: wrote test cases with ID, type, priority, preconditions, steps, test data, and expected result.
- **Test execution**: ran the test cases manually and recorded actual results and status. *(Executed on: [date])*
- **Defect reporting**: documented failures with steps to reproduce and screenshots.
- **Test closure**: summarized results in the Summary sheet.

## 📊 Test Execution Summary

| Module | Total | Pass | Fail | Blocked |
|---|---|---|---|---|
| Login | 24 | [ ] | [ ] | [ ] |
| Employee Management | 30 | [ ] | [ ] | [ ] |
| Leave | 25 | [ ] | [ ] | [ ] |
| Attendance | 18 | [ ] | [ ] | [ ] |
| **Total** | **97** | **[ ]** | **[ ]** | **[ ]** |

**Key findings:** No critical defects found" only if that is what you actually observed.

## 📁 Deliverables

- 📄 [Test Cases (Google Sheets)](https://docs.google.com/spreadsheets/d/1y6Sy11EQegOzKEaIVkKb6yN57vwsF7XDKYNThrzykOA/edit?usp=sharing)
- 📄 `OrangeHRM_Test_Cases.xlsx` (Excel copy, in this repository)
- 🐞 Bug reports and screenshots: `/screenshots` *(add if available)*

### Test case columns

`TC ID` · `Type` · `Priority` · `Scenario` · `Preconditions` · `Test Steps` · `Test Data` · `Expected Result` · `Actual Result` · `Status` · `Remarks`

## ⚠️ Notes & Limitations

- The OrangeHRM demo is a shared public site and resets periodically, so data may change between sessions.
- Some expected results depend on system configuration (e.g. attendance rules, date format) and were verified during execution.

## 💭 Conclusion

This project helped me practice designing structured test cases and thinking beyond the happy path, especially around validation rules, boundaries, and data conflicts in an HR system.

---

**Author:** Shafa Khairunisa Salsabila · [GitHub](https://github.com/shafakhairunisa)
