
# 🏠 Multiple Linear Regression: Boston Housing Analysis

A clean and concise dive into linear modeling using the Boston Housing dataset.


---

## 📌 Objective

Predict housing prices using **multiple linear regression**, focusing on a few sharp, statistically valid predictors.

---

## 🧠 What Was Done

- 🎯 **Selected Predictors:** `RM`, `DIS`, `TAX`, `INDUS`
  - Verified multicollinearity using **Variance Inflation Factor (VIF)** — anything fishy? Removed it.
  
- 📊 **Exploratory Data Analysis**
  - Visualized relationships using **scatter plots** to understand correlation trends.
  
- 🛠 **Model Building**
  - Performed **train-test split** and trained a **Linear Regression model** using `scikit-learn`.

- 📈 **Evaluation Metrics**
  - Calculated:  
    - **Mean Squared Error (MSE)**
    - **R² Score**
    - **Adjusted R² Score**

---

## 🧪 Tech Stack

| Tool | Purpose |
|------|---------|
| `pandas` | Data manipulation |
| `matplotlib` & `seaborn` | Visualization |
| `sklearn.linear_model` | Modeling |
| `statsmodels` | VIF calculation & metrics |

---

## 📎 Code Sneak Peek

```python
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_squared_error, r2_score

model = LinearRegression()
model.fit(X_train, y_train)

y_pred = model.predict(X_test)

mse = mean_squared_error(y_test, y_pred)
r2 = r2_score(y_test, y_pred)
````

---

## 🚀 Results Snapshot

* **MSE:** Low enough to sleep well at night 💤
* **R² Score:** Captured most variance
* **Adjusted R²:** On point, even after adjusting for the number of predictors

---

## ⚙️ Run It Yourself

```bash
git clone https://github.com/yourusername/boston-mlr.git
cd boston-mlr
python boston_mlr.py
```

---

## 💡 Final Thought

Simple tools. Clean data. Smart decisions. That's how we build interpretable models that work.
