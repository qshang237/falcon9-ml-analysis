# SpaceX Falcon 9 First Stage Landing Prediction

An end-to-end data science project predicting whether SpaceX Falcon 9's first stage will successfully land, enabling cost estimation for rocket launches.

## Project Overview

SpaceX advertises Falcon 9 launches at $62M — significantly cheaper than competitors — largely due to first stage reusability. This project builds a machine learning pipeline to predict landing success, using real launch data collected via the SpaceX API and web scraping.

## Pipeline

1. **Data Collection** — SpaceX REST API + web scraping
2. **Data Wrangling** — cleaning, feature engineering, label encoding
3. **Exploratory Data Analysis** — SQL queries + visual analysis
4. **Geospatial Analysis** — launch site mapping with Folium
5. **Interactive Dashboard** — built with Plotly Dash
6. **ML Prediction** — classification models with GridSearchCV tuning

## Results

| Model | Test Accuracy |
|---|---|
| Logistic Regression | **94.4%** |
| KNN | **94.4%** |
| SVM | 88.9% |
| Decision Tree | 72.2% |

Best model: **Logistic Regression** (C=0.01, L2 regularisation)

## Tech Stack

Python, Pandas, NumPy, Scikit-learn, SQL, Plotly Dash, Folium, BeautifulSoup, Requests

## Certificate

IBM Data Science Professional Certificate — [Coursera](https://www.coursera.org/professional-certificates/ibm-data-science)
