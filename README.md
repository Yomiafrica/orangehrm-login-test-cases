# OrangeHRM Login Page – Manual Test Cases

## 📋 Project Overview

This repository contains manual test cases for the **Login Page** of the [OrangeHRM Demo Application](https://opensource-demo.orangehrmlive.com/). The test cases cover a wide range of scenarios including functional, UI, security, performance, and compatibility testing.

- **Author:** Adesanya Oriyomi
- **Application Under Test:** OrangeHRM (Demo)
- **URL:** https://opensource-demo.orangehrmlive.com/
- **Test Type:** Manual Testing
- **Total Test Cases:** 75 (TC_001 – TC_075)

---

## 📁 File Structure

```
├── OrangeHRM_Login_Testcases.xlsx   # Test cases spreadsheet
└── README.md                        # Project documentation
```

---

## 🧪 Test Coverage Areas

| Category | Test Cases | Description |
|---|---|---|
| **Smoke / Navigation** | TC_001 – TC_002 | URL accessibility and login page load |
| **Functional – Authentication** | TC_003 – TC_016, TC_034, TC_075 | Valid/invalid credentials, blank fields, special characters, copy-paste, browser-saved credentials |
| **UI / Visual** | TC_019 – TC_022, TC_024, TC_035, TC_039, TC_040, TC_065, TC_066, TC_073 | Logo, layout alignment, error message styling, broken images, spelling |
| **Security** | TC_027 – TC_032, TC_057 | Password masking, show/hide icon, account lockout, session cookies, direct URL access |
| **Navigation & Redirects** | TC_007 – TC_008, TC_023, TC_026, TC_031, TC_069, TC_071, TC_074 | Logout, dashboard redirect, forgot password, back to login, OrangeHRM.inc link |
| **Input Validation** | TC_038, TC_041 – TC_047 | Blank fields, max character limits, special symbols, spaces, emojis, numbers-only |
| **Cross-Browser Compatibility** | TC_048 – TC_052 | Chrome, Microsoft Edge, Safari, Firefox, Android browser |
| **Session Management** | TC_055 – TC_060 | Multiple tabs, multiple browsers, session persistence on tab switch |
| **Performance** | TC_063 – TC_064, TC_068 | Page load time, slow network, high server load |
| **Edge Cases** | TC_059 – TC_062 | Long delay login, system time change, network disconnect, cache/cookie clearing |
| **Accessibility / UX** | TC_025, TC_054, TC_067, TC_070 | Mobile usability, zoom at 150%, tab key order, Escape key behaviour |
| **Error Handling** | TC_033, TC_036 – TC_038, TC_072 | Error message content, error disappears after login, repeated login behaviour, field clearing |

---

## ✅ Test Results Summary

| Status | Count |
|---|---|
| ✅ Pass | 70 |
| ❌ Fail | 5 |
| Total | 75 |

### ❌ Failed Test Cases

| Test Case | Description |
|---|---|
| TC_022 | Login button should be disabled until both fields are filled — **button is not disabled** |
| TC_028 | Show/hide password icon should be present — **icon is not present** |
| TC_030 | Account should lock after 5 failed login attempts — **account does not lock** |
| TC_041 | Username field should enforce a 40-character maximum — **accepts more than 40 characters** |
| TC_042 | Password field should enforce a 40-character maximum — **accepts more than 40 characters** |

---

## 🗂️ Test Case Structure

Each test case in the spreadsheet follows this format:

| Column | Description |
|---|---|
| **Test Case ID** | Unique identifier (e.g., TC_001) |
| **Test Case Description** | What is being tested |
| **Pre-condition** | State required before executing the test |
| **Test Steps** | Step-by-step instructions to execute the test |
| **Test Data (Input)** | Specific input values used |
| **Expected Result** | The correct, expected behaviour |
| **Actual Result** | What actually happened during testing |
| **Status** | Pass / Fail |

---

## 🔧 Test Environment

| Parameter | Details |
|---|---|
| **Application** | OrangeHRM Demo |
| **Browsers Tested** | Chrome, Microsoft Edge, Firefox, Safari, Android Browser |
| **Test Credentials** | Username: `Admin` / Password: `admin123` |
| **Testing Mode** | Manual |

---

## 🚀 How to Use This Repository

1. Clone or download the repository.
2. Open `OrangeHRM_Login_Testcases.xlsx` in Microsoft Excel or Google Sheets.
3. Navigate to the application URL: https://opensource-demo.orangehrmlive.com/
4. Execute each test case following the listed steps and input data.
5. Record the actual result and update the status (Pass/Fail) accordingly.

---

## 📌 Notes

- All test cases were executed on the **OrangeHRM open-source demo** environment.
- The demo application may be reset periodically, which could affect session-related test results.
- Failed test cases represent potential bugs or missing features in the current demo build.
