# 🌾 Indian Crop Production Analysis & Prediction

An end-to-end Agriculture Analytics and Machine Learning project that transforms Indian agricultural data into meaningful insights using **Python, Scikit-learn, and Power BI**.

This project demonstrates the complete data analytics and machine learning workflow—from data cleaning and exploratory analysis to interactive dashboard development and crop production prediction.

---

# 📌 Project Overview

The objective of this project is to analyze Indian agricultural production data to uncover state-wise, crop-wise, season-wise, and year-wise production patterns and predict crop production using Machine Learning.

The project includes:

- Data Cleaning using Python
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Data Visualization
- Machine Learning using Random Forest Regression
- Interactive Power BI Dashboard
- Model Evaluation

---

# 📂 Dataset

**Dataset:** Indian Agriculture Crop Production Dataset

The dataset contains **246,091 records** and **7 columns** related to agricultural production.

The dataset contains:

- State Name
- District Name
- Crop Year
- Season
- Crop
- Area
- Production

After handling missing values in the `Production` column, **242,361 records** were retained for analysis.

An additional feature was created during preprocessing:

- Yield

### Yield Calculation

    Yield = Production / Area

---

# 🛠️ Tools & Technologies

| Tool / Technology | Purpose |
|-------------------|---------|
| Python | Data Cleaning & Analysis |
| Pandas | Data Manipulation |
| NumPy | Numerical Operations |
| Matplotlib | Data Visualization |
| Seaborn | Exploratory Visualization |
| Scikit-learn | Machine Learning |
| Random Forest Regressor | Crop Production Prediction |
| Power BI | Dashboard Development |
| DAX | Measures & KPIs |
| Jupyter Notebook | Development & Analysis |

---

# 🔄 Project Workflow

    Raw Agricultural Data
            ↓
    Data Cleaning & Preprocessing
            ↓
    Exploratory Data Analysis
            ↓
    Feature Engineering
            ↓
    Data Visualization
            ↓
    Power BI Dashboard
            ↓
    Machine Learning
            ↓
    Model Evaluation
            ↓
    Agricultural Insights

---

# 🐍 Python Analysis

Python was used for data cleaning, preprocessing, exploratory analysis, feature engineering, and visualization.

### Data Cleaning

- Checked dataset structure and data types
- Examined missing values
- Removed records with missing `Production` values
- Checked for duplicate records
- Removed records where `Area` was not positive
- Created `Yield` feature
- Prepared categorical variables for Machine Learning

### Exploratory Data Analysis

- State-wise Production Analysis
- Crop-wise Production Analysis
- Year-wise Production Trends
- Season-wise Production Analysis
- Area vs Production Analysis
- State-wise Average Yield
- State vs Crop Production Analysis
- Crop Yield Distribution

---

# 🤖 Machine Learning

A **Random Forest Regression** model was developed to predict crop production.

### Features Used

- State Name
- Crop
- Season
- Crop Year
- Area

Categorical variables were encoded using **LabelEncoder**.

The target variable was log-transformed before model training:

    y = np.log1p(df['Production'])

A sample of **50,000 records** was used for Machine Learning.

The data was divided into:

- 80% Training Data
- 20% Testing Data

---

# 🌲 Random Forest Regression

The Machine Learning model used was **Random Forest Regressor**.

### Model Parameters

| Parameter | Value |
|-----------|-------|
| `n_estimators` | 50 |
| `max_depth` | 10 |
| `n_jobs` | -1 |
| `random_state` | 42 |

---

# 📏 Model Evaluation

The model was evaluated using:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

### Results

| Metric | Score |
|--------|------:|
| MAE | 0.66 |
| MSE | 0.93 |
| RMSE | 0.96 |
| **R² Score** | **0.91** |

The Random Forest Regression model achieved an **R² score of 0.91** on the test data.

---

# 📊 Power BI Dashboard

The project contains an interactive Power BI dashboard for analyzing agricultural production and yield patterns.

### Dashboard Features

- KPI Cards
- State-wise Production
- Crop-wise Production
- Year-wise Production Trends
- Season-wise Analysis
- State-wise Yield Analysis
- Crop Performance Analysis
- Interactive Filters and Slicers

---

# 📸 Dashboard Preview

## 🌾 Crop Production Dashboard

![Crop Production Dashboard](dashboard/Crop_Production_Dashboard.png)

---

## 📈 Agricultural Analysis Dashboard

![Agricultural Analysis Dashboard](dashboard/Agricultural_Analysis.png)

---

# 📈 Key Insights

### Production Insights

- A small number of states contribute significantly to overall agricultural production.
- Crop production varies considerably across states and years.
- Different crops show significant differences in production levels.

### Agricultural Insights

- Cultivated area has a positive relationship with production.
- Average yield varies across states and crops.
- Different states show specialization in particular crops.
- Crop production patterns vary across agricultural seasons.

### Machine Learning Insights

- State, crop, season, crop year, and cultivated area were used as features for crop production prediction.
- The Random Forest Regression model achieved an **R² score of 0.91** on the test data.

---

# 🎯 Skills Demonstrated

- Data Cleaning
- Data Preprocessing
- Exploratory Data Analysis
- Feature Engineering
- Data Visualization
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Random Forest Regression
- Model Evaluation
- Power BI
- DAX
- Dashboard Design
- Data-driven Insight Generation

---


⭐ If you found this project helpful, consider giving it a star!
