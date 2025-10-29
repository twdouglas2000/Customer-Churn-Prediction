_Customer Churn Prediction_ (Python, NumPy, Pandas, R, Scikit-learn, Logistic Regression, SVM)

**Project Overview**

This project focused on developing machine learning models (Logistic Regression and Support Vector Machine) in Python and R to predict customer churn using telecommunications data.

The primary goal was to maximize model recall for the "Churner" class, prioritizing the identification of at-risk customers (minimizing false negatives). This approach allows the business to implement proactive retention strategies to prevent missed opportunities and lost revenue.

**Data Source and Preparation**

The model was trained on customer telecommunications data from a provided 2024 dataset.

**Preprocessing Highlights**

Binarization: Customer demographic and service data were preprocessed and binarized to standardize the data and enhance model performance.

Continuous Data: Continuous features, such as tenure and MonthlyCharges, were converted into binary features based on whether the values were above or below the median.

Feature Selection: The multicollinear features TotalCharges and PhoneService were intentionally removed to prevent redundancy and potential model overfitting.

**Methodology and Results**

Multiple classification models were developed and compared across Python (Scikit-learn) and R (glmnet) environments. The Python Logistic Regression model was chosen for its optimal balance of strong performance and interpretability.

Model	Recall (Customers Who Will Churn);	Precision (Customers Who Will Churn);	Overall Accuracy

Python Logistic Regression (Strongest Model)	57%;	68%;	81%

Python SVM (Sigmoid Kernel)	58%;	66%;	81%

R Logistic Regression (Tuned)	52%;	63%;	79%

**Key Churn Drivers**

The Logistic Regression analysis identified key churn contributors by determining the percentage effect on the odds of attrition:

Fiber Optic Internet Service: Increases churn probability by +148%.

Two-Year Contracts: Decreases churn probability by -85%.

Tenure (Above Median): Decreases churn probability by -54%.

**Business Applications**

The core predictive findings were translated for business applications, yielding concrete recommendations for marketing, sales, and customer service teams:

Customer Service / Product: Implement targeted surveys to investigate and resolve the root mechanical problems associated with the high churn rate from fiber optic service.

Sales / Marketing: Reduce the cost of longer contracts (two-year) to incentivize adoption and market these discounted rates to increase customer acquisition and retention.

Customer Service / Loyalty: Proactively promote offers or loyalty rewards, including personalized messages, targeted toward customers with lower tenure to increase customer loyalty early on.

**Technology Stack**

The predictive analysis and modeling were executed using the following technology stack:

Python: NumPy, Pandas, Scikit-learn (LogisticRegression, SVM).

R: R (tidymodels, glmnet).
