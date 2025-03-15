# Credit Risk Analysis for Extending Bank Loans

## 📌 Objective
The goal of this project is to analyze bank loan data and predict the likelihood of loan default using machine learning techniques. By leveraging models such as Random Forest, Support Vector Machine (SVM), and Logistic Regression, we aim to provide insights into credit risk assessment and improve decision-making for loan approvals.

## 📂 Dataset
**Dataset Source:** [Kaggle - Credit Risk Analysis for Extending Bank Loans](https://www.kaggle.com/datasets/atulmittal199174/credit-risk-analysis-for-extending-bank-loans)

### 📊 Features:
- **Age**: Age of the borrower.
- **Income**: Annual income of the borrower.
- **DebtInc**: Debt-to-income ratio.
- **Other Features**: Additional financial parameters.
- **Default (Target Variable)**: Indicates whether the borrower defaulted (1) or not (0).

## 📖 Theory
Credit risk analysis is essential in the banking sector to mitigate losses from non-performing loans. Machine learning models can help identify high-risk borrowers by analyzing historical data and detecting patterns associated with defaults.

- **Random Forest:** An ensemble method that uses multiple decision trees to improve prediction accuracy and prevent overfitting.
- **Support Vector Machine (SVM):** A classification algorithm that finds the optimal hyperplane to separate defaulters from non-defaulters.
- **Logistic Regression:** A statistical method used for binary classification problems like predicting loan defaults.

## 🔍 Exploratory Data Analysis (EDA)
- Checked for missing values and handled them by removing nulls.
- Analyzed distributions of features such as income and debt-to-income ratio.
- Visualized relationships between different features using `matplotlib` and `seaborn`.

## 🛠️ Implementation Steps
1. **Load Data:** Read the dataset and inspect its structure.
2. **Preprocess Data:** Handle missing values and standardize numerical features.
3. **EDA:** Generate insights using statistical summaries and visualizations.
4. **Train-Test Split:** Split data into 80% training and 20% testing sets.
5. **Feature Scaling:** Standardize input features using `StandardScaler`.
6. **Train Models:** Train Random Forest, SVM, and Logistic Regression models.
7. **Hyperparameter Tuning:** Optimize SVM using `GridSearchCV`.
8. **Evaluate Models:** Assess performance using accuracy, confusion matrices, and cross-validation.
9. **Prediction Function:** Implement a function to predict the probability of loan default for new applicants.

## 📊 Model Evaluation
The models were compared using accuracy scores and cross-validation:
- **Random Forest Accuracy:** Achieved competitive accuracy with feature importance analysis.
- **SVM Accuracy:** Tuned with grid search for optimal performance.
- **Logistic Regression Accuracy:** Used for baseline comparison.

## 📌 Example Usage
```python
# Predict default probability for new customers
new_customers = pd.DataFrame({
    'age': [35, 42, 28],
    'income': [60000, 82000, 45000],
    'debtinc': [15.2, 8.7, 23.4]
    # Add all required features
})
predictions = predict_default_probability(new_customers)
print(predictions)
```

## 📜 Conclusion
This project demonstrates the effectiveness of machine learning in credit risk assessment. By leveraging different models, we can enhance the accuracy of loan default predictions, aiding financial institutions in making informed lending decisions.

## 🔗 Dependencies
- Python 3.x
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

## 📢 Acknowledgments
- Dataset sourced from [Kaggle](https://www.kaggle.com/datasets/atulmittal199174/credit-risk-analysis-for-extending-bank-loans).

## 🤝 Contributions
Feel free to contribute by optimizing the models, adding new features, or improving the analysis!

