# Practical Application 3 - Comparing_Classifiers

## Notebook
[Workbook](https://github.com/krupakmurthy/Comparing_Classifiers/blob/main/prompt_III_final.ipynb)

### Project Overview
This project carriws out comparison of classifiers for a dataset based on Portugese bank which uses telephone for marketing.

### Dataset
- The dataset contains information on marketing campaigns conducted over telephone by a Portuguese banking institution, where the target variable indicates whether a customer subscribed to a long-term deposit.
- The dataset is imbalanced, with approximately 36,548 samples labeled 'no' and 4,640 samples labeled 'yes' (8% success rate).
- Link to the dataset: [Bank_Marketing](https://archive.ics.uci.edu/dataset/222/bank+marketing )

### Process followed
- Addressed imbalance using SMOTEENN - a combination of oversampling and undersampling for better class separation.
- Several models were built and optimized to predict whether a customer would subscribe to a deposit - Logistic Regression, K-Nearest Neighbors, Decision Tree Classifier, Support Vector Classifier
- Used ROC Curve and Accuracy score as the two main evaluation metrics.

### Results and Insights
- The 5 most important features for training are - duration, num_employees, month, euribor_3m_rate and consumer_confidence_index
- Balancing the dataset significantly improved model performance on minority class predictions.
- Hyperparameter tuning enhanced overall accuracy and generalization of the models.
- Out of all, Decision Tree performs the best in terms of test accuracy and training time as well.
- All models provided good results, all with AUC > 0.9.
