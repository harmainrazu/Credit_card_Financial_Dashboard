# Credit_card_Financial_Dashboard

![CREDIT CARD LOGO](https://www.google.com/imgres?q=credit%20card%20logo&imgurl=http%3A%2F%2Fwww.credit-card-logos.com%2Fimages%2Fmastercard_credit-card-logos%2Fmastercard_logo_5.gif&imgrefurl=http%3A%2F%2Fwww.credit-card-logos.com%2F&docid=bOh20XWEFR57oM&tbnid=IKnD3g-5pg1LwM&vet=12ahUKEwiqzdrw3rCLAxWscmwGHRiVMm4QM3oECEIQAA..i&w=216&h=133&hcb=2&ved=2ahUKEwiqzdrw3rCLAxWscmwGHRiVMm4QM3oECEIQAA)


Credit Card Transaction and Customer Dashboard using Power BI

## PROJECT OBJECTIVE:

To develop a comprehensive credit card weekly dashbooard thst provides real-time insights into key performance 
metrics and trends, enabling stakeholders to monitor and analyze credit card operations effectively. 




## SQL query;

-- SQL Query to create and import data from csv files:

-- 0. Create a database 
CREATE DATABASE ccdb;

-- 1. Create cc_detail table

```sql

CREATE TABLE cc_detail (
    Client_Num INT,
    Card_Category VARCHAR(20),
    Annual_Fees INT,
    Activation_30_Days INT,
    Customer_Acq_Cost INT,
    Week_Start_Date DATE,
    Week_Num VARCHAR(20),
    Qtr VARCHAR(10),
    current_year INT,
    Credit_Limit DECIMAL(10,2),
    Total_Revolving_Bal INT,
    Total_Trans_Amt INT,
    Total_Trans_Ct INT,
    Avg_Utilization_Ratio DECIMAL(10,3),
    Use_Chip VARCHAR(10),
    Exp_Type VARCHAR(50),
    Interest_Earned DECIMAL(10,3),
    Delinquent_Acc VARCHAR(5)
);


-- 2. Create cc_detail table

CREATE TABLE cust_detail (
    Client_Num INT,
    Customer_Age INT,
    Gender VARCHAR(5),
    Dependent_Count INT,
    Education_Level VARCHAR(50),
    Marital_Status VARCHAR(20),
    State_cd VARCHAR(50),
    Zipcode VARCHAR(20),
    Car_Owner VARCHAR(5),
    House_Owner VARCHAR(5),
    Personal_Loan VARCHAR(5),
    Contact VARCHAR(50),
    Customer_Job VARCHAR(50),
    Income INT,
    Cust_Satisfaction_Score INT
);
```

--Then import data from excel.csv file into the SQL.



