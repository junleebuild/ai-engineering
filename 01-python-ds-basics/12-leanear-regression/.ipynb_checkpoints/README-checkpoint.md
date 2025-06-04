# 🧠 Linear Regression (Part 02)

## 📌 Overview

In this section, I studied **Linear Regression**, one of the most fundamental supervised machine learning algorithms.  
It’s used to predict a continuous outcome based on the relationship between input variables (features) and the target variable.

I used the **scikit-learn** library (`sklearn`) to perform the steps of training, evaluating, and visualizing linear regression.

---

## 📁 Files Included

- `01-my linear regression with python.ipynb` – My personal practice notebook  
- `02-linear regression project.ipynb` – Project assignment file  
- `03-linear regression project - solutions.ipynb` – Instructor’s reference solution  
- `01-ref linear regression with python.ipynb` – Instructor's lecture notebook  
- `USA_Housing.csv` – Dataset for the initial regression model  
- `Ecommerce Customers` – Dataset for the project

---

## 🔧 Key Concepts and Workflow

### 1. 📊 Train-Test Split

```python
from sklearn.model_selection import train_test_split

X = df[['Avg. Area Income', 'Avg. Area House Age', 'Avg. Area Number of Rooms',
        'Avg. Area Number of Bedrooms', 'Area Population']]
y = df['Price']

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, random_state=101)
```

We split the dataset into:
- `X_train`: Training features  
- `y_train`: Training labels  
- `X_test`: Test features  
- `y_test`: Test labels

> 🔎 **Goal**: Teach the model with training data and evaluate its performance on test data.

---

### 2. 🧠 Model Training

```python
from sklearn.linear_model import LinearRegression

lm = LinearRegression()
lm.fit(X_train, y_train)
```

- The `.fit()` function **trains the model** by finding the best-fitting line through the training data.
- Internally, it calculates the **optimal coefficients (slope)** and **intercept** for the regression equation:

> 📘 𝑦 = 𝛽₀ + 𝛽₁𝑋₁ + 𝛽₂𝑋₂ + ⋯ + 𝛽ₙ𝑋ₙ

---

### 3. 🧮 Interpreting Coefficients

```python
coeff_df = pd.DataFrame(lm.coef_, X.columns, columns=['Coefficient'])
```

Each coefficient tells us **how much the target variable (`Price`) will change** when the corresponding feature increases by one unit, **keeping all others constant**.

---

### 4. 📈 Model Evaluation

We predicted outcomes for test data and evaluated the model:

```python
predictions = lm.predict(X_test)

from sklearn import metrics

print("MAE:", metrics.mean_absolute_error(y_test, predictions))
print("MSE:", metrics.mean_squared_error(y_test, predictions))
print("RMSE:", np.sqrt(metrics.mean_squared_error(y_test, predictions)))
```

**Evaluation Metrics:**
- MAE: Mean Absolute Error
- MSE: Mean Squared Error
- RMSE: Root Mean Squared Error

---

### 5. 📊 Visualization (Optional)

```python
sns.scatterplot(x=y_test, y=predictions)
```

Shows how closely the predicted values match the actual target values.

---

## 💬 Personal Reflection

I finally started understanding what machine learning actually **does** behind the scenes.  
The `.fit()` function felt like the model was “studying” the patterns in data, and then `.predict()` let it guess the outcomes based on that study.

Even though I didn’t fully understand every mathematical detail, the overall process of **train → fit → predict → evaluate** makes intuitive sense now.  
Looking at `coef_` also helped me see how features influence the target, which I think is very powerful in real-life applications like housing or sales predictions.
