# EDA-Hospitality-Domain-Analysis



## Project Overview

This Exploratory Data Analysis (EDA) project investigates **AtliQ Grands**, a hospitality business experiencing performance fluctuations across multiple cities in India. The goal was to uncover **data-driven insights** on hotel performance, occupancy trends, revenue generation, and customer ratings — to support better decision-making for business growth.

## Live Demo

Coming soon — interactive Power BI Dashboard will be linked here.

---

## Technologies Used

**Backend & Data Handling:** Python, Pandas, NumPy
**Visualization:** Matplotlib, Seaborn
**Data Source:** CSV files (Bookings, Hotels, Rooms, Dates, Aggregated Bookings)
**IDE:** Jupyter Notebook

---

## Why These Technologies

Python and its data-analysis ecosystem (Pandas + NumPy) made it efficient to clean, merge, and analyze multiple datasets. Matplotlib and Seaborn were used for powerful yet customizable visual storytelling — perfect for business reports.

---

## Project Structure

```
├── Data/
│   ├── fact_bookings.csv
│   ├── fact_aggregated_bookings.csv
│   ├── dim_hotels.csv
│   ├── dim_rooms.csv
│   ├── dim_date.csv
│   └── new_data_august.csv
│
├── Code/
│   └── hospitality_eda.ipynb
│
└── README.md
```

---

## Key Features

* **Data Cleaning:**
  Removed outliers in revenue and negative guest counts.
  Handled missing values in booking capacity.
* **Data Transformation:**
  Created occupancy rate (%), city-wise, and category-wise metrics.
* **Insights Visualization:**

  * Occupancy % by Room Type and City
  * Revenue Generated & Realized per Room, City, and Platform
  * Month-by-Month Revenue Trends
  * Average Customer Ratings per City
* **Data Merging:**
  Combined data across multiple fact and dimension tables to create a unified analytical dataset.

---

## Challenges Solved

* Fixed data inconsistencies in date formats (`DD-MM-YY` vs `MM/DD/YYYY`).
* Removed outliers in financial metrics using the **3σ (standard deviation)** method.
* Successfully merged multiple datasets (`fact_bookings`, `dim_hotels`, `dim_rooms`, etc.) with different primary keys and naming conventions.
* Repaired duplicated and mismatched columns for August data before concatenation.

---

## Insights Summary

* **Presidential rooms (RT4)** had the highest occupancy and revenue per booking.
* **Delhi** showed the highest average occupancy (~62%), while **Bangalore** lagged slightly (~56%).
* **Weekend bookings** achieved 72% occupancy vs. only 50% on weekdays.
* **Mumbai** contributed the most to total realized revenue (~₹668M).
* **Direct bookings** and **Tripster platform** delivered the highest revenue share.

---

## Future Improvements

* Build an **interactive Power BI dashboard** for executives.
* Automate data ingestion using Python pipelines.
* Integrate **forecasting models** to predict future occupancy trends.
* Add a **SQL layer** for better query-based analytics.

---

