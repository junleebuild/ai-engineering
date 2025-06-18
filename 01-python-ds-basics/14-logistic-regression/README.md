
# 🤖 13 - Logistic Regression 

## 📌 Overview

In this section, I studied **Logistic Regression**, one of the most widely used supervised classification algorithms.  
Unlike linear regression (which predicts a continuous number), logistic regression predicts a **probability**, allowing it to classify between two categories (binary classification).

Common examples:
- Will a user click this ad or not?
- Is this email spam or not?
- Will this customer churn or not?

---

## ⚙️ Key Concepts

- The output of logistic regression is **between 0 and 1** — a probability.
- The model uses a **sigmoid (logistic) function** to map predictions to probabilities:

\[
\sigma(z) = \frac{1}{1 + e^{-z}}
\]

- If the probability is greater than 0.5 → predict **class 1**  
  Else → predict **class 0**

---

## 🧑‍💻 Project: Predicting Ad Clicks

### Dataset: `advertising.csv`

### Features:
- **Daily Time Spent on Site**  
- **Age**  
- **Area Income**  
- **Daily Internet Usage**  
- **Ad Topic Line**  
- **City**  
- **Male**  
- **Timestamp**  
- **Clicked on Ad** (Target variable - 0 or 1)

---

### 📊 Workflow:

1️⃣ **EDA (Exploratory Data Analysis)**  
- Used `sns.jointplot()`, `sns.pairplot()` to understand feature relationships.

2️⃣ **Data Preparation**  
- Selected features for the model.
- Splitted the data into training/test sets:
    ```python
    X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, random_state=101)
    ```

3️⃣ **Training the Model**
    ```python
    from sklearn.linear_model import LogisticRegression

    logmodel = LogisticRegression(max_iter=1000)
    logmodel.fit(X_train, y_train)
    ```

4️⃣ **Prediction**
    ```python
    predictions = logmodel.predict(X_test)
    ```

5️⃣ **Evaluation**
    ```python
    from sklearn.metrics import classification_report, confusion_matrix

    print(classification_report(y_test, predictions))
    print(confusion_matrix(y_test, predictions))
    ```

---

## 💬 Personal Reflection

Logistic Regression helped me understand **classification vs regression** more clearly.  
Seeing how logistic regression predicts probabilities (not raw scores), and then uses the sigmoid function to classify was very useful.  
While I still need more practice with interpreting the confusion matrix and precision/recall, the process of training and evaluating a classifier is becoming more comfortable.

---

## 📁 Files Included

- `01-logistic regression.ipynb` – Learning notebook  
- `02-logistic regression project.ipynb` – Project notebook  
- `advertising.csv` – Dataset for ad click prediction
- `titanic_test.csv`
- `titanic_train.csv`
---
