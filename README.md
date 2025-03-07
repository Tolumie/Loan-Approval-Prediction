# **Loan Approval Prediction: EDA + Decision Tree, Random Forest & Logistic Regression Modeling**  

## **Project Overview**  
This project focuses on **automating loan eligibility prediction** for **Dream Housing Finance**, a company that provides home loans across urban, semi-urban, and rural areas. The goal is to **identify customer segments eligible for loan approval** using machine learning models, enabling the company to target potential borrowers effectively.  

## **Problem Statement**  
The company wants to automate the loan approval process based on customer details submitted during the online application. These details include **income, loan amount, credit history, education, marital status, and more**. Given a dataset of past applicants, we analyze the data and build predictive models to classify whether a loan should be approved (`Loan_Status = Y`) or rejected (`Loan_Status = N`).  

## **Dataset Description**  
The dataset consists of customer details relevant to loan eligibility. The key features include:  

| **Variable**          | **Description**                                      |
|----------------------|--------------------------------------------------|
| **Loan_ID**         | Unique identifier for each loan application      |
| **Gender**          | Applicant's gender (Male/Female)                 |
| **Married**         | Marital status (Yes/No)                          |
| **Dependents**      | Number of dependents                             |
| **Education**       | Education level (Graduate/Undergraduate)         |
| **Self_Employed**   | Whether the applicant is self-employed (Yes/No)  |
| **ApplicantIncome** | Applicant's monthly income                      |
| **CoapplicantIncome** | Income of co-applicant                         |
| **LoanAmount**      | Loan amount requested (in thousands)             |
| **Loan_Amount_Term** | Loan term duration (months)                     |
| **Credit_History**  | Whether credit history meets guidelines (1/0)    |
| **Property_Area**   | Area of the property (Urban/Semi-Urban/Rural)    |
| **Loan_Status**     | Loan approval status (Y/N - Target Variable)     |  

## **Project Workflow**  

### **1. Exploratory Data Analysis (EDA)**
- Handling missing values and data inconsistencies  
- Visualizing relationships between features and loan status  
- Analyzing trends based on **income, credit history, and loan amount**  
- Understanding the impact of categorical variables (e.g., Property Area, Education)  

### **2. Feature Engineering & Data Preprocessing**  
- Encoding categorical variables  
- Handling skewness and outliers in numerical variables  
- Scaling features for model compatibility  
- Creating new features (if necessary) to improve predictions  

### **3. Model Development & Evaluation**  
Three machine learning models were implemented:  
✅ **Logistic Regression** – Baseline model to understand linear relationships  
✅ **Decision Tree** – Captures non-linear patterns in loan approval trends  
✅ **Random Forest** – An ensemble model improving accuracy and reducing overfitting  

### **4. Performance Metrics & Model Selection**  
- **Accuracy Score**: Measures overall correctness of predictions  
- **Precision & Recall**: Evaluates model effectiveness in detecting eligible borrowers  
- **Confusion Matrix**: Analyzes classification errors  
- **ROC-AUC Curve**: Assesses model performance in distinguishing approvals vs. rejections  

## **Key Findings & Insights**  
📌 **Credit History** is the strongest predictor of loan approval. Applicants with a **good credit history (1)** have a significantly higher approval rate.  
📌 **Income** and **Loan Amount** show a relationship—higher income applicants tend to receive loan approvals more easily.  
📌 **Marital Status & Dependents** have minor impacts, but self-employed applicants face slightly higher rejection rates.  
📌 **Random Forest performed best**, delivering the highest accuracy and robust classification.  

## **Next Steps**  
🚀 **Hyperparameter tuning** to optimize Decision Tree & Random Forest models  
🚀 **Feature Engineering** to incorporate additional financial indicators  
🚀 **Deploying the model** via a web app for real-time loan approval predictions  

## **Technologies Used**  
🟢 **Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)**  
🟢 **Jupyter Notebook** for data analysis and model development  
🟢 **Machine Learning (Logistic Regression, Decision Tree, Random Forest)**  

## **Conclusion**  
This project successfully **demonstrates the power of machine learning in loan approval prediction**. By leveraging **EDA, feature engineering, and predictive modeling**, we provide insights into customer eligibility, helping Dream Housing Finance **streamline loan processing and target high-potential borrowers efficiently**.
