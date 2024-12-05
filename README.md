Synthetic Dataset for Risk Assessment and Loan Approval Modeling

Overview

This project utilizes a synthetic dataset of 20,000 records, designed to support the development of predictive models for risk assessment and loan approval decisions. The dataset includes a wide variety of personal, financial, and demographic features, making it an excellent foundation for data-driven decision-making processes.




Objectives:
Risk Score Prediction (Regression): Predict a continuous risk score reflecting the likelihood of loan default or financial instability.
Loan Approval Prediction (Classification): Classify whether a loan application will be approved or denied.
Dataset Details
The dataset comprises 35 features, providing a comprehensive view of an applicant's financial and personal circumstances:


Key Features:
Demographic Information: Age, marital status, and number of dependents.
Financial Metrics: Annual income, credit score, total assets, liabilities, and monthly income.
Loan-Specific Attributes: Loan amount, duration, purpose, and previous defaults.
Behavioral Data: Payment history, job tenure, and utility bills payment history.
Target Variables:
LoanApproved: Binary classification target (0 = Denied, 1 = Approved).
RiskScore: Continuous regression target for risk assessment.
Project Results
Classification Models:
Models Used:

XGBClassifier
DecisionTreeClassifier
Random Forest Classifier
Top Model Performances:

XGBClassifier: Accuracy = 99.67%
DecisionTreeClassifier: Accuracy = 99.05%
Random Forest: Accuracy = 98.73%
Regression Model:
For the Risk Score Prediction, a linear regression model was applied with the following insights:

The regression model performs well overall, with reasonable predictive accuracy.
The curve in the Actual vs. Predicted Values plot indicates non-linearity in the relationship between features and the target variable.
The residual distribution is centered around zero (a positive indication), but it exhibits right-skewness.
The Q-Q plot shows divergence of residuals above a log value of 1.5 from the theoretical normal line.
The residuals vs. predicted plot exhibits increasing variance at higher predicted values, indicating heteroscedasticity.
Variance Inflation Factor (VIF) values are below 5 for all features, indicating no multicollinearity.
Summary and Future Work
Insights:

The XGBClassifier showed the best performance for loan approval predictions, with an accuracy of 99.67%.
The linear regression model provided meaningful results for risk score prediction but highlighted areas for improvement in addressing heteroscedasticity and non-linearity.
Future Directions:

Test additional models such as Gradient Boosting Regression or Neural Networks for risk score prediction to address non-linear patterns.
Perform advanced feature engineering to reduce heteroscedasticity.
Explore other classification models to refine loan approval predictions.
