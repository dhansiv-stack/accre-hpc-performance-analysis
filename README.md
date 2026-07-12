# ACCRE HPC Performance Analysis

## Project Overview

This project analyzes operational data from Vanderbilt University's Advanced Computing Center for Research and Education (ACCRE) High-Performance Computing (HPC) cluster to investigate whether bursts of completed Slurm jobs contribute to scheduler unresponsiveness.

The analysis integrates large-scale Slurm job records with scheduler log files to identify unresponsive events, engineer analysis-ready features, and evaluate the relationship between workload patterns and scheduler performance using statistical analysis and data visualization.

## Dataset Overview

The analysis integrates three operational datasets from Vanderbilt University's ACCRE HPC environment:

- **fullsample.csv** – Slurm job execution records.
- **slurm_wrapper_ce5.log** – Scheduler command logs from the CE5 gateway.
- **slurm_wrapper_ce6.log** – Scheduler command logs from the CE6 gateway.

---

## Project Objectives

- Analyze HPC scheduler performance using operational cluster data.
- Identify completed Slurm jobs and scheduler unresponsive events.
- Clean and integrate multiple large-scale datasets.
- Engineer features suitable for statistical analysis.
- Evaluate whether bursts of job completions increase the likelihood of scheduler unresponsiveness.

---

## Project Workflow

```text
Slurm Job Records
        │
        ├──────────────┐
        │              │
        ▼              ▼
  CE5 Scheduler Logs  CE6 Scheduler Logs
        │              │
        └──────┬───────┘
               ▼
      Data Cleaning & Parsing
               │
               ▼
      Feature Engineering
               │
               ▼
     Exploratory Data Analysis
               │
               ▼
     Statistical Modeling
     (Logistic Regression)
               │
               ▼
   Performance Analysis &
      Hypothesis Testing
```

---

## Technologies Used

- Python
- pandas
- NumPy
- Matplotlib
- Statsmodels
- Logistic Regression
- High-Performance Computing (HPC)
- Slurm Workload Manager

---

## Skills Demonstrated

- Data Cleaning
- Feature Engineering
- Exploratory Data Analysis (EDA)
- Statistical Modeling
- Logistic Regression
- HPC Log Analysis
- Performance Analytics
- Scientific Data Interpretation

---

## Key Features

- Processed over seven million Slurm job records.
- Parsed and combined scheduler log files from multiple compute gateways.
- Identified scheduler unresponsive events using predefined operational criteria.
- Engineered analysis-ready features from heterogeneous datasets.
- Applied logistic regression to evaluate the relationship between job completion bursts and scheduler responsiveness.
- Produced visualizations and statistical summaries to support hypothesis testing.

---

## Repository Contents

```text
├── README.md
├── notebooks/
│   ├── Data_Introduction.ipynb
│   └── ACCRE_HPC_Performance_Analysis.ipynb
├── ACCRE Introduction.pdf
└── data_dictionary.md
```

> **Note:** The original datasets are not included in this repository because of their large size. The notebooks assume the required data files are available locally.
---

## Future Improvements

- Develop predictive models for scheduler unresponsiveness.
- Incorporate additional resource utilization metrics.
- Evaluate temporal trends and seasonal workload patterns.
- Build an interactive dashboard for HPC performance monitoring.

---

**Author:** Sivaraja Vaithiyalingam