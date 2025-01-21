# Timeseries_Sales_Forecasting
Time series sales forecasting project for Tecos Group of Companies. Utilising machine learning to analyse historical sales data, identify trends, and build predictive models for improved business decision-making.
Time Series Sales Forecasting for Tecos Group of Companies
# Time Series Sales Forecasting for Tecos Group of Companies

![image](https://github.com/user-attachments/assets/22091c3d-1400-4edd-879f-200521a17bdc)


## Overview

This project focuses on developing an accurate time series sales forecasting model for Tecos Group of Companies, a British multinational retailer. Leveraging machine learning techniques, the project aims to predict future sales trends based on historical data to assist in strategic decision-making, inventory management, and revenue optimization.

## Project Objectives

* **Sales Trend Prediction**: Develop robust forecasting models to project future sales across various time horizons.

* **Pattern Recognition**: Identify seasonal trends, cyclic patterns, and key factors influencing sales.

* **Data-Driven Decision Making**: Equip stakeholders with actionable insights to optimise sales operations.

* **Model Evaluation and Optimization**: Compare multiple forecasting techniques to ensure the most accurate predictions.

  ![image](https://github.com/user-attachments/assets/09bea250-96db-4dd3-8ffb-414d4a6c60c9)


## Business Problem

Tecos Group of Companies has encountered challenges in predicting sales patterns due to fluctuating market demand, seasonality, and customer preferences. The goal of this project is to implement reliable forecasting models that can aid the company in improving:

* Demand planning and inventory management.
* Revenue growth through accurate forecasting.
* Resource allocation and budgeting.

## Dataset Overview

The dataset consists of historical sales records containing various attributes essential for analysis.

### Key Columns:

| Column Name | Description |
|-------------|-------------|
| Order Date | Date and time of the sales transaction |
| Region | Geographical sales region |
| Customer Segment | Customer type (e.g., Consumer, Small Business) |
| Product Category | Category of product sold |
| Units Sold | Number of units sold |
| Unit Price | Price per unit |
| Revenue | Total revenue generated |
| Profit Margin | Profit margin percentage |

## Approach and Methodology

### 1. Data Preprocessing

* Data cleaning: Handling missing values and duplicate records.
* Feature engineering: Creating time-based features (e.g., month, year, quarter).

### 2. Exploratory Data Analysis (EDA)

* Sales trends analysis.
* Seasonal decomposition to identify underlying patterns.
* Correlation analysis to determine factors affecting sales.

### 3. Model Development

The project explores multiple time series forecasting models, including:

**Traditional Models:**
* Autoregressive Integrated Moving Average (ARIMA)
* Exponential Smoothing (Holt-Winters)

**Machine Learning Approaches:**
* Facebook Prophet (for weekly and monthly sales forecasting)
* Long Short-Term Memory (LSTM) Networks

### 4. Model Evaluation

Performance metrics used to assess model accuracy:

* Mean Absolute Error (MAE): Measures average error in prediction.
* Root Mean Squared Error (RMSE): Penalizes large errors more than MAE.
* Mean Absolute Percentage Error (MAPE): Evaluates the percentage error relative to actual values.

## Visualization

* Sales trend visualisation with line and bar charts.
* Interactive dashboards showcasing sales performance.
* Heatmaps to detect regional and category-wise sales trends.
  ## Model Selection and Performance

### Weekly Forecasting: LSTM Metrics

Our analysis shows that LSTM Weekly Metrics provides optimal performance for short-term forecasting. The model achieved consistent MAPE (Mean Absolute Percentage Error) values across categories:

* **Electronics**: 15.84% MAPE
* **Furniture**: 13.84% MAPE
* **Office Supplies**: 16.25% MAPE

### Monthly Forecasting: Exponential Smoothing (ES)

For long-term predictions, Exponential Smoothing demonstrated superior performance with low MAPE values:

* **Electronics**: 11.28% MAPE
* **Office Supplies**: 11.73% MAPE
* **Furniture**: 15.70% MAPE

## Performance Evaluation

### Why MAPE as Key Metric?

MAPE (Mean Absolute Percentage Error) was chosen as the primary evaluation metric for several reasons:

* **Business Interpretability**: Percentage-based metric that's easily communicated to stakeholders
* **Scale Independence**: Enables meaningful comparisons across different product categories
* **Error Weighting**: Effectively penalizes large prediction deviations
* **Industry Standard**: Widely adopted in demand forecasting applications

### Model Comparison

#### Alternative Models Considered

1. **Holt-Winters (ES Weekly)**
   * Electronics: 16.81% MAPE
   * Furniture: 15.81% MAPE
   * Office Supplies: 16.96% MAPE
   * *Verdict*: Slightly higher MAPE values compared to LSTM Weekly

2. **Prophet**
   * Weekly Forecasts: 17.82% MAPE
   * Monthly Forecasts: 26.81% MAPE
   * *Verdict*: Moderate performance for weekly, poor for monthly forecasts

3. **ARIMA**
   * Weekly MAPE Range: 21.77% - 22.83%
   * *Verdict*: Struggles with seasonal patterns, higher error rates

## Implementation Guidelines

### Weekly Forecasting Implementation

**Selected Model**: LSTM Weekly Metrics

**Key Benefits**:
* Lowest MAPE values across all product categories
* Strong pattern recognition capabilities
* Robust generalization performance

### Monthly Forecasting Implementation

**Selected Model**: Exponential Smoothing (ES) Monthly Metrics

**Key Benefits**:
* Consistent performance across major categories
* Computationally efficient
* Excellent handling of seasonal patterns

## Business Impact

### Operational Benefits

* **Improved Accuracy**: Enhanced demand planning and inventory optimization
* **Granular Insights**: 
  * Weekly trends through LSTM
  * Monthly patterns through ES
* **Efficient Implementation**: 
  * LSTM for complex pattern recognition
  * ES for straightforward deployment

### Strategic Advantages

* **Data-Driven Decisions**: Informed choices for pricing and promotions
* **Resource Optimization**: Better allocation of inventory and staff
* **Risk Management**: Reduced forecasting errors across categories

## Future Enhancements

* Incorporation of external economic factors for better forecasting.
* Deployment of models via cloud platforms (AWS, Azure).
* Development of an automated retraining pipeline.

## Contribution Guidelines

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes with meaningful messages.
4. Submit a pull request for review.

## Contact

For further inquiries or collaboration, please reach out via:

* Email: eneojaide@gmail.com
* LinkedIn: www.linkedin.com/in/ene-ojaide

