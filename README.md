# Why 28% of Swiggy Orders Are Delivered Late: A Data Case Study

---

## 1. Project Overview

Late deliveries are one of the most critical operational challenges in food delivery platforms. They directly impact customer satisfaction, refunds, retention, and brand trust.

This project analyzes Swiggy delivery data to understand why orders are delivered late, what operational factors drive delays, and how businesses can reduce SLA breaches using data‑driven strategies.

---

## 2. Problem Statement

Approximately 28% of orders are delivered beyond the promised SLA time.

The objective of this project is to:

1. Measure the scale of late deliveries
2. Identify root causes behind delays
3. Detect high‑risk orders
4. Explore operational strategies to reduce late deliveries

---

## 3. Dataset Description

The dataset contains 45K+ delivery records with operational, geographical, and time‑based attributes.

### Key Columns:

1. Delivery Partner Details
2. Restaurant & Delivery Location Coordinates
3. Order & Pickup Time
4. Weather Conditions
5. Traffic Density
6. Vehicle Type & Condition
7. Multiple Deliveries
8. City
9. Time Taken (Delivery Duration)

---

## 4. Data Cleaning & Preprocessing

Data preparation steps included:

1. Handling NaN and inconsistent values
2. Cleaning categorical text fields
3. Converting time columns to datetime format
4. Extracting order hour & minute features
5. Removing invalid latitude & longitude entries
6. Formatting delivery duration column

Clean data ensured accurate delay and SLA analysis.

---

## 5. SLA Definition

A delivery is considered **Late** if:

Time Taken > 30 minutes

This threshold was used to create a Late Delivery flag for analysis.

---

## 6. Key Analysis Areas

### 6.1 Late Delivery Measurement

1. Percentage of late deliveries
2. Average delay duration

### 6.2 Distance Impact

1. Delivery distance calculation using geo‑coordinates
2. Delay probability across distance ranges

### 6.3 Time‑Based Analysis

1. Hourly delay distribution
2. Peak vs non‑peak comparison
3. Weekend vs weekday performance

### 6.4 City‑Wise Analysis

1. Late delivery rates by city
2. Operational load comparison

### 6.5 Order Risk Characteristics

1. Distance
2. Traffic conditions
3. Weather
4. Multiple deliveries
5. Rider ratings

---

## 7. High‑Risk Order Identification

A rule‑based framework was built to tag orders likely to be delivered late using:

1. Long delivery distance
2. Peak hours
3. Heavy traffic
4. Adverse weather
5. Multiple active deliveries
6. Low rider ratings

This helps enable proactive operational intervention.

---

## 8. Distance Cap Simulation

A delivery radius simulation was conducted to evaluate delay reduction.

Steps:

1. Apply distance caps (2 km, 5 km, 8 km, etc.)
2. Recalculate late delivery %
3. Compare against current performance

This demonstrated how limiting long‑distance orders can reduce SLA breaches.

---

## 9. Project Architecture Diagram

The project follows a structured analytics pipeline from raw data to business insights.

```
            Raw Swiggy Delivery Data
                       │
                       ▼
            Data Cleaning & Preprocessing
                       │
                       ▼
        Feature Engineering (Time & Distance)
                       │
                       ▼
         Exploratory Data Analysis (EDA)
                       │
                       ▼
        Delay Measurement & SLA Analysis
                       │
                       ▼
        Risk Segmentation & Pattern Mining
                       │
                       ▼
        Distance Cap Simulation Modeling
                       │
                       ▼
              Business Insights
                       │
                       ▼
            Operational Recommendations
```

---

## 10. Dashboard & Visualization Sections

The following visual dashboards were created to support the analysis:

### 10.1 Late Delivery KPI Dashboard

1. Overall Late Delivery %
2. Average Delay Time
3. SLA Breach Count

### 10.2 Distance vs Delay Analysis

1. Delay probability by distance range
2. Distance distribution of late orders

### 10.3 Time‑Based Performance Dashboard

1. Hourly late delivery frequency
2. Peak vs non‑peak comparison
3. Weekend vs weekday delays

### 10.4 City‑Wise Operations Dashboard

1. Late delivery % by city
2. Order volume vs delay correlation

### 10.5 High‑Risk Order Dashboard

1. Risk category segmentation
2. Late probability by risk level

### 10.6 Distance Cap Simulation Dashboard

1. Late % under distance caps
2. Reduction comparison vs current SLA performance

---

## 11. Tools & Technologies Used

1. Python
2. Pandas
3. NumPy
4. GeoPy
5. Matplotlib
6. Data Cleaning & Feature Engineering
7. Exploratory Data Analysis (EDA)

---

## 10. Business Impact

This analysis helps:

1. Identify operational bottlenecks
2. Improve last‑mile logistics planning
3. Optimize delivery radius
4. Prioritize high‑risk orders
5. Reduce SLA breaches
6. Enhance customer satisfaction

---

## 11. Project Outcome

The project delivers a structured understanding of late delivery drivers and proposes data‑backed strategies to improve delivery efficiency.

---

## 12. Future Improvements

1. Cost impact analysis (refunds, compensation)
2. Rider allocation optimization
3. Real‑time delay prediction model
4. Demand vs supply balancing

---

## 14. Closing Note

"Data doesn’t just explain delays it helps design faster deliveries."
