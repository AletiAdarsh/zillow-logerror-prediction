Zillow Log-Error Prediction

A Colab-based pipeline for predicting Zillow’s Zestimate log-error using EDA, feature engineering, and hyperparameter-tuned models (XGBoost & LinearRegression).

Open in Colab

Table of Contents

Project Overview

Repository Structure

Getting Started

Prerequisites

Install Dependencies

Pipeline Breakdown

Data Loading

Exploratory Data Analysis (EDA)

Data Cleaning

Dataset Comparison

Feature Engineering

Modeling & Tuning

Usage

Contributing

License

Contact

Project Overview

This project tackles the Zillow Prize challenge of predicting the log-error in Zillow’s home-value estimates (Zestimates). It runs entirely in Google Colab and demonstrates:

Data Loading & Inspection

Exploratory Data Analysis (EDA)

Data Cleaning & Missing-Value Handling

Feature Engineering & Transformations

Model Training & Hyperparameter Tuning

Result Interpretation & Next Steps

Repository Structure

zillow-logerror-prediction/
├── ZXTRN_HOUSING_DATA.ipynb   # Main Colab notebook
├── README.md                  # Project overview & instructions
├── requirements.txt           # Python dependencies
└── .gitignore                 # Files to ignore in Git

Getting Started

Prerequisites

Google account for Colab

GitHub account to fork or clone the repo

(Optional) Local Python environment if you wish to run outside Colab

Install Dependencies

pip install -r requirements.txt

Pipeline Breakdown

Data Loading

Load properties_2016.csv, properties_2017.csv, train_2016_v2.csv, train_2017.csv, and sample_submission.csv.

Exploratory Data Analysis (EDA)

Print shapes & dtypes

List & plot missing-value percentages

Plot histograms of all numeric features

Data Cleaning

Drop columns with >80% missing

Dataset Comparison

Compare schema of shared vs. unique columns

Compare summary statistics of common features

Check parcelid consistency

Feature Engineering

Log-transform skewed variables

Cap/remove extreme outliers

Encode categorical codes

Modeling & Tuning

Split features (X) and target (log-error)

Use RandomizedSearchCV (5-fold) to tune XGBoost & LinearRegression

Evaluate best models using Mean Absolute Error (MAE)

Usage

Open the notebook in Colab.

Mount Google Drive (if needed) and adjust file paths.

Run all cells.

Inspect outputs & best-model parameters.

Fork or clone to extend.

Contributing

Contributions welcome!

Fork the repo

Create a branch: git checkout -b feature/your-feature

Commit your changes: git commit -m 'Add feature: description'

Push and open a pull request

License

This project is licensed under the Apache License 2.0.

Contact

Created by AletiAdarsh.Questions or suggestions? Open an issue via GitHub Issues.
