# Day-81-Model-evaluation

###  Overview

**Model Evaluation** is the process of measuring how well a **machine learning model performs** on data.

It helps determine whether a model is **accurate, reliable, and ready for real-world use**.

---

##  Why Model Evaluation?

* To check model performance
* To compare different models
* To avoid overfitting and underfitting

---

##  Evaluation Metrics (Classification)

###  Accuracy

Percentage of correct predictions

```id="k1a8bz"
Accuracy = (Correct Predictions) / (Total Predictions)
```

---

###  Precision

How many predicted positives are actually correct

```id="6dj2kz"
Precision = TP / (TP + FP)
```

---

###  Recall

How many actual positives are correctly identified

```id="m3d9r1"
Recall = TP / (TP + FN)
```

---

###  F1 Score

Balance between precision and recall

```id="p9f1x3"
F1 Score = 2 * (Precision * Recall) / (Precision + Recall)
```

---

###  Confusion Matrix

A table used to evaluate classification results:

|                 | Predicted Positive | Predicted Negative |
| --------------- | ------------------ | ------------------ |
| Actual Positive | TP                 | FN                 |
| Actual Negative | FP                 | TN                 |

---

##  Evaluation Metrics (Regression)

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* R² Score

---

##  Example (Python)

```python id="m2k9x1"
from sklearn.metrics import accuracy_score

y_true = [0, 1, 1, 0]
y_pred = [0, 1, 0, 0]

print(accuracy_score(y_true, y_pred))
```

---

##  Key Takeaways

- Evaluation helps measure model performance
- Different metrics for classification and regression
- Important for improving models

---

