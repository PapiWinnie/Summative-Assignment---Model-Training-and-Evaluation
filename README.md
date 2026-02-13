# Crop Yield Prediction: A Comparative Study of Classical ML and Deep Learning

## 1. Project Overview

This project addresses the challenge of agricultural yield forecasting by systematically comparing Classical Machine Learning (Decision Trees, Random Forest, XGBoost) and Deep Learning architectures (Sequential and Functional API Wide & Deep networks). By leveraging environmental and management data, this study aims to provide precise, actionable insights for sustainable intensification and food security (UN SDG 2: Zero Hunger).

## 2. Dataset Description

The research utilizes the Agriculture Crop Yield Dataset, consisting of 336,776 records.

### Feature Metadata:

**Categorical Features:**
* **Region:** Geographical location (North, East, South, West)
* **Soil_Type:** Soil classification (Clay, Sandy, Loam, Silt, Peaty, Chalky)
* **Crop:** Crop species (Wheat, Rice, Maize, Barley, Soybean, Cotton)
* **Weather_Condition:** Predominant climate (Sunny, Rainy, Cloudy)
* **Fertilizer_Used / Irrigation_Used:** Binary indicators of management practices

**Continuous Features:**
* **Rainfall_mm:** Precipitation levels
* **Temperature_Celsius:** Mean growth temperature
* **Days_to_Harvest:** Duration from planting to maturity

**Target Variable:**
* **Yield_tons_per_hectare:** Agricultural productivity metric

## 3. Installation & Setup

To ensure reproducibility, follow these steps:

**Clone the repository:**
```bash
git clone [GITHUB_REPO_URL]
cd [REPO_NAME]
```

**Download the Data:**
* Download `crop_yield.csv` from [Kaggle][KAGGLE_DATASET_URL]
* Place the file in the root directory or update the path in the notebook:
```python
crop_yield_data = pd.read_csv('crop_yield.csv')
```

**Install Dependencies:**
```bash
pip install pandas numpy scikit-learn tensorflow xgboost matplotlib seaborn
```

## 4. Modeling Pipeline

The project follows a modular 7-experiment structure:

* **Experiment 1 & 2:** Baseline and Pre-pruned Decision Trees (Establishing bias-variance baselines)
* **Experiment 3 & 4:** Ensemble Methods (Random Forest and XGBoost for high-stability forecasting)
* **Experiment 5 & 6:** Deep Learning (Sequential API models with and without L2/Dropout regularization)
* **Experiment 7:** Wide & Deep Architecture (Functional API to combine memorization and generalization)

## 5. Key Results

| Model | MAE | R² (Test) | Generalization Gap |
|-------|-----|-----------|-------------------|
| Wide & Deep NN | 0.3997 | 0.9125 | 0.0006 |
| XGBoost | 0.4006 | 0.9126 | 0.0000 |
| Random Forest | 0.3999 | 0.9127 | 0.0028 |

Detailed analysis, including Learning Curves and Error Distributions, can be found in the [final PDF report][REPORT_PDF_URL].

## 6. Project Deliverables

* **Final Report:** [Link to PDF in Repo][REPORT_PDF_URL]
* **Presentation Video:** [Link to YouTube/Vimeo/Drive][PRESENTATION_VIDEO_URL]

## 7. Citation (IEEE Style)

[1] S. O. Attakorah, "Agriculture Crop Yield Dataset," Kaggle, 2024. [Online]. Available: https://www.kaggle.com/datasets/samuelotiattakorah/agriculture-crop-yield.

---
