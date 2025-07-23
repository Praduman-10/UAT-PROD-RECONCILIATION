# UAT-PROD-RECONCILIATION

# 📊 Datasets Recon Automation 3.0

This project is a fully automated **Data Reconciliation Pipeline** built using Python and Jupyter Notebook. It is designed to compare structured datasets from **UAT (User Acceptance Testing)** and **Production** environments to identify mismatches, validate transformations, and ensure data consistency across stages.

---

## 💼 Use Case

In real-world data workflows, validating that UAT and Production datasets match is critical for ensuring quality before deployment. This notebook acts as a lightweight ETL validator, highlighting discrepancies at both the schema and record levels.

---

## 🚀 What This Pipeline Does

### ✅ Features:

- **Automatic File Comparison**: Accepts two structured files (e.g., `.csv`, `.xlsx`) from UAT and PROD.
- **Schema Matching**: Checks column names and order; identifies missing, extra, or renamed columns.
- **Row-Level Comparison**: Matches rows based on key columns (e.g., IDs or composite keys).
- **Mismatch Reporting**: Clearly highlights differences in:
  - Data types
  - Null values
  - Row counts
  - Field-level content
- **Tolerance Handling**: Handles minor differences in numerical precision (optional).
- **Logging & Exports**: Generates mismatch logs and summary reports.
- **Flexible Matching Logic**: User can define key columns and configure matching sensitivity.
- **Multi-Sheet Support**: Handles comparison across multiple sheets or tabs if Excel files are used.
- **Structured Output**: Produces downloadable Excel or CSV with:
  - Matched rows
  - Mismatches with reason
  - Summary statistics

---

## 🛠️ Tech Stack

- Python 3.x
- Jupyter Notebook
- `pandas`, `openpyxl`, `numpy`

---

## 🌟 Key Strengths

| Feature | Benefit |
|--------|---------|
| 🔁 Fully automated | Save hours of manual reconciliation |
| 📑 Structured summary | Clear reporting for QA, Dev, or Data Teams |
| 🔎 Granular mismatch insights | Pinpoint exactly where and why data differs |
| ⚙️ Configurable logic | Works across projects with varying rules |
| 📁 Multiple formats supported | Accepts `.csv`, `.xlsx`, etc. |
| 🧠 Easy to understand | Clear markdowns and inline comments |

---

## ⚠️ Limitations & Future Enhancements

| Limitation | Workaround / Future Plan |
|------------|--------------------------|
| ❌ No fuzzy matching | Plan to integrate fuzzywuzzy or rapidfuzz for approximate string comparison |
| ❌ Only structured data | Current version does not handle semi-structured (JSON/XML) |
| ❌ Manual file input | Future scope: build a CLI or Streamlit GUI for file selection |
| ❌ No database connectors | Currently supports only file inputs, Only pull static data from DB's and not the live DBs (e.g., SQL) |

---
