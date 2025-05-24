# 📊 Churn Prediction Project — ETL, Dashboard & ML Model

## 🎯 Project Objective

1. To design a complete ETL pipeline, develop a Power BI dashboard, and build a machine learning model to:

2. Analyze customer data across demographic, geographic, service, and financial dimensions.

3. Identify churn drivers and customer segments prone to churn.

4. Predict future churners using a Random Forest model for proactive decision-making.

## 🔧 Tech Stack

1. SQL Server (ETL, Data Cleaning, Views)

2. Power BI (Data Transformation, Dashboarding)

3. Python with Random Forest (Churn Prediction Model)

## 🧩 Project Components

### ✅ STEP 1: ETL Process in SQL Server

1. Created db_Churn and staging table using SSMS Import Wizard.

2. Handled nulls, datatype mismatches (e.g., converting BIT to VARCHAR(50)).

3. Performed exploratory SQL analysis (e.g., churn breakdown by gender, contract, state).

4. Loaded cleaned data into prod_Churn table.

5. Created SQL views (vw_ChurnData, vw_JoinData) for downstream Power BI usage.

### ✅ STEP 2: Data Modeling in Power BI

1. Added calculated columns:

    Churn Status (binary label)

    Monthly Charge Range, Age Group, and Tenure Group

2. Created mapping tables with sorting logic for age and tenure cohorts.

3. Unpivoted service columns for detailed service-level churn analysis.

4. Applied DAX to create key performance metrics:

    Total Customers

    Total Churn & Churn Rate

    New Joiners

### ✅ STEP 3: Machine Learning with Random Forest (Python)

-> Extracted cleansed data from SQL Server.

-> Performed feature engineering and one-hot encoding.

-> Trained a Random Forest Classifier to predict churn likelihood.

-> Model Evaluation Results:

Confusion Matrix:

[[783    64]

[126    229]]

Classification Report:

![image](https://github.com/user-attachments/assets/9630a932-d23a-4d04-9048-cf02d6c06891)

Overall metrics:

    Accuracy: 0.84

    Macro Avg: Precision=0.82, Recall=0.78, F1=0.80

    Weighted Avg: Precision=0.84, Recall=0.84, F1=0.84

-> Identified key churn indicators using feature importance.

-> Integrated model insights back into Power BI for decision support.

### 📈 Business Impact

-> Built an interactive Power BI dashboard for leadership to:

-> Explore churn across age, geography, service type, and revenue metrics.

-> Identify high-risk segments and marketing opportunities.

-> Enabled proactive retention strategy by predicting future churners with high accuracy.

## Output

![image](https://github.com/user-attachments/assets/37fbdd12-9256-4d23-98a2-02106759c0ff)

![image](https://github.com/user-attachments/assets/ba43569f-1d6c-489b-96ce-9432d3ed36fd)

## Output Explanation



