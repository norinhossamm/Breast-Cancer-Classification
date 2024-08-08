# Breast Cancer Wisconsin

This project focuses on the classification of breast cancer into malignant or benign categories, utilizing machine learning techniques to enhance diagnostic accuracy and support healthcare professionals in making informed decisions.

**Technologies Used**: Logistic Regression - Decision Tree - XGBoost - SVC 

## Breast Cancer Wisconsin (Diagnostic) Dataset

The Breast Cancer Wisconsin (Diagnostic) dataset comprises 569 samples derived from digitized images of fine needle aspirates of breast masses. Each sample includes 30 features capturing the characteristics of cell nuclei, such as radius, texture, perimeter, area, and smoothness, among others. These features are calculated in three forms: mean, standard error, and "worst" (the mean of the three largest values), ensuring a comprehensive dataset with high precision. This rich dataset, free of missing values, is balanced with 357 benign and 212 malignant cases, available via the UCI Machine Learning Repository. It provides a crucial resource for developing machine learning models to classify breast cancer more accurately.

<div align=center>
<img width="600" alt="Screenshot 2024-08-08 at 6 00 48 PM" src="https://github.com/user-attachments/assets/ab3e8c84-fe41-4302-b54a-6a7a1433c0d1">
</div>

## Data Processing and Feature Engineering:

- ID Removal: The 'ID' attribute was removed to prevent it from being erroneously used in the predictive model, as it provides no informational value regarding the diagnosis.

- Encoding Target Variable: The categorical target variable 'Diagnosis', initially labeled as 'B' (Benign) and 'M' (Malignant), was converted to a binary format with '0' representing Benign and '1' representing Malignant. This conversion facilitates the use of algorithms that require numerical input.

- Feature Correlation Assessment: A thorough examination of the correlation between features and the target variable was conducted to identify any strong correlations that could impact model performance.

<p align="center">
  <img src="https://github.com/user-attachments/assets/9dd81beb-1b72-4d28-8450-c786a1868fbc" alt="Descriptive Alt Text">
</p>


- Visualization of Correlations: Scatter plots were generated to visually explore the relationships between features and the target variable, aiding in the intuitive understanding of data interdependencies.

<p align="center">
  <img src="https://github.com/user-attachments/assets/b395ca8c-4faf-4fa8-b324-73d459f8ad35" alt="Descriptive Alt Text">
</p>

- Dropping Highly Correlated Features: Features exhibiting very high correlation (greater than 0.9) with existing features were dropped to reduce multicollinearity, which can dilute the model's ability to distinguish between independent predictors.

![image](https://github.com/user-attachments/assets/fb343837-33d2-4122-a156-1c87f3b3c716)

## Evaluation Metrics:

- Accuracy: Measures the overall correctness of the model.
  
- Confusion Matrix: Visualizes the accuracy of predictions across actual and predicted classifications, highlighting the counts of true positives, true negatives, false positives, and false negatives.
  
- Classification Report: Provides precision, recall, and F1-score for a detailed assessment of model performance across different classes.

<div align=center>
<div style="display: flex; justify-content: center; width: 100%; margin-bottom: 10px; padding-left: 20px;">
  <img width="300" alt="Screenshot 2024-08-08 at 6 15 01 PM" src="https://github.com/user-attachments/assets/36bfbaef-3dd2-43bc-864c-4df83492504e" style="margin-right: 10px;">
  <img width="300" alt="Screenshot 2024-08-08 at 6 15 44 PM" src="https://github.com/user-attachments/assets/4b37cfe9-3bda-44fb-853b-6075dd4054c1">
</div>
<div style="display: flex; justify-content: center; width: 100%; padding-left: 20px;">
  <img width="300" alt="Screenshot 2024-08-08 at 6 16 17 PM" src="https://github.com/user-attachments/assets/babd04b5-dedf-427b-ba03-845d9109308e" style="margin-right: 10px;">
  <img width="300" alt="Screenshot 2024-08-08 at 6 16 37 PM" src="https://github.com/user-attachments/assets/4469f3cc-54ba-42a9-b0ac-603b0ae5da70">
</div>
</div>

## Results and Conclusion:

In this project, four different models were evaluated: Logistic Regression, Decision Tree, XGBoost, and SVC. The Support Vector Classifier (SVC) demonstrated the highest overall performance with an accuracy of 97.4%, along with excellent precision, recall, and F1-scores of 0.98, 0.97, and 0.97, respectively. Logistic Regression also performed well, achieving an accuracy of 96.5%. XGBoost and Decision Tree models followed closely with accuracies of 95.6% and 93.9%, respectively. Given SVC's superior performance, it was chosen for further fine-tuning. However, evaluations revealed that the default hyperparameters provided the best results, affirming the initial model setup's efficacy.


<div align=center>
<img width="624" alt="Screenshot 2024-08-08 at 6 37 04 PM" src="https://github.com/user-attachments/assets/a3505723-384b-400a-b15a-79b3b4c9f79a">
</div>

In conclusion, the breast cancer classification project effectively demonstrated the potential of machine learning in medical diagnostics. The SVC model, with its exceptional accuracy of 97.4%, proved to be the most effective tool in distinguishing between benign and malignant breast tumors. The findings affirm that even with basic configurations, advanced algorithms like SVC can deliver robust and reliable predictions. This project not only enhances our understanding of algorithmic applications in healthcare but also sets a benchmark for future diagnostic improvements, highlighting the critical role of precision and accuracy in medical outcomes.



