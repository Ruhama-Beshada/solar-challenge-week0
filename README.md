
# 🌞 Solar Challenge Week 0 — Environment Setup & EDA Preparation

## 📘 Project Overview
This repository contains the setup and exploratory data analysis (EDA) workflow for the **Solar Challenge Week 0**.  
The goal is to profile, clean, and explore solar datasets from **Benin (Malanville)**, **Togo (Dapaong)**, and **Sierra Leone (Bumbuna)** to prepare clean and comparable datasets for later analysis.

---

## ⚙️ Environment Setup

### 1. Clone the Repository
bash
git clone https://github.com/Ruhama-Beshada/solar-challenge-week0.git
cd solar-challenge-week0
# Create a virtual environment
python -m venv venv

# Activate environment
# On Windows
venv\Scripts\activate
# On macOS/Linux
source venv/bin/activate

# instal Dependencies
pip install -r requirements.txt

# Repository Structure
 
solar-challenge-week0/
│
├── .github/workflows/           # CI/CD workflows for testing
│   └── unittests.yml
│
├── notebooks/                   # Jupyter notebooks for EDA
│   ├── __init__.py
│   ├── README.md
│   ├── benin_eda.ipynb
│   ├── togo_eda.ipynb
│   └── sierra_leone_eda.ipynb
│
├── src/                         # Source scripts and helpers
│   ├── __init__.py
│   └── utils.py
│
├── tests/                       # Unit tests for validation
│   └── __init__.py
│
├── data/                        # (Git-ignored) raw & cleaned datasets
│   └── *.csv
│
├── requirements.txt             # Python dependencies
├── .gitignore                   # Files/folders excluded from Git
├── README.md                    # Project documentation
└── interim_report.md             # Week 0 interim report
# Task 2
## Data Analysis Workflow

## Task 2.1 — Data Loading & Inspection

Load raw CSV files for Benin, Sierra Leone, and Togo.

Inspect column types, missing values, and initial statistics.

## Task 2.2 — Country-Level EDA & Cleaning

Cleaning: Impute missing values with median, remove outliers using Z-score threshold.

## Visualizations:

Line plots: Solar irradiance (GHI, DNI, DHI) vs. Timestamp

Scatter plots & correlations: Wind speed/direction, temperature, relative humidity

Bubble plots: GHI vs. temperature with RH as bubble size

Outputs: Cleaned CSV files stored in data/ (not committed to Git).

# Task 3 — Cross-Country Comparison

Load cleaned datasets for all three countries.

Compare solar metrics (GHI, DNI, DHI) using:

Boxplots side-by-side by country

Summary tables (mean, median, standard deviation)

Optional ANOVA/Kruskal-Wallis statistical testing

## Visual summary:

Bar chart ranking countries by average GHI

Key observations documented in notebook markdown cells.

# Key Insights

## Benin (Malanville): Highest median GHI, consistent solar irradiance throughout the year.

## Sierra Leone (Bumbuna): Moderate solar potential, more variability in DNI and DHI.

## Togo (Dapaong): Lowest median GHI but stable trends, low variability.

Differences between countries are statistically significant based on ANOVA results (p-values < 0.05).

# Git Branches & Notebooks
Branch	Notebook	Purpose
eda-benin	benin_eda.ipynb	Country-specific EDA for Benin
eda-sierraleone	sierraleone_eda.ipynb	Country-specific EDA for Sierra Leone
eda-togo	togo_eda.ipynb	Country-specific EDA for Togo
compare-countries	compare_countries.ipynb	Cross-country comparison
# Usage

Activate virtual environment

Run notebooks in order:

benin_eda.ipynb

sierraleone_eda.ipynb

togo_eda.ipynb

compare_countries.ipynb

Inspect generated plots, tables, and cleaned CSVs.


>>>>>>> 36a5ab7be03b44579f720e81d5e1fe7c37dee4a7
