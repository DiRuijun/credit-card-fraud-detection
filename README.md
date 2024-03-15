# credit-card-fraud-detection 💳

Digital or online banking 🏦 is advantageous since it enables more customer-centric strategies and gives users instant access to banking services. However, this digital revolution has also opened avenues to banking fraud. Lack of customers’ awareness of online security risks makes them vulnerable to divulging confidential data to criminal groups that can be used to authenticate fraudulent transactions. 

Among the many criminal activities occurring in the financial and insurance industry, credit card fraud is the most prevalent. To prevent the losses caused by illegal acts, one of the main approaches is continuous up-gradation of data mining and machine learning. The study aims to identify fraudulent credit card transactions on the given data set using data science solutions.

**Step 1: Exploratory Data Analysis:** Data understanding is critical for feature selection and modelling. Each variable's distribution pattern and skewness is studied to enable necessary data adjustments.

**Step 2 Data Processing:** To study whether data is highly imbalanced between the fraudulent and non-fraudulent. There are four techniques to balance the data, including: under-sampling, oversampling, SMOTE (Synthetic Minority Over Sample Technique), and ADASYN (Adaptive Synthetic). ADASYN was adopted in this study to lower the bias introduced by class imbalance and adaptively shift the classification decision boundary towards complex examples. 

**Step 3 Modeling:** Two classification models (RadomForest and XGBoost) were selected for the study. For XGBoost, the number of trees was indentified based on the accuracy levels. Since data is imbalanced, the ROC curve data was studied to identify the threshold value (above the threshold value is fraudulent and below the threshold is not dishonest). And threshold dependent parameters such as confusion matrix, accuracy, precision, recall, and F-score were calculated. 

**Step 4 Hyperparameter Tuning:** After model building, the next step is hyperparameter tuning, which can be performed through techniques such as cross-validation (CV), grid-search cross-validation, K-Fold cross-validation, stratified K-Fold cross-validation, or train-validation-test splitting. This step is essential to improve accuracy, AUC, and lower misclassification error.

**Step 5 Model evaluation:** To evaluate the model based on AUC-ROC score and define threshold value. The F1 Score, Precision, and Recall were calculated. This will be key for banks to represent the business strategy to bring down the fraud.
