# Bike Lane Usage Analysis in Vancouver

## Project Overview

This project analyzes bike lane usage in Vancouver, focusing on the impact of weather conditions on cycling patterns. Given Vancouver's high precipitation rates and reliance on vehicle infrastructure, the project aims to determine if reallocating vehicle lanes for bike lanes is effective year-round in a city with such weather conditions. The analysis explores how weather factors influence bike lane usage and develops a predictive model to assess usage patterns.

## Objectives

- Explore how weather conditions (e.g., temperature, precipitation) affect bike lane usage in Vancouver.
- Build a predictive model to forecast bike lane usage based on weather data.
- Evaluate if reallocating vehicle lanes for bike lanes is effective, considering Vancouver's climate.

## Data Sources

- **Weather Data**: Includes daily temperature, precipitation, and other weather-related metrics.
- **Bike Lane Usage Data**: Contains records of bike lane usage across various locations in Vancouver.

Data was preprocessed and cleaned to ensure accuracy. Outliers and irrelevant data points were removed, and day-of-week dummy variables were added for categorical analysis.

## Methodology

The analysis uses the following methods and models:
- **Generalized Additive Model (GAM)**: To capture the nonlinear relationship between bike usage and weather variables.
- **Principal Component Analysis (PCA)**: For dimensionality reduction, identifying the primary factors influencing bike usage patterns.

## Key Findings

### Weather Impact on Bike Usage:

* **Temperature:** Higher temperatures are strongly correlated with increased bike lane usage, with Saturdays experiencing a more pronounced effect compared to weekdays.
* **Precipitation:** Rain and snow significantly reduce bike lane usage, which is particularly relevant given Vancouver's high annual precipitation rates (40-44% of days since 2021). This raises questions about the year-round practicality of reallocating vehicle lanes to bike lanes in a city with such weather conditions.

### Model Performance:

* The Generalized Additive Model (GAM) demonstrated strong predictive accuracy across most bike lanes, effectively capturing the key factors driving usage. However, the model underestimated bike lane usage during high-traffic periods.

### Peak Usage Patterns:

* Tourist-Heavy Lanes: Lanes near areas such as the Seawall, Kitsilano Beach, and Lions Gate Bridge at Spirit Trail showed higher-than-expected usage during peak seasons. This underestimation could potentially be influenced by increased tourist activity or other seasonal factors, though further analysis is needed to confirm this hypothesis.
* Weekday vs. Weekend Trends: Bike lane usage tends to increase Saturdays compared to weekdays, indicating that bike lanes might be underutilized during weekday rush hours when vehicular traffic is typically higher.

### Complex Predictor Relationships:

* Nonlinear Effects: Snow and cooling degree days exhibited nonlinear relationships with bike usage.
* Interaction Terms: The interaction between temperature and day of the week revealed that higher temperatures drive greater bike usage on Saturdays, suggesting a stronger recreational cycling pattern on weekends.

### Potential Model Improvements:

* Incorporating variables such as commuting patterns, time-of-day effects, infrastructure quality, and neighborhood demographics could help explain usage patterns more accurately, especially in non-tourist lanes.
* Including data on biking culture and lane quality could improve the model’s ability to capture peak usage trends in specific areas.

### Urban Planning Implications:

The findings suggest that dedicating vehicle lanes to bike lanes may be less effective during certain seasons. A more balanced approach, integrating bike infrastructure with public transit and other complementary transportation options, could better support urban transportation planning in Vancouver.

## Installation and Usage

### Prerequisites

The project requires Python 3.8+ and the following Python libraries:

- `pandas`
- `numpy`
- `matplotlib`
- `pygam`
- `scikit-learn`

### Setup Instructions

1. Clone the repository.
   ```bash
   git clone https://github.com/dshan805/bike_lane_usage.git
   cd bike-lane-usage-vancouver
