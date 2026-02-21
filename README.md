# Customer Churn Prediction in E-commerce

## Project Overview
Customer churn is a major business challenge, as retaining existing customers is more cost-effective than acquiring new ones. This capstone project focuses on predicting customer churn using machine learning techniques by analyzing customer demographics, service usage, and account-related information.

The project demonstrates a complete end-to-end data science workflow, covering Exploratory Data Analysis (EDA), data preprocessing and feature engineering, and model training with evaluation and comparison.

---

## Business Objective
The primary objective of this project is to identify customers who are likely to churn so that businesses can take proactive retention actions. By improving churn prediction accuracy, the project aims to support data-driven decision-making and reduce potential revenue loss.

---

## Dataset Summary

| Column | Meaning | Explanation |
|--------|---------|-------------|
| Age | Customer’s age in years | - |
| Gender | Customer’s gender | Male / Female / Other |
| Country | Country where the customer resides | - |
| City | City of the customer | - |
| Membership_Years | Number of years the customer has been registered on the platform | - |
| Login_Frequency | How often the customer logs into the platform | Number of logins in a given time period |
| Session_Duration_Avg | Average time a customer spends per session | In minutes |
| Pages_Per_Session | Average number of pages viewed per visit | - |
| Cart_Abandonment_Rate | Percentage of times a customer adds items to cart but does not complete the purchase | - |
| Wishlist_Items | Number of items the customer has added to their wishlist | - |
| Total_Purchases | Total number of completed purchases made by the customer | - |
| Average_Order_Value | Average monetary value spent per order | - |
| Days_Since_Last_Purchase | Number of days since the customer last made a purchase | - |
| Discount_Usage_Rate | Percentage of purchases where the customer used a discount or coupon | - |
| Returns_Rate | Percentage of orders returned by the customer | - |
| Email_Open_Rate | Percentage of marketing emails opened by the customer | - |
| Customer_Service_Calls | Number of times the customer contacted customer support | - |
| Product_Reviews_Written | Number of product reviews written by the customer | - |
| Social_Media_Engagement_Score | Score representing how much the customer interacts with the brand on social media | - |
| Mobile_App_Usage | Measure of how actively the customer uses the mobile application | - |
| Payment_Method_Diversity | Number of different payment methods used by the customer | e.g., credit card, UPI, PayPal, etc. |
| Lifetime_Value | Total revenue generated from the customer since signup | - |
| Credit_Balance | Remaining store credit or wallet balance of the customer | - |
| Churned | Target variable | 1 = Customer stopped using the platform, 0 = Customer is still active |
| Signup_Quarter | Quarter of the year in which the customer signed up | Q1, Q2, Q3, Q4 |

---

## Project Structure
The project is organized into the following notebooks:

- **EDA.ipynb**: Exploratory Data Analysis  
- **Data_Preprocessing.ipynb**: Data cleaning, encoding, and feature preparation  
- **Model_Training.ipynb**: Model development, tuning, and evaluation  

---

## Exploratory Data Analysis (EDA)
The EDA phase focuses on understanding the dataset and identifying patterns related to customer churn. Key activities include analyzing customer demographics, service usage behavior, and churn distribution. Visualizations and summary statistics are used to identify trends and class imbalance.

**Key Insights from EDA:**
- Churn customers exhibit distinct behavioral patterns, particularly in tenure, billing behavior, and service usage.
- Presence of class imbalance highlights the need for careful model evaluation, especially for recall-focused metrics.

---

## Data Preprocessing and Feature Engineering
The preprocessing phase prepares the data for machine learning by:

- Handling missing values  
- Encoding categorical variables  
- Scaling numerical features  

Proper train-test separation is maintained to prevent data leakage. This ensures the dataset is clean, consistent, and suitable for model training, improving both model stability and predictive performance.

---

## Model Training and Evaluation
Multiple machine learning models are trained and evaluated to compare performance:

- **Logistic Regression** (baseline, balanced, and tuned)  
- **Random Forest**  
- **AdaBoost**  
- **Gradient Boosting** (tuned)  

**Evaluation Metrics:**  
Accuracy, Precision, Recall, F1-score, and Confusion Matrices.  
Special emphasis is placed on recall and F1-score due to the business importance of correctly identifying churn customers.

---

## Best Model Result
- **Tuned Gradient Boosting** delivers the best overall performance.  
- Provides a strong balance between precision and recall.  
- Minimizes false negatives, making it the most suitable model for real-world churn prediction scenarios.

---

## Model Comparison Summary
- **Logistic Regression:** Strong baseline, interpretable, moderate performance.  
- **Random Forest:** Robust results, slightly outperformed by Gradient Boosting.  
- **AdaBoost:** Focuses on misclassified churn cases, improves predictions.  
- **Ensemble Models:** Generally outperform simpler approaches.

---

## Key Business Insight
Tuned Gradient Boosting provides reliable churn predictions, enabling early identification of at-risk customers and supporting effective, data-driven retention strategies.

---

## Tools and Technologies
- **Python**  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn  
- **Environment:** Jupyter Notebook
