# future_ml_01 : Sales Forecasting

![Python](https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge)

> Retail sales forecasting on the Superstore dataset, results presented in a way that makes sense to a business owner, not just a model score.

---

## Overview

A simple end-to-end sales forecasting project built as part of the **Future Interns Machine Learning Internship (Task 1)**. It cleans raw order data, engineers time-based features, trains and compares Linear Regression and Random Forest models, and outputs charts and a plain-language business summary covering inventory, staffing, and cash flow planning.

---

## Features

| Feature | Description |
|---|---|
| Data Cleaning | Parses dates, removes duplicates, handles missing values, derives profit margin and shipping days |
| Feature Engineering | Month, quarter, lag sales (1/3/12 months), rolling averages (3M/6M), cyclical month encoding |
| Model Training | Trains and compares Linear Regression and Random Forest; selects best by RMSE |
| Evaluation | MAE, RMSE, MAPE, R² with residual analysis and per-month error breakdown |
| Visualizations | Monthly trend, actual vs predicted, error distribution, category and region breakdowns |
| Business Report | Forecast output framed as inventory, staffing, and cash flow recommendations |

---

## Tech Stack

```
Language    : Python 3.10+
Environment : Jupyter Notebooks
ML          : scikit-learn (LinearRegression, RandomForestRegressor)
Data        : Pandas, NumPy
Viz         : Matplotlib, Seaborn
Dataset     : Sample Superstore — Kaggle
```

---

## Getting Started

### Installation

```bash
# 1. Clone the repo
git clone https://github.com/glikith/future_ml_01.git
cd future_ml_01

# 2. Install dependencies
pip install -r requirements.txt
```

### Dataset

Download the dataset from Kaggle and place it in the `data/` folder:

[https://www.kaggle.com/datasets/vivek468/superstore-dataset-final](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)


### Run

Execute the notebooks in order:

```
1. data_cleaning.ipynb
2. model_training.ipynb
3. visualization.ipynb
```

---

## How It Works

```
Raw Superstore CSV (data/)
          |
          v
data_cleaning.ipynb
— parse dates, drop duplicates, fix dtypes
— derive profit margin, shipping days
          |
          v
model_training.ipynb
— aggregate to monthly sales
— engineer lag, rolling, cyclical features
— train Linear Regression + Random Forest
— evaluate with MAE, RMSE, MAPE, R²
          |
          v
visualization.ipynb
— forecast vs actual chart
— monthly sales trend
— error distribution
— business summary output
          |
          v
outputs/
— predictions.csv
— forecast charts
— business report
```

---

## Output

The final output includes:

- Forecast vs actual sales comparison chart
- Monthly sales trend chart (2014–2017)
- Error distribution chart
- A plain-language business summary on how the forecast applies to inventory planning, staffing, and cash flow management

---

## Author

[Gummadi Likith](https://github.com/glikith)

Built as part of the **Future Interns Machine Learning Internship - Task 1**.
