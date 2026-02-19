# 🏠 UAE Real Estate Price Prediction

## 📌 Overview
A complete end-to-end machine learning project that analyzes 
and predicts real estate prices across UAE cities using 41,000+ 
property listings sourced from Bayut.com. The project covers 
data exploration, preprocessing, and predictive modeling in a 
single notebook to uncover key pricing factors in the UAE 
property market.

## 📊 Dataset
- **Source:** Bayut.com via Kaggle
- **Size:** 41,381 property listings
- **Cities:** Dubai, Abu Dhabi, Sharjah and more
- **Features:** Price, type, location, beds, baths,
  furnishing, completion status, area name, coordinates

## 📒 What's Inside the Notebook
The notebook is structured in the following order:

**Stage 1 — Data Loading & Overview**
Loading the dataset and reviewing its shape, columns, 
data types, and basic statistics.

**Stage 2 — Exploratory Data Analysis (EDA)**
Visual exploration of price distributions, city comparisons, 
property types, furnishing impact, completion status, 
bedroom/bathroom trends, top expensive areas, 
and monthly listing trends.

**Stage 3 — Data Preprocessing**
Handling zero values, missing data, outlier removal, 
log transformation of price, encoding categorical variables, 
feature engineering from dates, and feature scaling.

**Stage 4 — Model Training**
Three models trained and compared: Linear Regression 
(baseline), XGBoost, and Random Forest.

**Stage 5 — Model Evaluation**
R², RMSE, MAE comparison, actual vs predicted plots, 
feature importance analysis, residual analysis, 
overfitting check, and single property prediction test.

**Stage 6 — Interpretations & Conclusions**
Short written interpretations are provided at the very 
end of the notebook summarizing all key findings from 
EDA, preprocessing decisions, and model results.
> 📌 Viewer Note: Scroll to the bottom of the notebook
> to read the full interpretation of all analysis.

## 🤖 Models Trained & Results

| Model             | R² Score   | RMSE       | MAE        |
|-------------------|------------|------------|------------|
| **Random Forest** | **0.9564** | **0.1813** | **0.1210** |
| XGBoost           | 0.9553     | 0.1836     | 0.1283     |
| Linear Regression | 0.8654     | 0.3183     | 0.2397     |

## 🏆 Best Model: Random Forest
| Metric          | Value          |
|-----------------|----------------|
| Train R²        | 0.9772         |
| Test R²         | 0.9564         |
| Overfitting Gap | 0.0209 ✅ None |
| Average Error   | 12.13%         |

### Single Property Prediction Test
| Metric          | Value         |
|-----------------|---------------|
| Predicted Price | AED 1,484,825 |
| Actual Price    | AED 1,400,000 |
| Difference      | AED 84,825    |
| Accuracy        | 93.9% ✅      |


## 📝 Final Interpretations & Conclusions
> These interpretations are also written in detail inside 
> the notebook at the end of all analysis sections.

### 🏙️ EDA Findings
- Dubai dominates with highest listings and prices
- Apartments are the most common property type
- Furnished properties sell at higher prices
- Off-Plan properties are cheaper than Ready ones
- Business Bay and Downtown Dubai are most expensive areas
- Listing activity peaked in mid-2024

### ⚙️ Preprocessing Insights
- Zero values in building features were treated as missing
- Top and bottom 1% prices removed as outliers
- Log transformation successfully normalized price distribution
- Frequency encoding handled high cardinality area_name column
- Date features extracted seasonal pricing patterns

### 🤖 Model Conclusions
- Random Forest best explained 95.6% of price variation
- Average prediction error of 12.13% is acceptable for 
  real estate — even human experts vary by 10-15%
- No overfitting detected — model generalizes well
- Single property test confirmed 93.9% real-world accuracy

### 💡 Business Value
This model can help buyers verify fair pricing, assist 
sellers in setting competitive prices, support agents 
with data-driven valuations, and help investors identify 
underpriced properties in the UAE market.

---

## 👤 Author
**Shad Ali Shah**

## 📄 License
This project is licensed under the MIT License.
