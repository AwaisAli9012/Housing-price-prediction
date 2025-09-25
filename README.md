# California Housing Price Prediction

A machine learning project to predict median house values in California using the classic California Housing dataset. This project compares **Linear Regression** and **Random Forest Regressor** models to understand their performance on real estate price prediction.

![Model Comparison](https://img.shields.io/badge/Models-Linear_Regression_%26_Random_Forest-blue)
![Dataset](https://img.shields.io/badge/Dataset-California_Housing-8A2BE2)
![Python](https://img.shields.io/badge/Python-3.7%2B-green)

## 📊 Dataset Overview

The California Housing dataset contains **20,640** samples with **8 features** and **1 target variable**:

### Features:
- `MedInc`: Median income in block group
- `HouseAge`: Median house age in block group  
- `AveRooms`: Average number of rooms per household
- `AveBedrms`: Average number of bedrooms per household
- `Population`: Block group population
- `AveOccup`: Average number of household members
- `Latitude`: Block group latitude
- `Longitude`: Block group longitude

### Target:
- `MedHouseVal`: Median house value for California districts (in $100,000s)

**Dataset Properties:**
- No missing values
- Real-world geographical and demographic data
- Collected from the 1990 California census

## 🚀 Models Implemented

### 1. Linear Regression
- **Preprocessing**: StandardScaler for feature normalization
- **Assumption**: Linear relationship between features and target
- **Use Case**: Baseline model for comparison

### 2. Random Forest Regressor
- **Parameters**: 100 estimators, random state = 42
- **Advantages**: Handles non-linear relationships, provides feature importance
- **No Scaling Required**: Tree-based models are scale-invariant

## 📈 Evaluation Metrics

Three key metrics are used to evaluate model performance:

- **RMSE** (Root Mean Squared Error): Measures prediction accuracy in original units
- **MAE** (Mean Absolute Error): Average absolute prediction error
- **R² Score**: Proportion of variance explained by the model

## 🏆 Results

The models are evaluated on a **20% test set** (4,128 samples). Typical results show:

- **Random Forest** significantly outperforms Linear Regression
- **R² scores** around 0.80-0.85 for Random Forest vs 0.60-0.65 for Linear Regression
- **Feature Importance** reveals which factors most influence housing prices

## 📊 Visualizations

1. **Actual vs Predicted Plot**: Scatter plot showing Random Forest predictions against actual values with perfect prediction line
2. **Feature Importance Bar Chart**: Ranked bar plot showing the most influential features for price prediction

## 🛠️ Requirements

- Python 3.7+
- pandas
- numpy  
- scikit-learn
- matplotlib
- seaborn

## 📦 Installation

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
