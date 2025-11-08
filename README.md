# Healthcare Readmission & Cost Prediction Analysis

This project analyzes Medicare patient claims and beneficiary data to **predict hospital readmissions** and **estimate healthcare costs** within 30, 60, and 90 days. It integrates inpatient, outpatient, drug exposure, and clinical concept data to build a unified patient-level analytical dataset.

---

## 🏥 Project Objectives

- Merge and preprocess multi-year Medicare claims data
- Engineer healthcare utilization and chronic condition variables
- Calculate readmission events over 30/60/90-day windows
- Integrate prescription drug exposure and clinical concept metadata
- Model patient readmission risk and analyze key predictive factors
- Estimate associated medical reimbursement costs

---

## 📂 Dataset Components

| Dataset | Description |
|--------|-------------|
| Beneficiary Summary (bene08, bene09, bene10) | Patient demographic + chronic condition indicators |
| Inpatient Claims | Hospital admission records |
| Outpatient Claims | Ambulatory & outpatient visit claims |
| Drug Exposure Data | Prescription dispensing history |
| Concept Metadata | Standardized drug & condition terminology |

> **Note:** Paths reference Google Drive locations; adjust as needed.

---

## 🔧 Key Features Engineered

- Chronic condition flags (e.g., Diabetes, CHF, COPD, Depression, Stroke)
- Claim cost summaries (inpatient, outpatient, primary payer, beneficiary payments)
- Date-driven readmission flags:
  - `readmit_30`
  - `readmit_60`
  - `readmit_90`
- Drug exposure linked using standardized clinical concept identifiers

---

## 🧠 Modeling

The notebook demonstrates:
- Data cleaning and feature preparation
- Feature merging across claims and beneficiary profiles
- Predictive modeling for **readmission risk**
- Cost estimation for future medical utilization

---

## 🛠️ Technologies Used

| Category | Tools / Libraries |
|---------|-------------------|
| Language | Python |
| Data Handling | pandas, numpy |
| Visualization | matplotlib, seaborn |
| Machine Learning | scikit-learn |
| Notebook | Jupyter / Google Colab |

---

## ▶️ Running the Project

### **Option 1 – Google Colab (Recommended)**
1. Upload notebook to Colab
2. Mount Google Drive containing data:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
