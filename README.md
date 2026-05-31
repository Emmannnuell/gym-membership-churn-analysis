# Predicting Gym Membership Churn with Machine Learning 🏋️‍♂️

## 🎯 The Challenge
Customer retention is a critical growth driver for subscription-based businesses. The objective of this project was to analyze member behavior and build a predictive classification model to identify users at risk of canceling their gym membership (churn). Proactively anticipating this behavior allows management to execute targeted, data-driven loyalty strategies to reduce churn rates and secure recurring revenue.

## 🛠️ The Process
I approached this problem by executing a full data science workflow, from data exploration to model deployment:

* **Data Cleaning & Exploration (EDA):** Used **Pandas** and **NumPy** to preprocess historical member data, handle anomalies, and engineer behavioral features. 
* **Data Visualization:** Built correlation matrices and distribution plots using **Matplotlib** and **Seaborn** to uncover patterns between customer profiles and cancellation rates.
* **Model Training & Evaluation:** Implemented and compared classification algorithms (**Random Forest** and **Logistic Regression**) using **Scikit-Learn**. Tuned hyperparameters to optimize the balance between precision and recall (F1-score).

## 📈 Key Insights & Results
### Behavioral Drivers of Churn:
* **Attendance Frequency:** Members averaging fewer than 2 visits per week in the last month showed a drastically higher probability of churning.
* **Contract Type:** Month-to-month contracts were highly volatile and served as the strongest predictor of cancellation compared to annual plans.
* **Engagement:** Low utilization of additional gym services (such as group classes or cafe purchases) strongly correlated with member dropouts.

### Model Performance & Business Impact:
After evaluating the models, **Random Forest** was selected due to its superior performance:
* **Accuracy:** 92%
* **F1-Score (Churn Class):** 0.85

> **🚀 Business Impact:** By leveraging this model, the gym can accurately identify **85% of at-risk members** before they finalize their cancellation, enabling the marketing and support teams to launch proactive retention campaigns.

## 📂 Repository Structure
* `churn.ipynb`: Complete Jupyter Notebook containing EDA, data preprocessing, feature engineering, and model training/evaluation.
* `datasets/`: Folder containing the processed historical data used for the analysis.
