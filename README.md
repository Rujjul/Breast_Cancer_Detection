## 📖 Overview

This project demonstrates the use of **Logistic Regression** to classify breast cancer tumors as either benign or malignant. Using the Wisconsin Breast Cancer dataset, this machine learning model analyzes various cell features to make accurate predictions, showcasing the power of data science in medical diagnostics.

The goal is to build a reliable classifier and evaluate its performance using standard metrics.

---
## 🔬 Methodology

The project follows a standard machine learning workflow:

1.  **Data Loading**: The dataset is loaded using the `pandas` library.
2.  **Data Preprocessing**: The 'Sample code number' column is dropped, and the data is split into features (`X`) and the target variable (`y`).
3.  **Train-Test Split**: The dataset is divided into an 80% training set and a 20% test set to evaluate the model on unseen data.
4.  **Model Training**: A **Logistic Regression** model from `scikit-learn` is trained on the training data.
5.  **Model Evaluation**: The model's performance is assessed using:
    * A **Confusion Matrix** to understand the classification results on the test set.
    * **10-fold Cross-Validation** to ensure the model's stability and reliability on the training data.

---
## ✨ Results

The model demonstrated excellent performance in classifying tumors.

### Confusion Matrix on Test Set

The confusion matrix below shows the model's predictions on the 20% test set.

|                    | Predicted: Benign (2) | Predicted: Malignant (4) |
| :----------------- | :--------------------: | :----------------------: |
| **Actual: Benign (2)** |          **84** |            3             |
| **Actual: Malignant (4)**|           3            |          **47** |

* **Test Set Accuracy**: From the matrix, the accuracy is calculated as $(84 + 47) / (84 + 3 + 3 + 47) = 131 / 137 \approx \textbf{95.6%}$.
### K-Fold Cross-Validation

To ensure the model is robust, 10-fold cross-validation was performed on the training set.

* **Average Accuracy**: **96.70%**
* **Standard Deviation**: **1.97%**

This high accuracy and low standard deviation indicate that the model is both highly accurate and stable across different subsets of the data.

---
