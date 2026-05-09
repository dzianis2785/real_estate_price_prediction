# 🏠 Real Estate Price Prediction Using Machine Learning

![](./images/data_cleaning.png)

## 📌 Project Overview

This project focuses on solving a real-world business problem for a real
estate agency --- improving the speed and accuracy of property price
evaluation.

Using machine learning techniques, the project builds predictive models
that estimate housing prices based on property characteristics,
demographic indicators, and geographic features.

The project demonstrates a full data science workflow including:

-   Data cleaning and preprocessing
-   Exploratory Data Analysis (EDA)
-   Feature engineering
-   Model training and evaluation
-   Hyperparameter tuning
-   Feature importance analysis

------------------------------------------------------------------------

# 📚 Table of Contents

1.  Project Description
2.  Data Description
3.  Exploratory Data Analysis
4.  Modeling
5.  Results
6.  Project Structure
7.  Installation
8.  Usage
9.  Author
10. Conclusions

------------------------------------------------------------------------

# 📖 Project Description

The goal of this project is to build a machine learning model capable of
predicting real estate prices.

Project stages:

1.  Understanding the dataset
2.  Data cleaning and handling missing values
3.  Removing noisy and irrelevant features
4.  Feature engineering and feature selection
5.  Training several regression models
6.  Selecting the best performing models
7.  Hyperparameter optimization
8.  Identifying the most influential features

### 🎯 Objectives

-   Perform exploratory data analysis and data cleaning
-   Build a predictive model for real estate prices
-   Identify key factors that influence housing prices

![](./images/example_outliers.png)

------------------------------------------------------------------------

# 🗂 Data Description

The project uses real estate market data from the United States and
Canada.

The agency required a model capable of predicting housing prices based
on:

-   property characteristics
-   residents' income levels
-   education levels of residents
-   city size
-   geographic location

The original dataset contains:

-   377,000+ real estate transactions
-   18 features including the target variable

### Geographical Data

Property locations were geocoded using the [Geopy](https://geopy.readthedocs.io/en/stable/) library.

Additional geographic information about U.S. city center coordinates was
obtained from the Geonames [GitHub](https://gist.githubusercontent.com/esjewett/635c1549ee0eee6b32acee36012763f0/raw/US_cities.csv) open geographic database. 

### Demographic Data

Socioeconomic indicators were taken from:

U.S. Census 2020
https://data.census.gov

### Datasets

All datasets used in the project can be downloaded here:

https://drive.google.com/file/d/15Do3SFiQ42AFEWoZ04Aajgh8VIpNTj3Y/view

------------------------------------------------------------------------

# 🔎 Exploratory Data Analysis

During the analysis several issues were identified:

-   Large number of missing values
-   Duplicate records
-   Outliers in numerical features
-   Strong skewness in several variables

Most numerical features follow a log-normal distribution with right
skewness.

Data cleaning included:

-   Removing duplicates
-   Handling missing values
-   Removing unrealistic property prices
-   Feature transformations

------------------------------------------------------------------------

# 🤖 Modeling

Several machine learning regression models were tested:

-   Linear Regression
-   Ridge Regression
-   Lasso Regression
-   Random Forest
-   XGBoost
-   LightGBM

Hyperparameter tuning was performed using cross-validation.

------------------------------------------------------------------------

# 📊 Results

The best performance was achieved using tree-based ensemble models.

Random Forest and Gradient Boosting Models significantly outperformed linear
models due to nonlinear relationships in the data.

The final model identified the top 10 most influential features
affecting real estate prices.

------------------------------------------------------------------------

# 📂 Project Structure

real_estate_price_prediction/

-   real_estate_price_prediction_project.ipynb
-   requirements.txt
-   README.md

------------------------------------------------------------------------

# ⚙️ Installation

``` bash
git clone https://github.com/dzianis2785/real_estate_price_prediction.git
```

Install dependencies:

``` bash
pip install -r requirements.txt
```

------------------------------------------------------------------------

# ▶️ Usage

Open the main notebook:

real_estate_price_prediction_project.ipynb

The notebook contains:

-   full analysis
-   data cleaning workflow
-   model training
-   evaluation results

------------------------------------------------------------------------

# 👤 Author

Dzianis Krauchuk

Email: dzianis2785@gmail.com\
LinkedIn: https://www.linkedin.com/in/dzianis-krauchuk-1a09b2278/

------------------------------------------------------------------------

# 📌 Conclusions

1.  The dataset contains a large amount of noise, missing values, and
    duplicates.
2.  Most numerical features follow a log-normal distribution.
3.  The original dataset alone was insufficient for building a strong
    predictive model, so it was enriched with external data sources.
4.  Ensemble models such as Random Forest and Gradient Boosting Models 
    outperform linear regression models.
5.  The data contains strong nonlinear relationships between variables.
