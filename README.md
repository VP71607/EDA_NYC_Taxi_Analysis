# 🗽 NYC Yellow Taxi Trip Analysis (2023)

[![Python](https://img.shields.io/badge/python-3.x-blue?style=for-the-badge&logo=python)](https://www.python.org/)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter)](https://jupyter.org/)
[![Platform](https://img.shields.io/badge/Platform-Colab-red?style=for-the-badge&logo=googlecolab)](https://colab.research.google.com/)

---

## 📑 Table of Contents
- [Project Overview](#project-overview)
- [Objectives](#objectives)
- [Dataset Description](#dataset-description)
- [Tools and Libraries](#tools-and-libraries)
- [Analysis Workflow](#analysis-workflow)
- [Key Insights](#key-insights)
- [Future Scope](#future-scope)
- [Author](#author)

---

## 📘 Project Overview
This project performs an **Exploratory Data Analysis (EDA)** on NYC Yellow Taxi Trip data for 2023. The analysis aims to uncover patterns in passenger behavior, fare structures, trip demand, and revenue trends.  

The insights can help optimize taxi operations, improve pricing strategies, and enhance service quality.

---

## 🎯 Objectives
- **Data Refinement:** Clean and preprocess raw trip data.
- **Anomaly Detection:** Handle missing, zero, and negative values.
- **Revenue Analysis:** Deconstruct fare components (fare, tip, surcharge, tolls).
- **Trend Identification:** Explore temporal trends (hourly, daily, monthly patterns).
- **Spatial Analysis:** Investigate geographical patterns using pickup and drop-off zones.
- **Strategic Insights:** Derive actionable findings to improve taxi operations.

---

## 🧩 Dataset Description
- **Source:** NYC Taxi & Limousine Commission (TLC) trip record data.
- **Volume:** ~300,000 rows sampled for analysis.
- **Key Features:**
  - `VendorID`, `passenger_count`, `trip_distance`, `RatecodeID`
  - `PULocationID`, `DOLocationID`, `payment_type`
  - `fare_amount`, `extra`, `mta_tax`, `tip_amount`, `tolls_amount`
  - `improvement_surcharge`, `total_amount`, `congestion_surcharge`, `airport_fee`
  - `pickup_datetime`, `dropoff_datetime`

---

## 🧮 Tools & Libraries
| Category | Libraries/Tools |
| :--- | :--- |
| **Data Manipulation** | `pandas`, `numpy` |
| **Data Cleaning** | `pandas`, `datetime` |
| **Visualization** | `matplotlib`, `seaborn`, `plotly` |
| **Environment** | `Google Colab` / `Jupyter Notebook` |

---

## ⚙️ Analysis Workflow

### 1. Data Overview & Cleaning
Loaded and inspected the dataset for missing values and duplicates. Handled zero/negative fares and converted timestamps into datetime objects.

### 2. Feature Engineering
Created new metrics to enrich the analysis:
* `trip_duration`: Calculated from pickup and drop-off times.
* `pickup_hour` & `weekday`: Extracted for temporal analysis.
* `tip_percentage`: To study tipping behavior.

### 3. Exploratory Analysis
Studied the distribution of passenger counts and trip distances. Analyzed correlations between fare components and external factors like time of day.



---

## 📊 Key Insights
* **Peak Hours:** Trip demand peaks between **3 PM – 7 PM**, with **6 PM** being the busiest hour of the day.
* **Passenger Density:** Most trips involve **1–2 passengers** traveling short distances (**<5 miles**).
* **Revenue Spikes:** Nighttime trips generate higher revenue per mile due to night surcharges and better tipping.
* **Tipping Trends:** Tips are proportionally higher for solo passengers and shorter trip durations.
* **Pricing Dynamics:** Vendor 2 generally exhibits higher charges per mile for short-distance trips.

---

## 📈 Future Scope
- **Interactive Mapping:** Geospatial visualization using `Folium` or `GeoPandas`.
- **Advanced Statistics:** Hypothesis testing on fare and tip variations.
- **Predictive Modeling:** Developing fare estimation and demand forecasting models.
- **Automation:** Automated monthly report generation via Python scripts.

---

## 👤 Author
* **Vijay Patil** 
* **Role:** Devops Engineer | Data Enthusiast and Aspiring Data Analyst
* **Notebook:** EDA_NYC_Taxi_Analysis_Vijay_Patil.ipynb

[![GitHub](https://img.shields.io/badge/GitHub-Profile-181717?style=flat&logo=github)](https://github.com/VijayPatil)
