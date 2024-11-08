Here’s a concise GitHub README summary for your project based on the details from the paper:

---

# Oil Production Prediction Using Time Series Forecasting and Machine Learning Techniques

This project provides a comparative analysis of time series forecasting and machine learning models for predicting oil production, particularly in the context of the Volve production field in Norway. The goal is to build an accurate and robust model that can assist production engineers in optimizing extraction processes and managing resources effectively.

## Overview

Oil production forecasting is essential for planning in the oil and gas industry. Traditional methods, including mathematical models and empirical correlations, often lack precision due to complex factors impacting production. With advancements in artificial intelligence and data analytics, machine learning (ML) has become a viable alternative, offering enhanced prediction accuracy. This project explores various models, including time series models (ARIMA, Prophet) and machine learning algorithms (Random Forest, CatBoost, XGBoost), to improve production forecasting.

## Methodology

The dataset comprises daily production records from 2007 to 2016, divided into a training set (70%) and a test set (30%). After initial data cleaning and feature selection, the project tested and compared several models:

1. **Time Series Models**: 
   - **ARIMA** and **Prophet** were used for univariate analysis but showed limited accuracy, with high error margins and negative R² scores.
   
2. **Machine Learning Models**:
   - **Random Forest**, **CatBoost**, and **XGBoost** algorithms were trained on multivariate data, incorporating additional features like bottom-hole pressure, temperature, annulus pressure, choke size, and tubing downhole pressure.
   - Feature selection and model tuning were conducted to refine the prediction accuracy further.

3. **Stacked Ensemble Model**:
   - Combining the strengths of each ML model, a stacked regressor with XGBoost, CatBoost, and Random Forest as base models provided the most accurate predictions, achieving an R² score of 97.5% and a low mean absolute error.

## Key Findings

The results indicate that machine learning models significantly outperform traditional time series forecasting methods for oil production prediction. The inclusion of additional production factors improved accuracy and reliability, highlighting the limitations of univariate time series models in capturing complex production dynamics. The stacked ensemble model demonstrated superior accuracy across all metrics, making it a promising tool for industry applications.

## Conclusion

This project demonstrates the potential of machine learning for precise oil production forecasting. By incorporating multiple influencing factors and using ensemble techniques, production predictions can be made more accurately, supporting operational and strategic decision-making in the oil and gas industry.

## Keywords

- Time Series Forecasting
- Machine Learning
- Oil Production Prediction
- ARIMA, Prophet, XGBoost, CatBoost, Random Forest
