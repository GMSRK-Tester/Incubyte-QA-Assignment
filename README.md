# 📧 Gmail Compose Function – QA Test Cases
### Incubyte QA Assignment Submission

> **Tester:** Gubbala Mega Shiva Rama Krishna
> **Testing Platform:** Gmail (Web) | Chrome Browser | Windows Laptop
> **Submission Format:** Excel Sheet (.xlsx)

----------------------------------------------------------------------------------

## 📌 Assignment Overview

**Objective:**
To test the Compose function in Gmail — specifically to send an email with:
- **Subject:** 'Incubyte'
- **Body:** 'QA test for Incubyte'

**Deliverables:**
1. ✅ Traditional Style Test Cases
2. ✅ BDD (Behaviour-Driven Development) Style Test Cases
3. ✅ Both Positive and Negative test cases covered
4. ✅ Submitted via Git URL in Excel format

----------------------------------------------------------------------------------

## 📁 Repository Structure

```
📦 Incubyte-QA-Assignment
 ┣ 📄 README.md                          ← You are here
 ┗ 📊 Gmail_Compose_Test_Cases.xlsx      ← Test Cases (Traditional + BDD)
```

----------------------------------------------------------------------------------

## 📊 Test Summary

| Category                         | Count |
|----------------------------------|-------|
| **Total Traditional Test Cases** | 48    |
| **Total BDD Scenarios**          | 43    |
| **Total Test Cases**             | 91    |
| ✅ Pass                         | 91    |
| ❌ Fail                         | 0     |

### 🔢 By Type
| Type     | Count |
|----------|-------|
| ➕ Positive | 69  |
| ➖ Negative | 22  |

### 🚦 By Priority
| Priority | Count |
|----------|-------|
| 🔴 High   | 16   |
| 🟡 Medium | 34   |
| 🟢 Low    | 41   |

### ⚠️ By Severity
| Severity  | Count |
|-----------|-------|
| 🔴 Critical | 6   |
| 🟠 Major    | 28  |
| 🟡 Minor    | 41  |
| ⚪ Cosmetic | 16  |

----------------------------------------------------------------------------------

## 🧪 Traditional Test Cases – Modules Covered

| Module                        | Test Cases             |
|-------------------------------|------------------------|
| Compose – Launch              | TC_001                 |
| Compose – Window Controls     | TC_002, TC_003, TC_004, TC_005 |
| Compose – Close / Draft Save  | TC_006, TC_007, TC_033, TC_034, TC_035 |
| Compose – Send Mail           | TC_008 to TC_013       |
| Compose – CC / BCC / Multiple | TC_014, TC_015, TC_016 |
| Compose – Schedule Send       | TC_017, TC_018         |
| Compose – Text Formatting     | TC_019 to TC_025       |
| Compose – Insert (Link/Emoji/Image/Signature) | TC_026 to TC_032 |
| Compose – Multiple Windows    | TC_036                 |
| Compose – Keyboard Shortcut   | TC_037                 |
| Compose – Authentication      | TC_038                 |
| Compose – Subject Field       | TC_039 to TC_042       |
| Compose – Body Field          | TC_043 to TC_046       |
| Compose – Edge Cases          | TC_047, TC_048         |

----------------------------------------------------------------------------------

## 🥒 BDD Test Cases – Scenarios Covered

BDD test cases follow the **Given / When / Then** format.

| Scenario ID | Scenario Title |
|-------------|----------------|
| BDD_001 | Open Compose window |
| BDD_002 | Maximize Compose window |
| BDD_003 | Restore Compose window from full screen |
| BDD_004 | Minimize Compose window |
| BDD_005 | Reopen a minimized Compose window |
| BDD_006 | Close Compose window with no data entered |
| BDD_007 | Close Compose window after entering data saves a draft |
| BDD_008 | Send email with valid recipient, subject and body |
| BDD_009 | Send email without a subject |
| BDD_010 | Send email without a body |
| BDD_011 | Send email without subject and without body |
| BDD_012 | Attempt to send email without a recipient |
| BDD_013 | Attempt to send email with an invalid recipient address |
| BDD_014 | Send email by adding a CC recipient |
| BDD_015 | Send email by adding a BCC recipient |
| BDD_016 | Send email to multiple recipients in To field |
| BDD_017 | Schedule an email for future delivery |
| BDD_018 | Cancel a scheduled email before delivery |
| BDD_019 | Apply Bold formatting to body text |
| BDD_020 | Apply Italic formatting to body text |
| BDD_021 | Apply Underline formatting to body text |
| BDD_022 | Change font size of selected body text |
| BDD_023 | Change font color of selected body text |
| BDD_024 | Insert a hyperlink in the email body |
| BDD_025 | Insert an emoji into the email body |
| BDD_026 | Attach a local file to the email |
| BDD_027 | Attempt to attach a file larger than 25MB |
| BDD_028 | Insert a file from Google Drive |
| BDD_029 | Insert an inline image in the email body |
| BDD_030 | Insert a saved signature into the email |
| BDD_031 | Discard an in-progress draft |
| BDD_032 | Reopen and send a previously saved draft |
| BDD_033 | Close the Compose window while maximized |
| BDD_034 | Open multiple Compose windows simultaneously |
| BDD_035 | Compose button unavailable when logged out |
| BDD_036 | Subject field accepts maximum length text |
| BDD_037 | Subject field accepts special characters |
| BDD_038 | Subject field accepts Unicode and emoji |
| BDD_039 | HTML-like text in body is treated as plain text |
| BDD_040 | Body text is retained after switching browser tabs |
| BDD_041 | Paste text into the body field |
| BDD_042 | Send to a syntactically valid but non-existent address |
| BDD_043 | Attempt to send email with no internet connection |

----------------------------------------------------------------------------------

## 🔑 Key Negative Test Cases Highlighted

| Test Case | Scenario | Expected Outcome |
|-----------|----------|-----------------|
| TC_006 / BDD_006 | Close compose with no data | No draft saved |
| TC_012 / BDD_012 | Send with empty To field | Error: "Please specify at least one recipient" |
| TC_013 / BDD_013 | Send with invalid email format | Error: address not recognized |
| TC_029 / BDD_027 | Attach file > 25MB | Auto-converted to Google Drive link |
| TC_033 / BDD_031 | Discard draft | "Draft discarded" — no draft saved |
| TC_047 / BDD_042 | Send to non-existent valid address | Bounce notification received later |
| TC_048 / BDD_043 | Send with no internet | Network error, auto-saved to Drafts |

----------------------------------------------------------------------------------

## ✅ How to View the Test Cases

1. Download the Excel file 'Gmail_Compose_Test_Cases.xlsx' from this repository
2. Open it in **Microsoft Excel** or **Google Sheets**
3. Navigate between the three sheets:
   - **Legend & Summary** – Overall stats and color-code key
   - **Traditional Test Cases** – 48 detailed manual test cases
   - **BDD Test Cases** – 43 BDD-style Gherkin scenarios

----------------------------------------------------------------------------------

## 👤 Tester Details

| Field                | Details                         |
|----------------------|---------------------------------|
| **Name**             | Gubbala Mega Shiva Rama Krishna |
| **Reviewed By**      | Not Available                   |
| **Reviewer Remarks** | Not Available                   |

----------------------------------------------------------------------------------

*Submitted as part of the Incubyte QA Engineer Assignment.*
