# E-Commerce Furniture Sales Prediction

This project builds an end-to-end machine learning model to predict the number of units sold for furniture products on an e-commerce platform using pricing and product title information.

## Business Problem
E-commerce platforms face challenges in forecasting product demand due to highly skewed sales patterns and limited product-level data. Inaccurate predictions can lead to poor inventory planning and ineffective pricing strategies.

## Objective
- Predict product-level sales using machine learning  
- Analyze the impact of price and discounts on demand  
- Support data-driven inventory and pricing decisions  

## Dataset
- E-commerce Furniture Dataset (2024)
- ~2000 products
- Key features: product title, price, original price, units sold

## Approach
- Data cleaning and preprocessing (currency formatting, missing values)
- Feature engineering (discount calculation)
- Text vectorization using TF-IDF
- Log transformation of target variable to handle skewness
- Model training using Linear Regression and Random Forest Regressor

## Results
| Model | MAE | RMSE | R² |
|------|-----|------|----|
| Linear Regression | ~17.6 | ~72.2 | ~0.05 |
| Random Forest | ~16.5 | ~67.9 | ~0.16 |

Random Forest outperformed Linear Regression by capturing non-linear relationships in the data.

## Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

## Conclusion
The project demonstrates a practical machine learning approach to e-commerce sales prediction. Despite limited features, the model produces stable and realistic demand forecasts and can be extended with additional data such as ratings or reviews.


