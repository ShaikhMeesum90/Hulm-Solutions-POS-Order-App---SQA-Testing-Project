# 🛒 Hulm POS & Order App - SQA Testing Project

![Build Status](https://img.shields.io/badge/Build-Passing-brightgreen)
![Test Coverage](https://img.shields.io/badge/Test%20Coverage-95%25-blue)
![Bug Count](https://img.shields.io/badge/Bugs%20Found-41-red)
![App Version](https://img.shields.io/badge/Version-1.0-orange)

## 📖 Overview

This repository contains the comprehensive **Software Quality Assurance (SQA)** artifacts for the **Hulm Solutions POS & Order Apps** ecosystem. The project focuses on manual functional testing, UI/UX validation, and rigorous bug tracking for a multi-module web application.

The testing process covered two primary applications:
1.  **POS App**: Point-of-Sale interface, cart management, and checkout workflows.
2.  **Order App**: Sales order processing, inventory management, and customer CRM.

---

## 📊 Testing Statistics

### **Bug Severity Breakdown**
A total of **41 bugs** were identified and documented during the testing lifecycle.

| Severity Level | Count | Description |
| :--- | :---: | :--- |
| 🔴 **High** | **14** | Critical functional blockers (e.g., Order fulfillment failures, Data duplication). |
| 🟡 **Mid** | **11** | Validation logic errors (e.g., Invalid input acceptance, Search malfunction). |
| 🟢 **Low** | **16** | UI/Alignment issues (e.g., Misaligned buttons, Text overflow). |

### **Execution Highlights**
* **Total Scenarios Covered**: 11+ High-Level Scenarios (TS_001 to TS_011).
* **Key Modules Tested**: Sales Order, Inventory, Products, Categories, Customers, POS Checkout.
* **Testing Type**: Black Box Testing, Manual Functional Testing, Negative Testing, UI Validation.

---

## 🕵️ Key Findings & Bugs

During the execution phase, several critical and functional issues were unearthed. Below is a snapshot of significant findings:

* **Logic Errors**: The system allowed the creation of **duplicate customers and products**, violating unique constraint requirements.
* **Validation Failures**: Numeric characters were accepted in "Name" fields, and invalid email formats were processed without error.
* **Critical Timezone Issue**: Order creation timestamps were off by **7 hours** (Server time vs. PST), affecting order tracking accuracy.
* **Functional Blockers**: 
    * "Complete Checkout" button functionality failed under specific conditions.
    * Reloading the POS page caused an unintended session logout.
* **UI/UX**: Multiple dropdowns and pagination controls were vertically misaligned, impacting the visual consistency of the dashboard.

---

## 📂 Repository Structure

The repository is organized into structured Excel/CSV logs for transparency and traceability:

* **`Hulm_POS&Order_App_TestCases.xlsx`**: Detailed test cases including steps, pre-requisites, and expected results.
* **`Hulm_POS&Order_App_TestExecutionResults.xlsx`**: Actual execution logs marking cases as **PASS/FAIL** with tester comments.
* **`Hulm_POS&Order_App_BugReport.xlsx`**: A consolidated list of all defects found, categorized by priority (High/Mid/Low).

---

## 🛠️ Tools & Technologies

* **Manual Testing**: Functional, Regression, and Sanity testing.
* **Test Management**: Excel-based Test Case Management.
* **Bug Tracking**: Structured Bug Reporting (ID, Scenario, Reproducible Steps).
* **Web Technologies Tested**: Responsive Web App (React/Node based environment).

---

## 🚀 Getting Started

To review the testing artifacts:
1.  Clone this repository.
2.  Open the `.xlsx` or `.csv` files to view detailed test steps and bug evidence.
3.  Refer to `Test Scenarios` for the high-level scope of the project.

---

**Created by:** Meesum  
**Project:** Hulm Solutions SQA
