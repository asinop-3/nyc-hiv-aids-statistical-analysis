# NYC HIV & AIDS Statistical Analysis (2016–2021)

## Overview
This project analyzes HIV and AIDS diagnoses in New York City using publicly available data from NYC Open Data. The goal is to understand how diagnosis rates vary over time, across boroughs and neighborhoods, and among demographic groups, while applying statistical inference and predictive modeling techniques.

The analysis combines exploratory data analysis, hypothesis testing, regression modeling, and machine learning methods to identify persistent disparities and evaluate how well different modeling approaches capture patterns in public health data.

## Data
The dataset was sourced from **NYC Open Data** (https://tinyurl.com/yxby8nu2) and published by the NYC Department of Health and Mental Hygiene (DOHMH). It contains yearly records of HIV and AIDS diagnoses across New York City, including:

- Diagnosis counts and rates per 100,000 population  
- Borough and neighborhood geography  
- Sex and race/ethnicity  
- Concurrent HIV/AIDS diagnoses (late-stage detection)

Due to reporting gaps, the primary analysis focuses on **2016–2021**.

## Methods & Techniques

### Exploratory Data Analysis
- Time trends in HIV and AIDS diagnosis rates  
- Borough- and neighborhood-level comparisons  
- Demographic disparities by sex and race/ethnicity  
- Distributional analysis using boxplots and histograms  
- Geographic pattern exploration across NYC  

### Statistical Inference
- One-sample t-test (COVID-era drop in diagnoses, 2020)  
- Paired t-test (Bronx vs. NYC-wide rates)  
- Two-sample Welch t-test (late-stage diagnoses in Queens)  

### Modeling
- Linear and polynomial regression for trend analysis  
- Borough- and neighborhood-level regression models  
- Decision tree regression (interpretability-focused)  
- Random forest regression with cross-validation  
- Model evaluation using MAE, RMSE, and R²  

## Key Findings
- HIV and AIDS diagnoses declined overall from 2016–2019, with a sharp dip in 2020 and rebound in 2021 likely driven by pandemic-related testing disruptions.
- The Bronx consistently exhibits the highest HIV and AIDS diagnosis rates across boroughs.
- Black and Latino/Hispanic populations experience disproportionately higher diagnosis rates.
- Males have consistently higher HIV diagnosis rates than females.
- Tree-based models outperform linear models in predictive accuracy, highlighting the importance of neighborhood and demographic factors.
- Extreme high-rate neighborhoods are difficult to predict accurately due to data sparsity.

## Files in This Repository
- **Final code** contains the complete, cleaned analysis submitted for the course.
- **Final report (PDF)** presents results, interpretation, and conclusions in a formal write-up.

## Reproducibility
The analysis was conducted in **R** using common statistical and data science libraries, including:
- tidyverse
- ggplot2
- rpart
- randomForest
- caret

All data sources are public and documented above.

## Limitations & Future Work
- Limited number of years restricts time-series reliability.
- Sparse data in some neighborhoods and demographic groups affects model accuracy.
- Tree-based models underpredict rare, high-burden cases.

Future extensions could include:
- Additional years of data
- Socioeconomic and access-to-care variables
- Spatial or gradient boosting models
- More formal forecasting frameworks

## Authors
Fahim Ahamed  
Anthony Sinopoli  
Fatima Nasyr  

*Listed alphabetically*
