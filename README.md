# Birth-Rate_timeseries-analysis
male vs female
Birth Rate Time Series Forecasting
## Overview

I wanted to explore how birth rates in the US have changed over time, and use it as an opportunity to compare a few different forecasting approaches head-to-head on the same data. This project analyzes daily/monthly birth counts (by gender) and builds forecasting models using SARIMA , XGBoost , and Prophet to see which technique handles the underlying trend and seasonality best.

## Data Source

Data comes from the CDC's National Center for Health Statistics (NCHS): https://www.cdc.gov/nchs/data_access/Vitalstatsonline.htm

The dataset includes daily birth records from 1969–1988 and monthly aggregated totals from 1989–2008, broken down by gender (male/female).

## Project Structure
Data Cleaning — handling invalid calendar dates, separating daily vs. monthly granularity
Exploratory Data Analysis — full-history trends, yearly totals, day-of-week and monthly seasonality, seasonal decomposition
Forecasting Models — SARIMA, XGBoost, and Prophet, trained and evaluated separately for male and female birth series
Model Comparison — MAE/RMSE across all three models
## Key Findings
Birth counts show clear weekly seasonality (lower on weekends) and long-term trend shifts across the full 1969–2008 period.
Of the three models tested, XGBoost produced the lowest error (MAE/RMSE) for both male and female series, outperforming Prophet and SARIMA.
Model performance was consistent in ranking across both genders, suggesting the result isn't specific to one series.
## Tools Used

pandas· · numpy· matplotlib· seaborn· statsmodels· xgboost·prophetscikit-learn

## About Me

Hi, I'm Monica,  a data scientist based in Toronto . I'm passionate about digging into messy, real-world datasets and figuring out what story they're actually telling. Time series and forecasting problems are a particular favorite of mine, there's something satisfying about testing multiple approaches against each other and seeing which one actually earns its keep on the data, rather than assuming a fancier model automatically wins.
