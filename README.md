# Customer Rating Prediction 🛒⭐

A machine learning project that predicts customer review scores (1–5) for orders on **Olist**, a Brazilian e-commerce marketplace, using order, delivery, payment, and product data.

## 📌 Project Idea

Customer ratings reflect how satisfied a buyer is with a product, the delivery, and the overall shopping experience. This project builds a regression model that predicts the review score a customer is likely to give, based on features such as delivery delay, shipping cost, payment type, product category, and order timing. The goal is to help the business flag at-risk orders (likely to receive low ratings) before the customer leaves a review, so the issue can be addressed proactively.

**Dataset:** [Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

## 👥 Team Members

| Member | ID | Contribution |
|---|---|---|
| Mahmoud Elaraby | 23011143 | Data loading & merging of all Olist tables, data auditing (missing values, duplicates, hidden nulls), and data cleaning/preprocessing (type conversion, outlier detection, handling missing values) |
| Maram Ahmed Rashed | 23011144 | Feature engineering — created delivery, time, pricing, and product-based features (e.g. delivery delay, delivery speed ratio, shipping price ratio, product volume/density, same-state shipping) |
| Mahmoud Waleed Mahmoud | 2401245338 | Exploratory Data Analysis (target distribution, feature distributions, correlation and time analysis) and the first model — Linear Regression |
| Mokhtar Ibrahim | 23011521 | Decision Tree and Random Forest regression models |
| Mariam Ramadan Amin | 23011529 | Final model — KNN Regressor, model comparison, and GridSearchCV hyperparameter tuning of the best-performing model |
| Jomana Mahmoud Farghaly | 2401244006 | Error analysis (predicted vs. actual, residual plots, error by category) and final business insights & recommendations |

## ⚙️ How It Works

1. Load and merge the Olist CSV files (customers, orders, order items, payments, reviews, products, sellers).
2. Clean and preprocess the data (fix data types, handle missing values and outliers).
3. Engineer features related to delivery time, pricing, product characteristics, and purchase timing.
4. Explore the data (distributions, correlations, time trends).
5. Train and compare four regression models: Linear Regression, Decision Tree, Random Forest, and KNN.
6. Tune the best model with GridSearchCV.
7. Evaluate the final model (MAE, RMSE, R²) and analyze prediction errors.
8. Summarize business insights and recommendations.

## 🛠️ Libraries & Requirements

- Python 3
- pandas
- numpy
- matplotlib
- seaborn
- plotly
- scikit-learn
- scipy
- joblib

Install everything with:
```bash
pip install pandas numpy matplotlib seaborn plotly scikit-learn scipy joblib
```

## ▶️ How to Run

1. Download the [Olist dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) and place the CSV files in the project folder (or update the file paths in the notebook).
2. Open `Customer_Rating_Prediction.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab.
3. Run the cells in order, from data loading through to the final model evaluation and business insights.
