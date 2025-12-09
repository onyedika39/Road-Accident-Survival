# 🚑 Road Accident Survival Analysis (Python EDA)

![Dashboard Preview](https://github.com/onyedika39/Road-Accident-Survival/blob/main/dataset_cover.jpg)

 ---
 
## Overview
This project explores **factors associated with survival in road accidents** using a structured tabular dataset.  
The analysis is implemented end-to-end in a Jupyter Notebook using **Python, Pandas, NumPy, Matplotlib, and Seaborn**.

The main goal is to understand how **age, gender, speed, helmet use, and seatbelt use** relate to the likelihood of surviving a road accident, and to practice a clear exploratory data analysis (EDA) workflow suitable for real-world analytics roles.

---

## Business Motivation
Road accidents are a major public health problem. Survival often depends not only on the severity of the crash but also on **human behaviour** and **safety equipment usage**.

By analysing an accident survival dataset, this project aims to:

- Quantify how survival varies across demographic groups.
- Compare survival outcomes for people who **used helmets or seatbelts** versus those who did not.
- Build evidence that can support **policy**, **education**, and **enforcement** decisions in road safety.

---

## Dataset

The dataset contains one row per person involved in a road accident.  
Key columns used in the analysis include:

- `Age` – Age of the individual.
- `Gender` – Gender of the individual.
- `Speed` – Reported speed at the time of the accident.
- `Survived` – Survival outcome (e.g. 1 = survived, 0 = did not survive).
- `Helmet_Used` – Whether a helmet was used.
- `Seatbelt_Used` – Whether a seatbelt was used.

> Note: the notebook focuses on cleaning, exploring, and visualising these core features rather than building predictive models.

---

## Methodology

### 1. Data Loading & Inspection
- Loaded the CSV file into a Pandas DataFrame.
- Inspected structure using `.head()`, `.info()`, and `.describe()`.
- Verified column types and basic distributions.

### 2. Data Cleaning
- Removed records with missing values (`dropna`) to ensure consistent analysis.
- Checked data types for each column (numeric vs categorical).
- Performed simple sanity checks (e.g. reasonable age and speed values).

### 3. Exploratory Data Analysis (EDA)
Core questions explored:

- **Age distribution** of accident victims.
- **Number of accidents by gender**.
- **Overall survival distribution** (how many survived vs did not).
- **Minimum and maximum speeds** recorded.
- **Counts of accidents involving helmet use**.
- **Counts of accidents involving seatbelt use**.
- **Survival rates by gender**.
- **Survival rates by helmet and seatbelt usage**.

Visuals created in the notebook include:

- Histogram of `Age`  
- Bar charts of `Gender`, `Helmet_Used`, and `Seatbelt_Used`  
- Pie charts for overall survival distribution  
- Bar charts for survival counts by category

These plots give a fast, interpretable view of how different factors are related to survival.

---

## Key Analytical Highlights

- A full exploratory workflow is implemented: **loading → cleaning → summarising → visualising**.
- Survival is analysed from both a **demographic perspective** (age, gender) and a **behavioural/safety perspective** (helmet and seatbelt use).
- The notebook computes survival rates grouped by key variables, enabling comparisons such as:
  - survival percentage by gender
  - survival percentage for helmet vs no-helmet
  - survival percentage for seatbelt vs no-seatbelt
- Visualisations make the findings easy to communicate to non-technical stakeholders.

> This project is intentionally focused on **exploratory analysis and insight generation**, which is a critical step before building any predictive model.

---

## Recommendations & Next Steps

### Recommendations
- Use survival-by-equipment analysis to support stronger **helmet** and **seatbelt** adoption campaigns.
- Target road safety education at demographic groups that appear more frequently in severe or non-survival cases.
- Combine this dataset with additional contextual data (e.g. time of day, road type, vehicle type) to improve understanding of high-risk scenarios.

### Potential Extensions
- Build a **logistic regression model** to predict survival probability based on available features.
- Introduce **statistical tests** (e.g. chi-square tests for categorical associations).
- Engineer new features such as speed bands (low/medium/high) or age groups.
- Deploy a simple **Streamlit or Dash dashboard** to allow interactive exploration by policy makers or analysts.

---

## Tools & Technologies

- **Language:** Python  
- **Environment:** Jupyter Notebook  
- **Libraries:**  
  - `pandas`, `numpy`  
  - `matplotlib`, `seaborn`  
  - `PIL` / `IPython.display` for loading cover image  

---


