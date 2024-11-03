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
   git clone https://github.com/dshan805/bike-lane-usage-vancouver.git
   cd bike-lane-usage-vancouver
