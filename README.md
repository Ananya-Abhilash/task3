# Linear Regression on Housing Dataset

This project demonstrates the implementation of **Simple and Multiple Linear Regression** using a housing dataset. The primary goal is to predict house prices based on features like area, number of bedrooms, availability of amenities, etc.

---

## Objective

* Understand and implement linear regression models.
* Evaluate the model using various metrics.
* Visualize predictions and interpret model coefficients.

---

## Tools Used

* **Pandas**: For data manipulation.
* **NumPy**: For numerical operations.
* **Matplotlib**: For visualizing the results.
* **Scikit-learn**: For implementing regression models and evaluation.

---

## Dataset

* Filename: `Housing.csv`
* Columns include:

  * `price` (target)
  * `area`, `bedrooms`, `bathrooms`, `stories`, `mainroad`, etc.
  * Categorical variables like `mainroad`, `guestroom`, `furnishingstatus`, etc.

---

## Steps Followed

### 1. **Import Libraries**

All necessary libraries for data processing, model building, and evaluation are imported.

### 2. **Load Dataset**

The dataset is loaded using `pandas.read_csv()`.

### 3. **Preprocessing**

* One-hot encoding is used to convert categorical columns into numeric format.
* The target variable (`price`) is separated from the features.

### 4. **Train-Test Split**

* The dataset is split into training and testing sets using `train_test_split()`.
* 80% training and 20% testing with a fixed random state for reproducibility.

### 5. **Model Fitting**

* A `LinearRegression` model from `sklearn.linear_model` is initialized and trained using `.fit()` on training data.

### 6. **Prediction & Evaluation**

* Predictions are made on the test set.
* The model is evaluated using:

  * Mean Absolute Error (MAE)
  * Mean Squared Error (MSE)
  * R² Score

### 7. **Model Interpretation**

* Coefficients of features are extracted using `.coef_` and displayed to understand the influence of each feature.

### 8. **Visualization**

* A scatter plot is drawn between actual vs predicted prices.
* A red dashed line represents the ideal prediction line (Perfect prediction).

---

## Output Summary

* **MAE**, **MSE**, and **R² Score** provide insight into model performance.
* Coefficients table shows which features contribute most to price.
* The scatter plot helps visually assess prediction accuracy.

---

## Extensions

* You can perform **Simple Linear Regression** using only one feature (e.g., `area`) and plot the regression line.
* Try feature selection or regularization (Lasso/Ridge) for performance improvement.

---

## Conclusion

This exercise provides a hands-on implementation of linear regression in Python using real-world housing data, focusing on model building, evaluation, and interpretation.
