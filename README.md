# Crop Yield Prediction: A Comparative Study of Classical ML and Deep Learning

## Project Overview

This project addresses the challenge of agricultural yield forecasting by systematically comparing **Classical Machine Learning models** (Decision Trees, Random Forest, XGBoost) and **Deep Learning architectures** (Sequential and Functional API Wide & Deep networks).

By leveraging environmental and management data, this study aims to provide precise, actionable insights for sustainable agricultural intensification and food security, aligning with **UN SDG 2: Zero Hunger**.

---

## Dataset Description

The research utilizes the **Agriculture Crop Yield Dataset**, consisting of **336,776 records**.

### Feature Metadata

#### Categorical Features
- **Region**: Geographical location (North, East, South, West)
- **Soil_Type**: Soil classification (Clay, Sandy, Loam, Silt, Peaty, Chalky)
- **Crop**: Crop species (Wheat, Rice, Maize, Barley, Soybean, Cotton)
- **Weather_Condition**: Predominant climate (Sunny, Rainy, Cloudy)
- **Fertilizer_Used / Irrigation_Used**: Binary indicators of management practices

#### Continuous Features
- **Rainfall_mm**: Precipitation levels
- **Temperature_Celsius**: Mean growth temperature
- **Days_to_Harvest**: Duration from planting to maturity

#### Target Variable
- **Yield_tons_per_hectare**: Agricultural productivity metric

---

## Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/[Your-Username]/[Your-Repo-Name].git
cd [Your-Repo-Name]
