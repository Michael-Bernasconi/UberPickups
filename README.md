# 🚗 Uber Pickups Data Mining Project: NYC Analysis

This project presents a comprehensive data mining analysis of **Uber pickup data in New York City** between May and September 2014. The goal is to identify spatial patterns, temporal trends, and provide predictive insights to optimize fleet management.

---

## 📌 Project Overview
The study analyzes urban mobility dynamics in one of Uber's most active markets. The main objectives are:
1.  **Spatial Analysis:** Understand demand behavior and identify key pickup hotspots.
2.  **Temporal Trends:** Analyze hourly, daily, and monthly patterns governing pickup flows.
3.  **Predictive Modeling:** Develop a model to estimate hourly demand to support strategic fleet allocation.

---

## 🛠️ Methods and Algorithms
Various data science techniques and Python libraries were utilized:
* **K-Means Clustering:** Used to define **10 distinct spatial zones** (clusters) in NYC based on geographic coordinates.
* **Graph Network Analysis (NetworkX):** Used to model transitions between clusters as a Directed Graph, where edge weights indicate transition frequency.
* **Random Forest Regressor:** Selected for its robustness and ability to handle non-linear data when forecasting hourly demand.
* **Visualization:** **Folium** was used to create interactive maps to highlight areas with high concentrations of events.

---

## 📊 Data Description
The dataset, sourced from Kaggle, contains detailed information about Uber pickups in 2014.
* **Timeframe:** Specifically focuses on May through September 2014.
* **Data Structure:** Includes Timestamps (Date/Time), Latitude, Longitude, and the Operational Base ID.

---

## 📈 Key Findings

### 🕒 Temporal Dynamics
* **Daily Patterns:** Demand peaks between **17:00 and 18:00** (evening commute)[cite: 142]. [cite_start]A secondary peak occurs between 07:00 and 08:00.
* **Weekly Variation:** Activity is consistently high on weekdays, but **Saturday** records the highest volume due to leisure and nightlife.
* **Monthly Trends:** Pickup volume gradually increased throughout the period, with August and September showing the highest volumes.

### 🤖 Model Performance
The Random Forest model demonstrated exceptional effectiveness in predicting demand:
* **Coefficient of Determination ($R^2$):** **0.854** (explaining 85.4% of the variability in hourly pickups).
* **Mean Squared Error (MSE):** 60,202.36 (consistent with the large scale of the target variable).
* The tight alignment of points along the diagonal in the prediction plots confirms high accuracy.

---

## 🚀 Conclusion & Future Work
The project proves that urban transport demand is highly predictable based on temporal features.
* **Practical Implications:** Transport companies can use these predictions to optimize vehicle allocation and minimize waiting times.
* **Future Work:** Accuracy could be improved by integrating external variables like weather, holidays, or major city events.

---
**Author:** Michael Bernasconi
