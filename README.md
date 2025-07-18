# Bangalore House Price Prediction

This machine learning project predicts house prices in Bangalore based on various property features like location, square footage, number of bathrooms, and BHK. The goal is to assist buyers or sellers in understanding the estimated price of a property using regression models.

## Table of Contents

- [Overview]
- [Technologies Used]
- [Dataset]
- [Data Preprocessing]
- [Model Training]
- [Evaluation]
- [How to Run]

---

##  Overview

The project includes:
- Data cleaning and preprocessing
- Encoding categorical variables
- Feature scaling
- Applying regression models (Linear, Lasso, Ridge)
- Evaluating performance using R² score
- Making predictions on new data

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib & Seaborn (for visualization)
- Scikit-learn (ML models and tools)
- Jupyter Notebook

---

## Dataset

The dataset contains the following features:
- **Location**
- **Total Square Foot (area)**
- **Number of Bathrooms**
- **Number of BHK (bedroom, hall, kitchen)**
- **Price** (target variable)

*Source: Kaggle dataset*

---

## Data Preprocessing

- Removed duplicates and null values
- Dropped outliers (like unrealistic BHK to sqft ratios)
- Applied `OneHotEncoding` for categorical features (like location)
- Scaled numerical features using `StandardScaler`

---

## Model Training

Implemented using `scikit-learn`:
- `LinearRegression`
- `Lasso`
- `Ridge`

Used `make_pipeline` and `make_column_transformer` to simplify transformation + model building.

---

## Evaluation

Performance was evaluated using the **R² Score** on test data:

- **Linear Regression**: `0.84`
- **Lasso Regression**: `0.82`
- **Ridge Regression**: `0.83`

*(Note: These scores may vary slightly depending on train-test split.)*

---
## How to Run

1. **Clone the repo**
   ```bash
   git clone https://github.com/misterk1269/ML_Project.git
   
2. Install required libraries
   ```bash
   pip install -r requirements.txt
   
3. Run the notebook
   ```bash
   jupyter notebook 

