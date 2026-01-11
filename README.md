
# Crime Data Analysis

## 📌 Project Overview

This project explores the `crimes.csv` dataset to analyze crime patterns based on **time**, **location**, and **victim age groups**.
Using Python and pandas, we answer specific analytical questions and support the findings with visualizations.

---

## 📂 Dataset

* **File name:** `crimes.csv`
* **Description:**
  The dataset contains recorded crime incidents with information such as:

  * Time of occurrence
  * Area/location
  * Victim age
  * Other crime-related attributes

---

## 🎯 Objectives

The notebook answers the following questions:

1. **Peak Crime Hour**

   * Identify the hour of the day (0–23) with the highest frequency of crimes.

2. **Peak Night Crime Location**

   * Determine which area has the highest number of crimes committed at night
     (between **10:00 PM and 3:59 AM**).

3. **Victim Age Group Analysis**

   * Calculate the number of crimes committed against victims in the following age groups:

     * `0–17`
     * `18–25`
     * `26–34`
     * `35–44`
     * `45–54`
     * `55–64`
     * `65+`

---

## 🛠️ Tools & Libraries Used

* **Python**
* **pandas** – data cleaning and analysis
* **matplotlib** – data visualization

---

## 📊 Methodology

### 1️. Data Exploration & Cleaning

* Checked data types and missing values
* Verified that victim ages are valid (no negative values)
* Extracted crime hours from time data

### 2️. Time-Based Analysis

* Converted crime time into hourly format
* Counted crime frequency per hour
* Filtered night crimes using specific hour ranges

### 3️. Age Group Categorization

* Used predefined age bins
* Applied `pd.cut()` to classify victim ages
* Counted crimes per age group

### 4️. Visualization

* Created bar charts to visually represent:

  * Night crime frequency by area
  * Crime distribution across victim age groups

---

## 📈 Key Outputs

* **`peak_crime_hour`** → Integer representing the busiest crime hour
* **`peak_night_crime_location`** → String representing the area with most night crimes
* **`victim_ages`** → pandas Series showing crime counts per age group

Each result is computed programmatically and supported by plots.

---

## 🧠 Key Insights

* Crime frequency varies significantly by hour, with identifiable peak periods at 12pm (highest peak) and 1 am.
* Night crimes are concentrated in specific areas specially the central area..
* Most crimes involve victims in adult age ranges, while minors and elderly victims represent smaller proportions.

---
