# Integrating Ground-Based and Satellite Data for Station-Level Air Quality Index (AQI) Prediction in Delhi

A machine learning project for predicting station-level Air Quality Index (AQI) in Delhi by integrating ground-based pollution data from the Central Pollution Control Board (CPCB) with satellite-derived vegetation data (Sentinel-2 NDVI). The project evaluates multiple regression and classification models to support air quality monitoring and policy-driven decision making.

---

## Project Overview

This project combines environmental monitoring, geospatial analysis, and machine learning to predict AQI at monitoring stations across Delhi.

Key objectives include:

- Integrating ground-based CPCB air quality data with Sentinel-2 NDVI.
- Predicting continuous AQI values using regression models.
- Predicting CPCB AQI categories using classification models.
- Analysing the relationship between vegetation (NDVI) and air quality.
- Comparing multiple machine learning algorithms for predictive performance.

---

## Dataset

**Ground-based data**
- Central Pollution Control Board (CPCB)
- 37 monitoring stations across Delhi
- Daily pollutant observations (2017–2024)

**Satellite data**
- Sentinel-2 imagery
- NDVI extracted using Google Earth Engine

---

## Machine Learning Models

### Regression
- Ridge Regression
- Random Forest
- XGBoost
- LightGBM
- Support Vector Regression (SVR)
- Decision Tree + Grey Wolf Optimisation (DT-GWO)

### Classification
- Logistic Regression
- Random Forest
- XGBoost

---

## Key Results

### Regression

- **Best Model:** Random Forest
- **Test RMSE:** **25.33**
- **Test R²:** **0.949**

### Classification

- **Highest Accuracy:** XGBoost (**82.3%**)
- **Best Balanced Accuracy:** Random Forest (**81.9%**)

Additional findings:

- PM₂.₅ and PM₁₀ were the strongest predictors of AQI.
- NDVI showed an overall negative correlation with AQI, indicating greener areas generally experienced better air quality.
- Ensemble models consistently outperformed linear approaches.

---

## Technologies Used

- Python
- Google Earth Engine
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- LightGBM
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## How to Run

1. Clone the repository

```bash
git clone https://github.com/alankarms/Delhi-AQI-Prediction-ML_GEE.git
```

2. Navigate to the project folder

```bash
cd Delhi-AQI-Prediction-ML-GEE
```

3. Create and activate a virtual environment (optional)

```bash
python -m venv venv
```

Activate:

**Windows**

```bash
venv\Scripts\activate
```

**macOS/Linux**

```bash
source venv/bin/activate
```

4. Install dependencies

```bash
pip install -r requirements.txt
```

5. Launch Jupyter Notebook

```bash
jupyter notebook
```

6. Open the notebooks and run the cells sequentially.

---

## Report

The complete dissertation report is included in this repository:

```
Delhi_AQI_Prediction_ML_GEE_Report.pdf
```

---

## Data Sources

- Central Pollution Control Board (CPCB)
- Sentinel-2 (Copernicus)
- Google Earth Engine

---

## Content Warning

This repository contains discussions and visualisations related to air pollution, environmental health, and public health impacts.

---

## Author

**Alankar Singh**

MSc Data Science  
University of Exeter
