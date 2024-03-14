# credit-card-fraud-detection

Digital or online banking is advantageous since it enables more customer-centric strategies and gives users instant access to banking services. However, this digital revolution has also opened avenues to banking fraud. Lack of customers’ awareness of online security risks makes them vulnerable to divulging confidential data to criminal groups that can be used to authenticate fraudulent transactions. 

Among the many criminal activities occurring in the financial and insurance industry, credit card fraud is the most prevalent. To prevent the losses caused by illegal acts, one of the main approaches is continuous up-gradation of data mining and machine learning. The study aims to identify fraudulent credit card transactions on the given data set using data science solutions.

**Step -1**: Load the data to understand it. Data understanding is critical since we will select the subset of features to carry out model training, and it includes types of data and its patterns. 

**Step -2**: Exploratory Data Analysis Study histogram to compare each variable’s data distribution pattern and skewness of the data. Make necessary data adjustments to avoid any problems while we train the model. 

**Step -3**: Class imbalance Study whether data is highly imbalanced between the fraudulent and non-fraudulent. We have learned four techniques to balance the data using various methods: Under-sampling, oversampling, 2 SMOTE (Synthetic Minority Over Sample Technique), and ADASYN (Adaptive Synthetic). We will use ADASYN techniques to lower the bias introduced by class imbalance and adaptively shift the classification decision boundary towards complex examples. 

**Step -4**: Data modeling and model selection We will use two classification models (RadomForest and XGBoost) for the current study. For XGBoost, we will identify the number of trees based on the accuracy levels. We will not use KNN since the data set are more than 10K (computation time is increased if data sets are more than 10K). The decision tree gives an interpretation of the flow chart. Hence, it is widely used, but we do not know when to stop building trees and tend to overfit. We will use parameters such as confusion matrix, accuracy, precision, recall, and F-score, threshold dependent. Since data is imbalanced, we will also perform a deep dive into the ROC curve data to identify the threshold value (above the threshold value is fraudulent and below the threshold is not dishonest). We will calculate the F1 score, Precision, and Recall.

**Step -5**: Hyperparameter Tunings the model At this time, we will have the best understanding of the type of data we have and the kind of model we were going to build. After model building, our next step will be either hyperparameter tunings (CV or Cross-validation) or grid-search cross-validation or K-Fold or stratified K-Fold, or train validation and test split. This step is essential to improve accuracy, AUC, and lower misclassification error.

**Step -6**: Model evaluation Evaluate the model based on AUC -ROC score, through which we will define the threshold value. We will calculate the F1 Score, Precision, and Recall. This will be key for banks to represent the business strategy to bring down the Fraud.
