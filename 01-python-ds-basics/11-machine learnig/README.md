# 🧠 Machine Learning Overview

## 📚 What is Machine Learning?

Machine Learning is a method of data analysis that automates analytical model building.  
By using algorithms that iteratively learn from data, it allows computers to find hidden insights without being explicitly programmed.

It is widely used in:
- Fraud detection
- Search engine optimization
- Credit scoring
- Predictive maintenance
- Recommendation systems
- Sentiment analysis
- Image recognition, and more.

---

## 🔍 Key Concepts

### Supervised vs Unsupervised Learning

| Type              | Description                                                                 |
|-------------------|-----------------------------------------------------------------------------|
| **Supervised**    | Trained on labeled data (input-output pairs). E.g., spam detection          |
| **Unsupervised**  | Finds patterns in unlabeled data. E.g., customer segmentation (clustering)  |

---

## 🧮 Neural Networks & Deep Learning

- **Neural Network**: A machine learning architecture inspired by biological neurons.
- **Deep Learning**: Neural networks with multiple hidden layers.

---

## 🧪 Supervised Learning Process

1. Data Acquisition
2. Data Cleaning
3. Data Splitting: Train / Validation / Test
4. Model Training
5. Hyperparameter Tuning
6. Model Evaluation
7. Model Deployment

---

## ⚠️ Overfitting vs Underfitting

| Term          | Description                                                                 |
|---------------|-----------------------------------------------------------------------------|
| **Overfitting** | Model performs well on training data but poorly on new data               |
| **Underfitting**| Model fails to capture the underlying trend; performs poorly overall       |

---

## 📊 Evaluation Metrics

### 📌 Classification

- **Accuracy** = (TP + TN) / (TP + TN + FP + FN)
- **Recall** = TP / (TP + FN) – how well we find relevant cases
- **Precision** = TP / (TP + FP) – how many predicted positive cases were actually correct
- **F1 Score** = 2 × (Precision × Recall) / (Precision + Recall)

> Confusion Matrix is used to summarize prediction results vs actual labels.

---

### 📈 Regression

- **MAE (Mean Absolute Error)**: Average of absolute differences  
- **MSE (Mean Squared Error)**: Average of squared errors  
- **RMSE (Root Mean Squared Error)**: Square root of MSE, same unit as label

Use-case context is crucial:  
- RMSE of 10 is great for house prices but bad for predicting candy bar cost.

---

## 🧩 Unsupervised Learning Techniques

- **Clustering**: Grouping similar data points (e.g., KMeans)
- **Anomaly Detection**: Identifying outliers (e.g., fraud detection)
- **Dimensionality Reduction**: Reducing number of features (e.g., PCA)

---

## 🧠 Final Thoughts

Machine Learning is not performed in isolation—it involves understanding data context, working with domain experts, and selecting proper metrics.  
This module provided a conceptual roadmap before diving into practical tools like **Scikit-learn**, **TensorFlow**, and **Keras**.

---

📎 Included File:  
- `11-Machine-Learning-Overview.pdf`