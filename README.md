# Zillow Log-Error Prediction

**A Colab-based pipeline for predicting Zillow’s Zestimate log-error using EDA, feature engineering, and hyperparameter-tuned models (XGBoost & LinearRegression).**

---

## Table of Contents

- [Project Overview](#project-overview)  
- [Repository Structure](#repository-structure)  
- [Getting Started](#getting-started)  
  - [Prerequisites](#prerequisites)  
  - [Install Dependencies](#install-dependencies)  
  - [Open in Colab](#open-in-colab)  
- [Pipeline Breakdown](#pipeline-breakdown)  
- [Usage](#usage)  
- [Contributing](#contributing)  
- [License](#license)  
- [Contact](#contact)  

---

## Project Overview

This project tackles the **Zillow Prize** challenge of predicting the **log-error** in Zillow’s home-value estimates (“Zestimates”). It runs entirely in **Google Colab** and demonstrates:

- **Data Loading & Inspection**  
- **Exploratory Data Analysis (EDA)**  
- **Data Cleaning & Missing-Value Handling**  
- **Feature Engineering & Transformations**  
- **Model Training & Hyperparameter Tuning**  
- **Result Interpretation & Next Steps**

---

## Repository Structure

```text
zillow-logerror-prediction/
├── ZXTRN_HOUSING_DATA.ipynb   # Main Colab notebook  
├── README.md                  # Project overview & instructions  
├── requirements.txt           # Python dependencies  
