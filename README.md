# credit-card-fraud-detection 💳

Digital or online banking 🏦 is advantageous since it enables more customer-centric strategies and gives users instant access to banking services. However, this digital revolution has also opened avenues to banking fraud. Lack of customers’ awareness of online security risks makes them vulnerable to divulging confidential data to criminal groups that can be used to authenticate fraudulent transactions. 

Among the many criminal activities occurring in the financial and insurance industry, credit card fraud is the most prevalent. To prevent the losses caused by illegal acts, one of the main approaches is continuous up-gradation of data mining and machine learning. The study aims to identify fraudulent credit card transactions on the given data set using data science solutions.

**Step 1: Exploratory Data Analysis:** Data understanding is critical for feature selection and modelling. Each variable's distribution pattern and skewness is studied to enable necessary data adjustments.

**Step 2 Data Processing:** To study whether data is highly imbalanced between the fraudulent and non-fraudulent. There are four techniques to balance the data, including: under-sampling, oversampling, SMOTE (Synthetic Minority Over Sample Technique), and ADASYN (Adaptive Synthetic). ADASYN was adopted in this study to lower the bias introduced by class imbalance and adaptively shift the classification decision boundary towards complex examples. 

**Step 3 Modeling:** Two classification models (RadomForest and XGBoost) were selected for the study. For XGBoost, the number of trees was indentified based on the accuracy levels. Since data is imbalanced, the ROC curve data was studied to identify the threshold value (above the threshold value is fraudulent and below the threshold is not dishonest). And threshold dependent parameters such as confusion matrix, accuracy, precision, recall, and F-score were calculated. 

**Step 4 Hyperparameter Tuning:** After model building, the next step is hyperparameter tuning, which can be performed through techniques such as cross-validation (CV), grid-search cross-validation, K-Fold cross-validation, stratified K-Fold cross-validation, or train-validation-test splitting. This step is essential to improve accuracy, AUC, and lower misclassification error.

**Step 5 Model evaluation:** To evaluate the model based on AUC-ROC score and define threshold value. The F1 Score, Precision, and Recall were calculated. This will be key for banks to represent the business strategy to bring down the fraud.

**CONCLUSION**

Total 5 models were created to detect credit card fraudulent transactions, including Logistics Regression, Random Forest, Neutral Network, Gradient Boosting, Decision Tree and XGBoost.

All the models were evaluated base on different metrics, including Accuracy, Recall, and Precision. The model should strike the right balance between precision and recall, as identifying the fraud precisely is as important as reducing the misidentification of transactions. And the area under the ROC curve plays an important role in the selection of model, as a measure of the classifier's ability to distinguish between positive and negative samples

Model recommendations: (1) Based on the Area under the ROC curve, the **Logistic Regression model** with L2 penalty was considered to be the best with AUC of 0.9862. The Recall of the LR model is 0.9387, and the Precision is 0.9383, which are both quite good values; (2) The **GRB model** also had good peformance with the AUC value of 0.977. The Recall for the LR model is 0.9183, and the Precision is 0.9183 with an accuracy of 0.918, which is very well-balanced for the scenario.
