---
name: 🐛 Bug report
about: Create a report to help us improve the ETL pipeline
title: '[BUG] '
labels: 'bug'
assignees: ''

---

## 📝 Description

Briefly describe the problem. Is it a failure during data extraction, a transformation error (e.g., incorrect age imputation), or a loading issue into SQLite?

## 👣 How to Reproduce

Steps to reproduce the behavior:
1. Run the main script/notebook: `[filename].ipynb` or `python main.py`
2. Reach the step: '...' (e.g., "Loading data into SQLite")
3. See error: '...' (e.g., `OperationalError: table passengers has no column named...`)

## 🎯 Expected Behavior

A clear and concise description of what you expected to happen (e.g., the SQLite database should be created with 891 rows and no null values in the 'Age' column).

## 📸 Screenshots or Console Output (if applicable)

If the bug relates to a data visualization or a specific terminal error, please paste a screenshot or the raw text here.



## 💻 Environment

- **OS:** (e.g. Windows 11, macOS, Ubuntu)
- **Python Version:** (e.g. 3.10.x)
- **Pandas Version:** (e.g. 1.5.x)
- **Database Tool:** (e.g., DB Browser for SQLite, DBeaver, or internal Python sqlite3)

## 🔍 Additional Context

Add any other context about the problem here. If the terminal showed an error message (Traceback), please paste it here:

```text
[Paste your error log here]
```
