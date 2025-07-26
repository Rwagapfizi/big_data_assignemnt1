# Uber Fares Dataset Analysis - Introduction to Big Data assignment (INSY 8413)

#### By Rwagapfizi Igor, 27329, Group E

---

This assignment project explores and analyzes a real-world Uber ride dataset using Python for data cleaning and Power BI for visualization. The aim is to uncover patterns in fare amounts, ride timing, passenger count, and geographic trends to inform strategic business decisions.

## Table of Contents

1. [Introduction](#introduction)
2. [Methodology](#methodology)
3. [Analysis](#analysis)
4. [Results](#results)
5. [Conclusion](#conclusion)
6. [Recommendations](#recommendations)

---

## Introduction

This assignment project analyzes the Uber Fares Dataset to uncover insights into fare patterns, ride durations, and operational metrics. The goal is to develop an interactive Power BI dashboard and present findings through a structured analytical report.
Objectives:

- Perform Exploratory Data Analysis (EDA) to understand dataset structure and quality.
- Conduct feature engineering to extract meaningful insights.
- Build an interactive Power BI dashboard with key visualizations.
- Generate a comprehensive report summarizing findings and recommendations.

---

## Methodology

### Data Collection

The dataset was sourced from a publicly available Uber dataset and includes:

- Fare amount
- Pickup datetime
- Pickup & Dropoff coordinates
- Passenger count

### Data Cleaning & Preprocessing (Python)

- Handled missing/null values in fare, location, and datetime fields.
- Extracted time-based features:
  - `hour`, `day`, `day_name`, `month`, `year`
- Categorized fares into bins (e.g., \$0–10, \$10–20).
- Created a binary flag for **peak hour rides** (`is_peak`).
- Removed extreme outliers (e.g., distances > 100 km or fares > \$100).

### Tools Used

- Python (Pandas, NumPy, Jupyter Notebooks)
- Power BI for dashboard creation and interactive visualization

---

## Analysis

### 1. Fare Distribution

- Most fares fall between **\$5 and \$25**.
- A column chart displays frequency of fares across binned ranges.

### 2. Time-Based Ride Patterns

- **Evening hours (5 PM–8 PM)** show highest ride demand.
- Weekends yield **higher average fares** than weekdays.
- Peak hours = higher volume and slightly increased fare values.

### 3. Geographic Trends

- Ride pickups are **heavily concentrated in urban/downtown areas**.
- Suburban-to-city rides are common during rush hours.

### 4. Ride Distance Analysis

- Most rides are under **5 km**.
- Distance correlates strongly with fare (as expected).
- Due to missing dropoff time, we used distance instead of actual trip duration.

---

## Results

- **Time of Day** impacts both ride frequency and fare amount.
- **Weekends and Peak Hours** drive higher prices and volumes.
- Rides are **geographically clustered** in key city centers.
- **Short-distance trips** are dominant, with occasional long-range travel.
- **Fare amount** increases predictably with distance, not passenger count.

---

## Conclusion

The analysis successfully uncovered insights into Uber rider behavior and operational hotspots:

- Time and location are strong predictors of fare levels.
- Evening and weekend patterns indicate leisure and commuter ride behavior.
- Urban centers serve as key nodes for pickup activity.

Power BI enabled intuitive dashboard creation to support these findings with visuals and interactivity.

---

## Recommendations:

- **Optimize Surge Pricing** during peak and weekend hours to maximize revenue.
- **Deploy more drivers** in urban hotspots between **5 PM – 8 PM**.
- **Encourage off-peak rides** with targeted promotions or discounts.
- **Capture Dropoff Times** for future inclusion of accurate trip durations.
- **Expand Service Coverage** in underrepresented areas with demand potential.

---

## File Structure

- **assignment.ipynb** # *Jupyter notebook for cleaning and enhancing dataset, and visualize data*
- **Rwagapfizi_Igor_27329.pbix** # *Power BI Dashboard File*
- **Rwagapfizi_Igor_Big_Data_Project_Report.pdf** # *Project Documentation that contains screenshots of data visuals*
- **uber.csv** # *Raw uncleaned dataset from Kaggle*
- **uber_cleaned.csv** # *Dataset cleaned from missing and duplicate values*
- **uber_enhanced.csv** # *Final dataset enhanced with analytical features*

---

## Author

**Rwagapfizi Igor, 27329**  
Adventist University of Central Africa – Introduction to Big Data Assignment Project (July 2025)

