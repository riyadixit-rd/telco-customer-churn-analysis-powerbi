# 📊 Telco Customer Churn Analysis Dashboard

An interactive **Customer Churn Analysis Dashboard** built using **Microsoft Power BI** to analyze customer retention, churn patterns, contracts, services, payment methods, tenure, and customer behavior.

## 📌 Project Overview

This project analyzes the **Telco Customer Churn dataset** containing customer information and their churn status.

The raw customer data was imported into Power BI and transformed into an interactive dashboard using data analysis, visualization, and DAX measures.

The dashboard helps identify patterns that may be associated with customer churn and provides a quick overview of customer retention performance.

## 🎯 Objectives

- Analyze the overall customer base
- Identify the number of churned customers
- Calculate the overall churn rate
- Compare churn across different contract types
- Analyze churn based on internet service
- Explore churn patterns across customer tenure
- Compare churn across payment methods
- Analyze churn by gender
- Explore the relationship between monthly charges and tenure
- Extract meaningful customer retention insights

## 🛠️ Tools & Technologies

- **Microsoft Power BI**
- **Power Query**
- **DAX**
- **Data Visualization**
- **Data Analysis**

## 📊 Dashboard KPIs

| KPI | Value |
|---|---:|
| Total Customers | 7,043 |
| Churned Customers | 1,869 |
| Churn Rate | 26.54% |

## 📈 Dashboard Visualizations

The dashboard includes:

- **Total Customers**
- **Churned Customers**
- **Churn Rate**
- **Churn by Contract**
- **Churn by Internet Service**
- **Churn by Tenure**
- **Churn by Payment Method**
- **Churn by Gender**
- **Monthly Charges vs. Tenure**

## 💡 Key Insights

- The dataset contains **7,043 customers**.
- **1,869 customers** have churned.
- The overall churn rate is **26.54%**.
- Contract type shows noticeable differences in customer churn.
- Internet service type is an important dimension for analyzing churn.
- Customer tenure shows different patterns between churned and retained customers.
- Payment methods show different churn distributions across customer groups.
- Monthly charges and tenure can be analyzed together to understand customer behavior.

## 🔄 Data Analysis Flow

```text
Telco Customer Churn Dataset
            ↓
      Data Import
            ↓
     Data Exploration
            ↓
      Data Cleaning
            ↓
       Power Query
            ↓
      DAX Measures
            ↓
    Power BI Dashboard
            ↓
    Churn & Retention Insights
```
## 🧮 DAX Measure

The dashboard uses DAX to calculate the overall churn rate:

```DAX
Churn Rate % =
DIVIDE(
    CALCULATE(
        COUNTROWS('Telco-Customer-Churn'),
        'Telco-Customer-Churn'[Churn] = "Yes"
    ),
    COUNTROWS('Telco-Customer-Churn'),
    0
) * 100
```
## 🧠 Skills Practiced

- Data loading and exploration
- Data cleaning and transformation
- Power Query
- DAX measure creation
- KPI development
- Customer churn analysis
- Data aggregation
- Data visualization
- Dashboard design
- Customer retention analysis
- Business insight generation

## 📷 Dashboard Preview

![Telco Customer Churn Dashboard](Screenshot%202026-08-29%20171835.png)

## 📁 Project Files

```text
telco-customer-churn-analysis-powerbi/
│
├── Telco-Customer-Churn-Analysis.pbix
├── README.md
└── Screenshot 2026-08-29 171835.png
```
## 🚀 How to Use

1. Download or clone this repository.
2. Open `Telco-Customer-Churn-Analysis.pbix` using **Microsoft Power BI Desktop**.
3. If required, update the dataset/source settings.
4. Refresh the data.
5. Explore the interactive dashboard and visualizations.

## 📌 Learning Outcome

This project was created as part of my **5-day Data Analytics mini-project sprint**.

Through this project, I gained practical experience in **Power BI, Power Query, DAX, KPI development, data visualization, and customer churn analysis**.

The project helped me understand how raw customer data can be transformed into an interactive dashboard and used to identify patterns that can support customer retention analysis.

## 👩‍💻 Author

**Riya Dixit**

GitHub: [riyadixit-rd](https://github.com/riyadixit-rd)
