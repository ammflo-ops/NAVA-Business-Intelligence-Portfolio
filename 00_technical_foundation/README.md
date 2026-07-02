# 00 Technical Foundation (Shared SQL Architecture)

This section contains the shared SQL architecture powering the entire NAVA Business Intelligence solution.

All analytical projects rely on the same SQL data warehouse, ensuring consistent business definitions, standardized transformations and reusable analytical views.

---

# 🏗️ Data Architecture

The solution follows a multi-layer SQL architecture designed to transform raw operational data into business-ready datasets.

<p align="center">
  <img src="../assets/NAVA_data_architecture.png" width="900">
</p>

1. **NAVA_Raw Layer**        : Store source data without transformation
2. **NAVA_Clean Layer**      : Clean, standardize and enrich the datasets
3. **NAVA_Analytics Layer**  : Build business-ready SQL views for reporting
---

# 📖 Architecture Overview

The architecture is divided into three logical layers.

| Layer | Purpose |
|--------|---------|
| **Raw Layer** | Store source data without transformation |
| **Clean Layer** | Clean, standardize and enrich the datasets |
| **Analytics Layer** | Build business-ready SQL views for reporting |

---

# 🚀 Project Components

## 📂 01 Raw Layer

### Objective

Load raw CSV files into the SQL database while preserving the original data structure.

### Key Activities

- Raw data ingestion
- Full load process
- No transformations
- Source data preservation

---

## 🧹 02 Clean Layer

### Objective

Prepare reliable datasets through cleansing, standardization and business rules.

### Key Activities

- Data cleansing
- Standardization
- Normalization
- Derived columns
- Business rules
- Referential integrity

---

## 📊 03 Analytics Layer

### Objective

Create reusable analytical views optimized for business reporting.

### Analytical Views

- `vw_sales_net`
- `vw_budget_vs_actual`
- `vw_marketing_performance`
- `vw_marketing_conversion`

---

# ✔ Data Quality

The project includes SQL validation scripts used to improve dataset reliability.

Examples include:

- Duplicate detection
- NULL value validation
- Referential integrity checks
- Business rule validation

---

# 📂 Repository Structure

```text
00_Technical_Foundation
│
├── datasets/
│
├── scripts/
│   ├── 01_Raw_Layer/
│   ├── 02_Clean_Layer/
│   ├── 03_Analytics_Layer/
│   └── 04_Data_Quality/
│
└── README.md
```

---

# 💡 Purpose

The objective of this technical foundation is to provide a single, reliable and reusable SQL architecture supporting all analytical projects within the NAVA Business Intelligence portfolio.
