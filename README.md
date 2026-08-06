# Temporal Graph AML Detection

## Project Overview

This project explores anti-money-laundering detection using synthetic financial transaction data.

The goal is to build a realistic machine learning pipeline for suspicious transaction detection, starting with transaction-level data understanding and later extending toward temporal feature engineering, tabular machine learning, graph construction, and graph-based AML detection.

## Problem Context

Anti-money-laundering systems help financial institutions identify suspicious transactions and accounts. In real banking environments, laundering activity is rare compared with normal activity, so the problem is highly imbalanced.

Instead of focusing only on accuracy, this project will focus on AML-oriented evaluation such as:

- Precision at top-K alerts
- Recall at top-K alerts
- PR-AUC
- Suspicious transaction ranking
- Temporal train/validation/test splits

## Dataset

Dataset: IBM Transactions for Anti Money Laundering

The selected starter file is:

```text
HI-Small_Trans.csv

Current dataset summary:

Transactions: 5,078,345
Laundering transactions: 5,177
Laundering rate: 0.1019%
Time range: 2022-09-01 00:00:00 to 2022-09-18 16:18:00
Unique senders: 496,999
Unique receivers: 420,640
Payment formats: 7
Payment currencies: 15

Raw and processed data files are not committed to GitHub. The notebook contains the download and preprocessing steps.

Repository Structure
temporal-graph-aml/
├── notebooks/
│   └── 01_data_understanding.ipynb
├── data/
│   ├── raw/              # ignored by git
│   └── processed/        # ignored by git
├── reports/
│   └── figures/          # ignored by git for now
├── models/               # ignored by git
├── README.md
├── requirements.txt
└── .gitignore
Current Progress
 Google Colab workspace setup
 Dataset downloaded to Google Drive
 Raw file inspection
 Clean column schema
 Clean Parquet generation
 Dataset overview
 Exploratory data analysis
 Temporal split
 Feature engineering
 Tabular baseline model
 Graph construction
 Graph-based modelling
 Explainability and alert analysis
Planned Notebooks
01_data_understanding.ipynb
02_temporal_split_and_features.ipynb
03_tabular_baseline.ipynb
04_graph_construction.ipynb
05_graph_model.ipynb
Tech Stack
Python
Google Colab Pro
Polars
Pandas
NumPy
Matplotlib
Scikit-learn
LightGBM
NetworkX
PyTorch Geometric later
Project Goal

The final goal is to demonstrate an end-to-end AML detection workflow that includes:

Clean data preparation
Temporal data understanding
Extreme class imbalance handling
Strong tabular ML baseline
Graph-based transaction representation
AML-specific model evaluation
Investigation-oriented interpretation