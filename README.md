# Zillow Log-Error Prediction

A Colab-based pipeline for predicting Zillow’s Zestimate log-error using EDA, feature engineering, and hyperparameter-tuned models (XGBoost & LinearRegression).

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

This project tackles the **Zillow Prize** challenge of predicting the log-error in Zillow’s home-value estimates (“Zestimates”). It runs entirely in Google Colab and demonstrates:

- **Data Loading & Inspection**  
- **Exploratory Data Analysis (EDA)**  
- **Data Cleaning & Missing-Value Handling**  
- **Feature Engineering & Transformations**  
- **Model Training & Hyperparameter Tuning**  
- **Result Interpretation & Next Steps**

---

## Repository Structure

zillow-logerror-prediction/
├── ZXTRN_HOUSING_DATA.ipynb # Main Colab notebook
├── README.md # Project overview & instructions
├── requirements.txt # Python dependencies



---

## Getting Started

### Prerequisites

- A Google account for Colab  
- GitHub account (to fork or clone the repo)  
- (Optional) Local Python environment if you wish to run locally

### Install Dependencies

```bash
pip install -r requirements.txt


Click the badge or open this link in your browser:

https://colab.research.google.com/github/<your-username>/zillow-logerror-prediction/blob/main/ZXTRN

Then choose “Open in playground” to make a copy and run.



**Pipeline Breakdown**
Data Loading
Load properties_2016.csv, properties_2017.csv, train_2016_v2.csv, train_2017.csv, and sample_submission.csv from Google Drive or your local path.

EDA (explore_data)

Print shape & data types

List & plot missing-value percentages

Histogram grid of all numeric features

Cleaning (drop_high_missing_cols)
Remove columns with >80% missing values.

Comparison (compare_datasets)

Schema comparison (shared vs. unique columns)

Summary-statistic comparison on common features

parcelid consistency check

Feature Engineering

Log-transform skewed numeric variables

Cap or remove extreme outliers

Encode categorical codes (e.g. region, land-use)

Modeling & Tuning

Split features (X) and target (logerror)

Use RandomizedSearchCV with 5-fold CV to tune XGBoost and LinearRegression

Evaluate best models on MAE of log-error

**Usage**
Open the notebook in Colab.

Mount your Google Drive (if needed) and adjust file paths.

Run all cells in order.

Inspect the outputs, plots, and final best-model parameters.

Fork or clone to experiment with additional models, features, or external data.

**Contributing**
Contributions are welcome! If you’d like to:

Fork the repo

Create a new branch (git checkout -b feature/your-feature)

Commit your changes (git commit -m "Add some feature")

Push to the branch (git push origin feature/your-feature)

Open a Pull Request

**License**
This project is licensed under the Apache License. See the LICENSE file for details.

**Created by Your AletiAdarsh – feel free to reach out via GitHub Issues with questions or suggestions.**


Questions or suggestions? Open an issue via GitHub Issues.
