# 🚗 Ford Car Price Prediction

## 📌 Project Overview
This project predicts the selling price of used Ford cars using a supervised machine learning regression model. 

The model is trained on real-world Kaggle data containing vehicle specifications such as model, year, mileage, fuel type, transmission, mpg, tax, and engine size.

This project includes a complete end-to-end ML workflow:
**EDA → Feature Engineering → Preprocessing → Model Training → Evaluation**

## 📂 Dataset Overview
The dataset contains multiple Ford car listings with the following attributes:

| Feature | Description | Type |
| :--- | :--- | :--- |
| **model** | Ford car model/variant | Categorical |
| **year** | Manufacturing year | Numerical |
| **price** | Selling price ($) | **Target** |
| **transmission** | Automatic / Manual / Semi-Auto | Categorical |
| **mileage** | Total miles driven | Numerical |
| **fuelType** | Petrol / Diesel / Hybrid / Electric / Other | Categorical |
| **tax** | Annual road tax | Numerical |
| **mpg** | Miles per gallon | Numerical |
| **engineSize** | Engine size in litres | Numerical |

## 🛠️ Tech Stack
* **Python**
* **Pandas, NumPy** – Data processing
* **Matplotlib, Seaborn** – Data visualization
* **Scikit-Learn** – Preprocessing & ML models
* **Jupyter Notebook**

## 📊 Key Workflow Steps

### 1. Data Cleaning & EDA
* Checked missing values and duplicates.
* Visualized distributions of price, year, mileage, and mpg.
* Studied correlations between features and the target.
* **Key Insight:** 👉 Car year, mileage, and engineSize have the strongest influence on price.

### 2. Feature Engineering
* **One-Hot Encoding** applied to: `model`, `transmission`, `fuelType`.
* Converted categorical values into an ML-friendly format.

### 3. Data Preprocessing
* **Scaling:** Used `StandardScaler` on numerical columns (`year`, `mileage`, `tax`, `mpg`, `engineSize`).
* **Splitting:** Split dataset into Training & Testing sets.

### 4. Model Building 
* Trained multiple regression models using different encoding techniques and evaluated performance.

### 5. Model Evaluation

| Model                                 | R² Score | Adjusted R² |
|---------------------------------------|----------|--------------|
| Linear Regression (OneHot-Encoding)   | 0.846    | 0.844        |
| Linear Regression (Labelled-Encoding) | 0.737    | 0.736        |


## 🚀 How to Run

```bash
git clone https://github.com/harshitsaxenavs/Ford-Car-Price-Prediction.git
cd Ford-Car-Price-Prediction
pip install pandas numpy seaborn matplotlib scikit-learn scipy
jupyter notebook ford.ipynb
```


## 📈 Future Improvements
- Model tuning
- Try XGBoost / Gradient Boosting


## 👨‍💻 Author
Harshit Saxena  
B.Tech CSE • Maharaja Surajmal Institute of Technology, Delhi  

📧 harshitsaxenavs@gmail.com  
GitHub: https://github.com/harshitsaxenavs  

## ⚠️ License
This project is not open-source. All rights reserved.
