# CropYield-Predictor-AI-Powered-Agricultural-Analytics
AI-powered agricultural analytics platform for crop yield prediction using machine learning, feature engineering, exploratory data analysis, and an interactive Streamlit dashboard.
# 🌾 CropYield Predictor

An end-to-end Data Science and Machine Learning project that predicts crop yield using environmental and agricultural factors. The project includes data cleaning, exploratory data analysis (EDA), feature engineering, model training, evaluation, and an interactive Streamlit dashboard for business insights and crop yield prediction.

---

## 📌 Project Overview

Agriculture plays a vital role in global food security. Accurate crop yield prediction helps governments, researchers, and farmers optimize production, improve resource allocation, and make data-driven decisions.

This project analyzes agricultural datasets containing rainfall, pesticide usage, temperature, country, crop type, and historical yield records to build predictive machine learning models.

---

## 🎯 Objectives

- Perform comprehensive data cleaning and validation
- Conduct exploratory data analysis with interactive visualizations
- Engineer meaningful agricultural features
- Train and compare multiple machine learning regression models
- Evaluate models using standard regression metrics
- Build an interactive Streamlit dashboard for prediction and analytics

---

## 📊 Dataset

**Source:** Kaggle – Crop Yield Prediction Dataset

The dataset contains **28,242 agricultural records** across multiple countries and crop types.

### Features

- Area
- Item (Crop)
- Year
- Average Rainfall
- Pesticides Used
- Average Temperature
- Crop Yield (Target)

---

## 🛠 Tech Stack

### Programming

- Python 3.11

### Data Analysis

- Pandas
- NumPy

### Visualization

- Matplotlib
- Seaborn
- Plotly

### Machine Learning

- Scikit-Learn

Models Implemented

- Linear Regression
- Ridge Regression
- Lasso Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor

### Dashboard

- Streamlit

### Model Storage

- Joblib

---

## 📂 Project Structure

```
CropYield-Predictor
│
├── 01_Data_Ingestion_Validation.ipynb
├── 02_Data_Cleaning.ipynb
├── 03_Exploratory_Data_Analysis.ipynb
├── 04_Feature_Engineering.ipynb
├── 05_Model_Training_Comparison.ipynb
├── 06_Model_Evaluation.ipynb
│
├── app.py
├── best_model.pkl
├── preprocessing_pipeline.pkl
│
├── validated_crop_data.csv
├── cleaned_crop_data.csv
├── feature_engineered_crop_data.csv
├── model_results.csv
├── prediction_results.csv
│
├── README.md
├── requirements.txt
```

---

## 📈 Exploratory Data Analysis

The project includes more than **15 visualizations**, including:

- Yield Distribution
- Rainfall Distribution
- Temperature Distribution
- Pesticide Distribution
- Correlation Heatmap
- Top Countries by Crop Yield
- Top Crops
- Year-wise Crop Yield Trend
- Rainfall vs Crop Yield
- Temperature vs Crop Yield
- Pesticides vs Crop Yield
- Treemap
- Sunburst Chart
- Interactive Plotly Visualizations

---

## ⚙ Feature Engineering

Created domain-specific features including:

- Rainfall Category
- Temperature Band
- Pesticide Category
- Rainfall × Temperature Interaction
- Log Transformation of Pesticides

A Scikit-Learn preprocessing pipeline using **ColumnTransformer** and **OneHotEncoder** was implemented to prevent data leakage and ensure reproducible preprocessing.

---

## 🤖 Machine Learning

Multiple regression models were trained and compared.

Evaluation Metrics:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score
- Cross Validation

The best-performing model was exported using Joblib for deployment.

---

## 📊 Streamlit Dashboard

The dashboard provides:

- Executive KPI Dashboard
- Interactive EDA
- Crop Yield Prediction
- Model Performance
- Business Insights

---

## 📌 Key Outcomes

- Built a complete end-to-end machine learning pipeline.
- Applied feature engineering techniques for agricultural analytics.
- Compared multiple regression algorithms.
- Developed an interactive analytics dashboard.
- Produced actionable insights for crop yield prediction.

---

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/CropYield-Predictor.git
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the Streamlit application:

```bash
streamlit run app.py
```

---

## 📷 Dashboard Preview

(Add screenshots of your Streamlit dashboard here.)

---

## 👩‍💻 Author

**Vyjayanthi Punuri**

BS-MS (Computer Science & Business Management)

Data Science | Machine Learning | Business Analytics
