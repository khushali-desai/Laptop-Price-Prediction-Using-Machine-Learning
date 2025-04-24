# 💻 Laptop Price Prediction - Machine Learning Project

## 🎯 Objective
To build a regression model that accurately predicts the price of laptops based on features such as brand, processor, RAM, SSD, rating, and weight. This helps in pricing strategy, customer decision-making, and market analysis.

## 🧰 Tools & Libraries Used
- `pandas`, `numpy` – Data manipulation and numerical computation  
- `matplotlib.pyplot`, `seaborn` – Data visualization  
- `sklearn.model_selection` – `train_test_split` for splitting data  
- `sklearn.linear_model` – `LinearRegression` for model training  
- `sklearn.ensemble` – `RandomForestRegressor` for higher accuracy  
- `sklearn.metrics` – `r2_score`, `mean_absolute_error` for model evaluation  

## 🔍 Workflow Summary

1. **Data Cleaning**
   - Handled null values with forward-fill, then dropped remaining nulls.
   - Converted rating and price to numeric types.
   - Removed duplicates and filtered outliers using the IQR method.

2. **Exploratory Data Analysis (EDA)**
   - Visualized brand-wise price trends and rating distributions.
   - Identified correlations between features and price.

3. **Feature Engineering**
   - One-hot encoded categorical variables (Brand, Processor, etc.).
   - Model used without scaling, due to Random Forest’s tree-based nature.

4. **Model Training & Evaluation**
   - Trained both **Linear Regression** and **Random Forest Regressor** on 80/20 split.

### 📈 Model Performance

| Model               | Train R² | Test R² | MAE (Test) |
|--------------------|----------|---------|------------|
| Linear Regression  | 0.78     | 0.74    | ~4500 INR  |
| Random Forest      | 0.97     | 0.88    | ~2500 INR  |

> ✅ **Random Forest** outperformed Linear Regression by a significant margin in both accuracy and error reduction.

## ✅ Conclusion
The Random Forest model proved to be the best choice for predicting laptop prices with **high accuracy and low error**. The project showcases real-world data preprocessing, visualization, and model selection – all critical parts of a machine learning pipeline.

---

📁 *This project was part of my Data Science learning journey and demonstrates hands-on proficiency in EDA, model building, and evaluation using real industry-style datasets.*
