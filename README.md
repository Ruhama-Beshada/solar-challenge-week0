
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



