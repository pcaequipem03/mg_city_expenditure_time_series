# Detecting and Analyzing Anomalies in City Expenditure Time Series

This repository contains the datasets used in the paper:

**_Detecting and Analyzing Anomalies in City Expenditure Time Series_**

The study presents an enhanced approach for detecting and analyzing anomalies in public expenditure time series. The method combines statistical techniques and machine learning models to identify unusual spending behaviors and rank expenditure items according to both the frequency of anomalies and their monetary impact. The goal is to generate suspicion alerts of potential fraud, helping prioritize cases and guide human auditing efforts more effectively.

In this extended version, the analysis is performed at a finer level of granularity within the governmental budget structure, enabling the detection of irregularities that may not be visible in more aggregated views. The approach is validated on a real-world dataset comprising over one million expenditure records from cities in the state of Minas Gerais, Brazil.

---

## 📂 Dataset Description

The repository provides two time series datasets derived from public expenditure data.

### 1. `time_series_function.csv`

Time series aggregated at the **function level**.

**Columns:**
- `city`: Name or identifier of the city  
- `function`: Government budget function (e.g., health, education)  
- `sub_function`: Subcategory within the function  
- `month`: Month of the record (1–12)  
- `year`: Year of the record  
- `value`: Total expenditure for the given aggregation  

---

### 2. `time_series_sub_function.csv`

Time series aggregated at a more detailed **sub-function level**, enabling finer-grained analysis.

**Columns:**
- `city`: Name or identifier of the city  
- `function`: Government budget function  
- `sub_function`: Detailed expenditure category  
- `month`: Month of the record (1–12)  
- `year`: Year of the record  
- `value`: Total expenditure for the given aggregation  

---

## 📊 Use Case

These datasets are intended to support:
- Time series anomaly detection  
- Public expenditure monitoring  
- Fraud detection and auditing support  
- Analysis of spending patterns across cities and budget categories  

---

## 🗂️ Data Source

The data used in this study were extracted from the **Computerized System of Municipal Accounts (SICOM)** (*Sistema Informatizado de Contas dos Municípios*), an open database maintained by the **Court of Accounts of the State of Minas Gerais (TCE-MG)** (*Tribunal de Contas do Estado de Minas Gerais*).

- SICOM Portal: https://portalsicom1.tce.mg.gov.br/  
- Open Data Portal (raw data): https://dadosabertos.tce.mg.gov.br/  

The raw SICOM data is publicly available through the official open data portal. From this source, we constructed the preprocessed datasets provided in this repository, including the time series used in our experiments.

---


## 📖 Citation

If you use this dataset, please cite:
