**Overview of the Analysis**

- I used a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.
- In this challenge, I used various algorithms to train and evaluate a model based on loan risk to predict the loan status of a loan application (A value of 0 in the “loan_status” column means that the loan is healthy, while a value of 1 means that the loan has a high risk of defaulting).
- I used the following three algorithms:
  - **Logistic Regression**:  a statistical method used for binary classification tasks, where the goal is to predict the probability that an instance belongs to a 
    particular class. Despite its name, logistic regression is a classification algorithm rather than a regression algorithm.
  - **Support Vector Machines (SVM)**: SVM is a powerful supervised learning algorithm used for classification tasks. It works by finding the hyperplane that best separates 
    classes in the feature space. SVMs are effective in high-dimensional spaces and are versatile due to the various kernel functions available.
  - **K-Nearest Neighbors (KNN)**: KNN is a simple, instance-based learning algorithm where the prediction is made based on the majority class among the k nearest neighbors 
    of a given data point in the feature space.


**Results**
- Logistic Regression model:
  - Accuracy - 0.99
  - Precision for label 0 (healthy loan) is 1.00, and for label 1 (high-risk loan) is 0.85.
  - Recall for label 0 is 0.99, and for label 1 is 0.91.
                           
- SVM model:
  - Accuracy - 0.99
  - Precision for label 0 is 1.00, and for label 1 is 0.84.
  - Recall for label 0 is 0.99, and for label 1 is 0.99.
    
- KNN model:
  - Accuracy - 0.99
  - Precision for label 0 is 1.00, and for label 1 is 0.84.
  - Recall for label 0 is 0.99, and for label 1 is 0.97.


**Summary**
- All three models perfrom very well with high precision and recall scores for predicting healthy loans (label 0).
- For predicting high-risk loans (label 1), SVM and KNN have higher recall comapred to Logistic Regression.
- SVM has the highest recall for label 1, followed closely by KNN, indicating that these models are better at identifying high-risk loans.
- The goal is to identify the creditworthiness of borrowers, which means correctly identifying high-risk loans (label 1) is crucial.
- Based on the provided results, Support Vector Machine (SVM) appears to perform the best for this task, as it has the highest recall for label 1, indicating its ability 
  to correctly identify high-risk loans.
- Therefore, I recommend using the Support Vector Machine (SVM) model for predicting the creditworthiness of borrowers.
  
