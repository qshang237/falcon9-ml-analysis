# SpaceX Falcon 9 First Stage Landing Prediction

A data science project predicting whether SpaceX Falcon 9's first stage will successfully land, enabling cost estimation for rocket launches.

## Project Overview

SpaceX advertises Falcon 9 launches at $62M, significantly cheaper than competitors, largely due to first stage reusability. This project collects real launch data from the SpaceX API, analyses the launch records with SQL, shows them in an interactive dashboard, and trains classification models to predict landing success.

## Contents

1. **Data Collection**: SpaceX REST API, with basic data wrangling (`notebooks/01_data_collection_api.ipynb`)
2. **Exploratory Data Analysis**: SQL queries (`notebooks/02_eda_sql.ipynb`)
3. **Interactive Dashboard**: built with Plotly Dash (`app/spacex_dash_app.py`)
4. **ML Prediction**: classification models with GridSearchCV tuning (`notebooks/03_ml_prediction.ipynb`)

The SQL analysis and the prediction notebook load the prepared datasets of the course from the course server. The dashboard reads `spacex_launch_dash.csv`, the prepared course dataset, which is not included in this repository.

## Results

| Model | Test Accuracy |
|---|---|
| Logistic Regression | **94.4%** |
| KNN | **94.4%** |
| SVM | 88.9% |
| Decision Tree | 72.2% |

Best model: **Logistic Regression** (C=0.01, L2 regularisation)

## Tech Stack

Python, Pandas, NumPy, Scikit-learn, SQL, Plotly Dash, Requests

## Certificate

IBM Data Science Professional Certificate ([Coursera](https://www.coursera.org/professional-certificates/ibm-data-science))
