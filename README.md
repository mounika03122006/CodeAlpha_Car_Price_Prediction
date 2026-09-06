# Car Price Prediction with Machine Learning

**CodeAlpha Data Science Internship — Task 3**

## 📌 Overview
This project predicts the resale (selling) price of a used car based on features such as present price, kilometers driven, fuel type, seller type, transmission, owner history, and car age. It demonstrates a complete machine learning workflow — from data cleaning to model evaluation.

## 📊 Dataset
The dataset (`car_data.csv`) contains 301 rows with the following columns:
- `Car_Name` — model name of the car
- `Year` — year of manufacture
- `Selling_Price` — price the car is being sold for (target variable)
- `Present_Price` — current showroom price
- `Driven_kms` — total kilometers driven
- `Fuel_Type` — Petrol / Diesel / CNG
- `Selling_type` — Dealer / Individual
- `Transmission` — Manual / Automatic
- `Owner` — number of previous owners

## 🛠 Tools & Libraries
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

## 🔍 Workflow
1. **Data Exploration** — checked structure, data types, and missing values
2. **Feature Engineering** — converted `Year` into `Car_Age`, dropped `Car_Name`, one-hot encoded categorical features
3. **EDA** — correlation heatmap and scatter plots to understand relationships with `Selling_Price`
4. **Modeling** — trained and compared Linear Regression and Random Forest Regressor using a scikit-learn Pipeline
5. **Evaluation** — measured performance using MAE, RMSE, and R²
6. **Feature Importance** — identified which features most influence price

## 📈 Results
| Model | MAE | RMSE | R² Score |
|---|---|---|---|
| Linear Regression | 1.22 | 1.87 | 0.849 |
| Random Forest | 0.64 | 0.98 | 0.958 |

- **Present_Price** and **Car_Age** were the strongest predictors of selling price.
- Random Forest outperformed Linear Regression, capturing non-linear relationships in the data.

## 🚀 How to Run
```bash
git clone https://github.com/mounika03122006/CodeAlpha_Car_Price_Prediction.git
cd CodeAlpha_Car_Price_Prediction
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
jupyter notebook "Car_Price_Prediction (Task 3).ipynb"
```
Run all cells to reproduce the analysis and results.

## 🙌 Acknowledgment
This project was completed as part of the **CodeAlpha Data Science Internship**.
