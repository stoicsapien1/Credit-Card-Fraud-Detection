# Credit Fraud Detection

## Project Overview
This project focuses on detecting fraudulent transactions in a credit card dataset. The dataset is highly imbalanced, with fraudulent transactions being a small percentage of the total dataset. The objective is to build a model that can accurately identify fraudulent transactions despite the imbalance.

## Dataset
The dataset used is the Credit Card Fraud Detection dataset, which contains 284,807 transactions with 30 features and a binary class label indicating whether the transaction is fraudulent or not. Key features include:

- **Time**: The time of the transaction
- **Amount**: The amount of the transaction
- **V1-V28**: Anonymized features resulting from a PCA transformation

## Data Exploration
- **Distribution of Classes**: The dataset is highly imbalanced with 99.83% of transactions being non-fraudulent and only 0.17% being fraudulent.
- **Feature Analysis**: Visualization of distributions for transaction time and amount, as well as correlation analysis between features.

## Data Preprocessing
1. **Scaling**: StandardScaler and RobustScaler were used to scale the `Amount` and `Time` features to improve model performance.
2. **Handling Imbalance**: SMOTE (Synthetic Minority Over-sampling Technique) was applied to balance the dataset by generating synthetic samples of the minority class.

## Model Building and Evaluation
Several classification models were evaluated, including:
- **Logistic Regression**
- **Decision Tree Classifier**
- **Random Forest Classifier**
- **Bagging Classifier**

The models were evaluated using metrics such as accuracy, precision, recall, F1 score, and confusion matrix to assess their performance on both training and test datasets.

## Results
- **Accuracy**: Achieved high accuracy across all models, but special attention was given to metrics like precision and recall due to class imbalance.
- **Confusion Matrix**: Detailed confusion matrices were analyzed to understand the false positives and false negatives.
- **Classification Report**: A comprehensive report was generated to summarize the performance of each model.

## Conclusion
The project successfully demonstrated how to handle imbalanced data and build a robust fraud detection model. The application of SMOTE and various classification algorithms showed promising results in detecting fraudulent transactions.

## Future Work
- **Model Tuning**: Further hyperparameter tuning and advanced techniques like ensemble methods could be explored.
- **Additional Features**: Incorporating additional features or external data could enhance model performance.

## References
- [Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets?search=credit+card+fraud)
- [SMOTE Documentation](https://imbalanced-learn.org/stable/references/generated/imblearn.over_sampling.SMOTE.html)

