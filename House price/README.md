# 🏠 House Price Prediction

This project is a **Machine Learning model** that predicts **house prices** based on given features.
It uses **Linear Regression** and **Random Forest Regressor**, along with **feature scaling** and **hyperparameter tuning** to achieve high accuracy.

---

## Features

* Loads a **House Prices Dataset** (CSV).
* Handles preprocessing and feature scaling.
* Implements multiple ML models:

  * **Linear Regression**
  * **Random Forest Regressor**
  * **Gradient Boosting Regressor** (extendable)
* Performs **GridSearchCV** for hyperparameter tuning.
* Evaluates models with metrics:

  * Mean Absolute Error (MAE)
  * Mean Squared Error (MSE)
  * R² Score

---

## Workflow

1. **Import Libraries**
   Uses `pandas`, `scikit-learn`, and ensemble models.

2. **Load Dataset**

   ```python
   data = pd.read_csv("house_prices_dataset.csv")
   ```

3. **Preprocessing**

   * Drop target column (`price`) for features (`X`).
   * Split into **train/test sets** (80/20).
   * Apply **StandardScaler** to normalize features.

4. **Model Training**

   * **Linear Regression** for baseline.
   * **Random Forest Regressor** for better performance.
   * **GridSearchCV** tuning on Random Forest for optimized hyperparameters.

5. **Evaluation**

   ```python
   print("MAE:", mean_absolute_error(y_test, y_pred))
   print("MSE:", mean_squared_error(y_test, y_pred))
   print("R² Score:", r2_score(y_test, y_pred))
   ```

---

## Example Output

```
Linear Regression
MAE: 101239.12
MSE: 2.34e+10
R² Score: 0.8123

Random Forest (default)
MAE: 41239.77
MSE: 9.12e+09
R² Score: 0.9274

Random Forest (GridSearch tuned)
Best R² score after tuning : 0.9448
Best parameters : {'max_depth': 20, 'min_samples_split': 2, 'n_estimators': 200}
```

✍️ **Author:** Harshvardhan Sanadhya
