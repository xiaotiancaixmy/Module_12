# Module_12
## Credit Risk Analysis Report
We evaluated two logistic regression models on credit risk assessment data: one trained on the original data and the other on oversampled data. Our analysis focused on model performance, specifically accuracy, precision, and recall, as well as the impact of oversampling as a technique to handle imbalanced datasets.

1. Analysis of the Logistic Regression Model with Original Data:
The logistic regression model trained on original data exhibited high proficiency in predicting healthy loans, demonstrated by a perfect precision score of 1.00 and a near-perfect recall score of 0.99. This indicates that the model was nearly flawless in identifying and predicting healthy loans.

However, when predicting high-risk loans, the model had a precision of 0.85 and a recall of 0.91. This indicates that the model correctly predicted high-risk loans 85% of the time when it classified a loan as high-risk and correctly identified 91% of all actual high-risk loans.

Despite this, there were certain limitations in the model's ability to predict high-risk loans, primarily due to the imbalance in the training data. The model's overall accuracy was 99.2%, which, while high, may not fully reflect its ability to accurately predict the minority class (high-risk loans) due to the skew in the dataset towards the majority class (healthy loans).

2. Analysis of the Logistic Regression Model with Oversampled Data:
To counteract the imbalance in the original dataset, we utilized a random oversampling technique on the minority class and trained a logistic regression model on this resampled data.

The model's precision for predicting high-risk loans was 0.84, indicating that it was correct 84% of the time when it classified a loan as high-risk. The recall for high-risk loans significantly improved to 0.99, meaning the model was able to correctly identify 99% of all actual high-risk loans in the dataset, a substantial improvement over the previous model.

The oversampling technique resulted in a slight increase in the model's overall accuracy to 99.38%. This approach managed to reduce the bias towards the majority class in the original data, and the model demonstrated a better ability to classify high-risk loans. However, there was a slight increase in the number of healthy loans that were incorrectly classified as high-risk.

Conclusion:
In conclusion, both logistic regression models were proficient in credit risk prediction, but the model trained on oversampled data showed a marked improvement in identifying high-risk loans. The oversampling technique effectively mitigated the imbalance in the training data, thus enhancing the model's predictive ability for the minority class. However, the trade-off between increased detection of high-risk loans and a slight rise in misclassification of healthy loans as high-risk is a factor that needs to be considered.

For future work, other resampling techniques or alternative machine learning models can be explored to improve predictive performance further, with a specific focus on optimizing the balance between identifying true high-risk loans and minimizing false alarms.