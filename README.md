# 🏦 Loan Default Prediction using Logistic Regression

This project predicts whether a loan will default or not using logistic regression. It involves data preprocessing, one-hot encoding, feature scaling, model training, and performance evaluation using key metrics and visualization.

---

## 📂 Dataset

The dataset used is:  
**`1. Predict Loan Default.csv`**

It contains information about loans and whether they were defaulted or not.

---

## 🧠 Objective

To build a machine learning model that can accurately classify whether a loan will default based on given features.

---

## ⚙️ Technologies Used

- Python
- Pandas
- Scikit-learn
- Seaborn
- Matplotlib

---

## 📈 Workflow

### 1. **Data Preprocessing**
- The column `LoanID` is dropped as it is only an identifier.
- Categorical variables are converted into numerical format using **One-Hot Encoding** with `drop_first=True` to avoid multicollinearity.

### 2. **Feature and Target Separation**
- Features (`X`) and the target (`y`) are separated. The target variable is `Default`.

### 3. **Feature Scaling**
- Features are standardized using **StandardScaler** to bring all numerical values to the same scale.

### 4. **Train-Test Split**
- The dataset is split into:
  - **70% training data**
  - **30% testing data**
- `random_state=42` ensures reproducibility.

### 5. **Model Training**
- A **Logistic Regression** model is trained on the training data.

### 6. **Prediction**
- Predictions are made on the test set.

### 7. **Evaluation**
- The model's performance is evaluated using:
  - **Accuracy**
  - **Precision**
  - **Recall**
  - **Confusion Matrix**

### 8. **Visualization**
- A **confusion matrix heatmap** is plotted using Seaborn for visual evaluation.

---

## 📊 Output Example

```text
Accuracy: 0.85
Precision: 0.76
Recall: 0.68

[[TN  FP]
 [FN  TP]]
```

## 📝 Conclusion

This project demonstrates a full machine learning pipeline:

-   Clean data → Encode → Scale → Split → Train → Evaluate → Visualize
    

The logistic regression model gives a clear baseline to predict loan defaults. More advanced models (like Random Forest or XGBoost) can be applied for improved performance in future iterations.

----------
