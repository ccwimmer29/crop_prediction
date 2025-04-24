# 🌾 Crop Yield Prediction Using Machine Learning

## Overview

This project aims to develop a machine learning solution for **accurate and scalable crop yield forecasting**. Farmers face significant uncertainty due to variable weather, soil quality, and climate change. Our models aim to **optimize agricultural strategies**, enhance **resource allocation**, and **reduce financial losses**—potentially saving up to $15 per hectare per season.

## 👥 Team

Vincent Chirio • Sourendu Saha • Cat Wimmer • Leon Tan  
*Machine Learning I | Dr. Gizem Agar | March 2025*

## 📊 Business Objective

- Improve forecast accuracy for crop yields.
- Optimize water, fertilizer, and labor use.
- Provide insights into yield-influencing features.
- Support long-term, climate-resilient agricultural planning.

## 🔍 Data

- **Source**: Kaggle, FAO, World Bank  
- **Size**: ~28,000 rows × 8 columns  
- **Years Covered**: 1990–2013  
- **Geographic Scope**: 101 countries  
- **Features**:
  - Crop yield (hg/ha)
  - Rainfall and temperature averages
  - Pesticide usage
  - Crop type and country

## 📈 Exploratory Data Analysis

- **Transformations**: Log-scaling, standard scaling, outlier removal
- **Feature Engineering**: Interactions, quadratic terms, and log transformations
- **Visualization**: PCA, clustering, and climate-yield heatmaps
- **Clustering**: K-Means grouped countries by climate zones

## 🔬 Modeling Strategy

- **Baseline**: Linear Regression  
- **Advanced Models**:
  - Support Vector Regression (SVR)
  - Random Forest Regressor
  - Gradient Boosting Regressor

> Models were evaluated using **R²**, **RMSE**, and **MAPE**, with hyperparameters tuned using Grid Search. Overfitting was mitigated through train-validation-test splits and data leakage prevention.

### 📊 Performance Summary (Test Set)

| Model                 | R²   | RMSE     | MAPE  |
|----------------------|------|----------|-------|
| Linear Regression     | 0.78 | 40,205   | 38%   |
| Support Vector Reg.   | 0.97 | 13,730   | 8.7%  |
| Gradient Boosting     | 0.96 | 17,529   | 29%   |
| Random Forest         | 0.98 | 11,264   | 16%   |

## 🚀 Deployment & Monitoring

- **Repository**: Public on GitHub for reproducibility
- **Updates**: Manual yearly dataset refresh and model retraining
- **Monitoring**: K-S statistic for data drift detection

## ✅ Key Takeaways

- **Random Forest** achieved the lowest RMSE
- **SVR** had the best MAPE
- **Model outputs help inform agricultural planning**, support climate resilience, and promote data-driven food security strategies

## ⚖️ Ethical Considerations

- Regional bias due to underrepresented areas
- Inequity in tool accessibility across farm sizes
- Reliance on historical data may limit future climate adaptability

## 📚 References & Data

- Paudel et al., 2021 – *Machine learning for large-scale crop yield forecasting* ([DOI](https://doi.org/10.1016/j.agsy.2020.103016))
- Kaggle Dataset: [Crop Yield Prediction Dataset](https://www.kaggle.com/datasets/patelris/crop-yield-prediction-dataset/data)
