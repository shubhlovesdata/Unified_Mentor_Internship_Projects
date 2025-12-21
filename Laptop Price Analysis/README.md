# 💻 Laptop Price Prediction

This project focuses on predicting the price of laptops based on various hardware configurations using Machine Learning regression techniques.

---

## 📊 Project Overview
The goal of this project is to provide an accurate price estimation tool for consumers and retailers. By analyzing a dataset of laptop specifications, we build a predictive model that understands how components like RAM, CPU, and GPU impact the final market value.



---

## 🔄 Machine Learning Project Lifecycle

To ensure a high-quality model, this project follows the 8-stage Machine Learning lifecycle:

### 1. Problem Definition
The objective is to solve a regression problem: predicting a continuous numerical value (**Price**) based on categorical and numerical features of a laptop.

### 2. Data Collection
The dataset used contains over 1,300 entries with features such as:
* Company (Brand)
* TypeName (Notebook, Gaming, Ultrabook, etc.)
* RAM & Weight
* CPU & GPU specifications
* Screen Resolution

### 3. Data Cleaning & Preprocessing
Data was refined for analysis by:
* Removing units like "GB" from RAM and "kg" from Weight.
* Converting columns to numeric types.
* Handling missing or inconsistent values.

### 4. Exploratory Data Analysis (EDA)
Performed univariate and bivariate analysis to identify trends:
* Impact of Brand on Price.
* Relationship between RAM capacity and cost.
* Distribution of Screen sizes.

### 5. Feature Engineering
Created new, more impactful features:
* **PPI (Pixels Per Inch):** Calculated from resolution and screen size.
* **Touchscreen/IPS:** Binary flags extracted from screen descriptions.
* **Processor Brand:** Simplified CPU names into "Intel Core i7", "AMD", etc.

### 6. Model Selection
Multiple algorithms were tested to find the best performance:
* Linear Regression
* Lasso & Ridge Regression
* **Random Forest Regressor** (Best Performance)
* XGBoost

### 7. Model Training & Pipeline
A Scikit-Learn **Pipeline** was used to bundle the `ColumnTransformer` (for One-Hot Encoding) and the model together. This ensures that the same preprocessing is applied during both training and inference.

### 8. Evaluation & Deployment
* **Performance:** Achieved an R2 Score of ~0.88.
* **Deployment:** Built a web interface using **Streamlit** for real-time predictions.

---

## 🛠 Tech Stack
* **Language:** Python 3.8+
* **Libraries:** Pandas, NumPy, Scikit-Learn, Seaborn, Matplotlib
* **UI/UX:** Streamlit

---

## 🚀 How to Run
1. Clone the repo: `git clone https://github.com/yourusername/laptop-price-predictor.git`
2. Install requirements: `pip install -r requirements.txt`
3. Run the app: `streamlit run app.py`

---

## 📊 Results Comparison

In this section, we validate the model's accuracy by comparing its prediction against a real-world retail listing from Amazon.

### Flipkart Price
The following laptop was selected for testing:
* **Model:** Acer Nitro V Intel Core i5 13th Gen
* **Specs:** 16 GB RAM / 512 GB SSD / Windows 11 Home / 6 GB Graphics (Nvidia GeForce RTX 3050)
* **Display:** 15.6 Inches, 144 Hz
* **Weight:** 2.1 Kg
* **Current Retail Price:** ₹83,990

![Flipkart Listing Screenshot]("C:\Users\shubh\OneDrive\Pictures\Screenshots\Screenshot 2025-12-21 111517.png")

---

### Predicted Price
Using the same configuration in our **Laptop Price Predictor** application:

1. **Brand:** Acer
2. **Type:** Gaming
3. **RAM:** 16 GB
4. **CPU:** Intel Core i5
5. **GPU:** Nvidia
6. **OS:** Windows

![Model Prediction Screenshot1]("C:\Users\shubh\OneDrive\Pictures\Screenshots\Screenshot 2025-12-21 111728.png")
![Model Prediction Screenshot2]("C:\Users\shubh\OneDrive\Pictures\Screenshots\Screenshot 2025-12-21 111756.png")

**Observation:** The model provides a price point closely aligned with the actual market value, demonstrating the effectiveness of the Random Forest Regressor and the feature engineering process.

© 2025 | Developed by Your Name
