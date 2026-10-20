# 🚗 Ride Hailing Analytics | Power BI

An interactive Power BI report that analyzes **100K ride-hailing trips** over one year to track revenue, ride outcomes, demand patterns, and customer satisfaction against a target success rate.

## 📌 Project Overview

A ride-hailing company wants to monitor how well its service performs and when demand is highest. This project analyzes **100K rides, 9,000 customers, and 900 drivers** between **October 18, 2023 and October 17, 2024** to answer questions such as:

- What share of rides is completed successfully, and are we reaching the 90% target?
- How many rides end as cancellations or no-shows?
- How do rides and revenue change by quarter?
- Which days of the week have the highest demand?
- How does surge pricing relate to rides and revenue?
- How satisfied are customers with their rides?

## 🎯 Objectives

- Track the main operational KPIs in one clear, interactive report.
- Measure the ride success rate against a 90% target.
- Identify demand and revenue patterns over time and across days of the week.
- Understand customer satisfaction through rating distribution.
- Let users filter the report by day, fare type, ride status, and date.

Ride_Hailing_Analytics_PowerBI/
├── ride_hailing_project.pbix
├── images/
│   └── 01-ride-hailing-report.png
└── README.md

## 📊 Report Features

The report is a single interactive page with four filters:

| Filter | Options |
|---|---|
| Day Filter | Day of the week |
| Is Surge | Normal Fare / Surge |
| Ride Status | Completed / Canceled / No-show |
| Date Filter | Date range slider |

| Visual | What it shows |
|---|---|
| Success Rate gauge | Ride success rate against the 90% target |
| KPI cards | Number of rides, customers, drivers, total actual revenue, and ride hours |
| Rides and Revenue by Year and Quarter | Combined column and line chart of rides and total actual revenue |
| Number of Rides by Day | Demand pattern across the days of the week |
| Customer Satisfaction Rate | Share of rides by customer rating (1 to 5) |

## 🔍 Key Findings

- **The ride success rate is 85.07%, below the 90% target**, a gap of about 5 percentage points and the main operational opportunity.
- **Scale:** 100K rides, 9,000 customers, and 900 drivers generated **$1.62M in revenue** and **38.74K ride hours**, about 11 rides per customer and 111 rides per driver.
- **Stable quarterly performance:** each full quarter in 2024 (Q1 to Q3) recorded about **25K rides** and **$401K to $408K in revenue**.
- **Demand is evenly spread across the week**, with 14K to 15K rides on every day and Thursday slightly ahead.
- **Customers are generally satisfied:** **70% of rides are rated 4 or 5 stars** (40% rated 4 and 30% rated 5), while 15% are rated 1 or 2 stars.

## 🗃️ Data Model

The report uses a simple model built around one fact table:

| Table | Purpose |
|---|---|
| ride_hailing_dataset | Ride-level data: date, day, surge flag, ride status, customer rating, and ride details |
| Dim_Date | Date dimension used for year, quarter, month, and day analysis |
| _Measures | Table that stores the DAX measures |

**DAX measures:** Number of Rides, Number of Customers, Number of Drivers, Total Actual Revenue, Number of Ride Hours, Success Rate %, and Target.

## 🛠️ Tech Stack

- **Power BI Desktop**: data modeling, interactive visuals, slicers, and gauge KPI
- **DAX**: KPI and success rate measures
- **Data modeling**: fact table, date dimension, and a dedicated measures table

## 🚀 How to Use

1. Download or clone this repository.
2. Open `ride_hailing_project.pbix` using Power BI Desktop.
3. The data is embedded in the file, so no external data source is required.
4. Use the Day, Is Surge, Ride Status, and Date filters to explore the report.

## ⚠️ Limitations & Next Steps

- **Both Q4 periods are partial.** The data runs from October 18, 2023 to October 17, 2024, so Q4 2023 (21K rides) and Q4 2024 (5K rides, $77K) cover only part of the quarter. The drop in the last quarter reflects the data cut-off, not a real decline.
- The report is a single page, so there is room to go deeper on **cancellations and no-shows**, the **effect of surge pricing** on revenue, and **driver-level performance**.
- Possible extensions: a ride demand forecast by hour and day, analysis of peak hours, and customer segmentation by ride frequency.



## 🖼️ Dashboard Screenshot

![Ride Hailing Report](images/%F0%9F%9A%96%20Ride%20Hailing%20Analytics%20Project%20%20Power%20BI.PNG)



## 👩‍💻 Author

**Sohair Samer Yehia**: Data Analyst

- [LinkedIn](https://www.linkedin.com/in/sohair-samer)
- [GitHub](https://github.com/Sohairsamer11)
