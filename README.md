# Validate Using Unseen Code Samples

## 📌 Project Overview

This project demonstrates how a code-review assistant can be validated using **unseen code samples**. The system analyzes a new code sample that was not previously reviewed, identifies potential issues, classifies their severity, and provides recommended fixes.

The goal is to evaluate whether the review workflow can consistently detect common coding, quality, and security issues in previously unseen source code.

---

## 🎯 Objectives

The main objectives of this project are:

* Validate the code-review workflow on unseen code.
* Detect common coding and security issues.
* Classify issues based on severity.
* Generate fix recommendations.
* Produce a validation summary report.
* Demonstrate a simple automated review process.

---

## 🛠️ Technologies Used

| Technology   | Purpose                      |
| ------------ | ---------------------------- |
| Python       | Implementation               |
| Google Colab | Execution environment        |
| LLM Concepts | Issue explanation and review |
| GitHub       | Version control and hosting  |

---

## 📂 Project Structure

```text
Validate-Using-Unseen-Code-Samples/
│
├── validate_unseen_code_samples.py
└── README.md
```

---

## 🔍 Unseen Code Sample

The project validates the reviewer using the following unseen code sample:

```python
import os

password = "secret123"

def calculate(a,b):
    return a/b

unused_var = 10
```

---

## 🚨 Issues Detected

### 1. Hardcoded Password

**Severity:** High

**Suggested Fix:**

```text
Store credentials in environment variables.
```

---

### 2. Unused Import

**Severity:** Medium

**Suggested Fix:**

```text
Remove the unused import.
```

---

### 3. Unused Variable

**Severity:** Medium

**Suggested Fix:**

```text
Remove the variable or use it.
```

---

### 4. Missing Whitespace After Comma

**Severity:** Low

**Suggested Fix:**

```text
Add a space after the comma.
```

---

## 🤖 Validation Process

The reviewer performs the following steps:

1. Load an unseen code sample.
2. Detect potential issues.
3. Classify issues by severity.
4. Generate fix recommendations.
5. Produce a validation report.

---

## 📋 Sample Output

```text
========== REVIEW RESULTS ==========

Issue 1: Hardcoded Password
Severity: High
Suggested Fix: Store credentials in environment variables.
----------------------------------------

Issue 2: Unused Import
Severity: Medium
Suggested Fix: Remove the unused import.
----------------------------------------

Issue 3: Unused Variable
Severity: Medium
Suggested Fix: Remove the variable or use it.
----------------------------------------

Issue 4: Missing Whitespace After Comma
Severity: Low
Suggested Fix: Add a space after the comma.
----------------------------------------

========== VALIDATION SUMMARY ==========
Total Issues Detected: 4
Validation Successful
```

---

## 🔄 Workflow

```text
      Unseen Code Sample
                ↓
        Issue Detection
                ↓
    Severity Classification
                ↓
      Suggested Fixes
                ↓
      Validation Report
                ↓
      Validation Summary
```

---

## 📚 Learning Outcomes

This project demonstrates:

* Validation using unseen code samples
* Automated issue detection
* Severity classification
* Code-fix recommendation generation
* Basic code-review automation
* Software quality assessment concepts

---

## 🚀 How to Run

### Step 1: Open Google Colab

Create a new notebook.

### Step 2: Copy the Code

Paste the contents of:

```text
validate_unseen_code_samples.py
```

into a code cell.

### Step 3: Run the Program

Execute the cell.

### Step 4: View Results

The program will:

1. Analyze the unseen code sample.
2. Detect issues.
3. Classify severity levels.
4. Display fix recommendations.
5. Generate a validation summary.

---

## 👩‍💻 Author

**Divya K**

---

## 📌 Project Type

**Validation of an Automated Code Review Assistant Using Unseen Code Samples**
