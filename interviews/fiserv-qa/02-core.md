# 🧪 02 - Core Testing Skills

## 📌 Overview

- Core testing skills are the foundation of effective QA work.
- Strong testers can plan, design, execute, track, and analyze defects systematically.

## 📝 Test Planning

- Define scope, objectives, risks, and timelines.
- Identify what to test and what not to test.

## ✅ Test Case Design

- Use equivalence partitioning.
- Apply boundary value analysis.
- Use decision table testing.
- Apply state transition testing.

Example:

- For age field:
  - valid: 18, 25, 60
  - invalid: 17, -1, 1000

## 🗂️ Test Case Management

- Keep test cases modular and reusable.
- Group by feature or module.
- Track status: Draft, Ready, Executed, Passed, Failed, Blocked.

## 🐞 Defect Management

- Use a clear title.
- Include steps to reproduce.
- Capture expected vs actual result.
- Add environment details.
- Mention severity and priority.

## 🔍 Root Cause Analysis

- Ask: Why did it happen?
- Review logs, code, data, environment, and configuration.

## 🗄️ Data Validation (SQL)

Example SQL checks:

```sql
SELECT COUNT(*) FROM users WHERE email IS NULL;
SELECT username FROM users WHERE status = 'inactive';
```
