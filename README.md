# 🧹 Data Cleaning Challenge – NYC Airbnb Dataset

## 📌 Overview
This project focuses on cleaning a real-world, messy dataset using Python.  
The objective is to handle missing values, correct data types, and detect & treat outliers while documenting each step clearly.

This project was completed as **Task 8** of a **Data Science Internship**.

---

## 📊 Dataset Information
- **Dataset Name:** NYC Airbnb Open Data (2019)
- **Source:** Kaggle
- **Records:** 48,000+
- **Common Issues Identified:**
  - Missing values
  - Incorrect data types
  - Extreme outliers

---

## 🛠️ Tools & Libraries Used
- Python
- Pandas
- NumPy
- Matplotlib

---

## 🔍 Data Cleaning Steps

### 1️⃣ Missing Value Handling
- **Text Columns (`name`, `host_name`)**
  - Filled missing values with `"Unknown"`
- **Numeric Column (`reviews_per_month`)**
  - Filled missing values using median
- **Date Column (`last_review`)**
  - Converted to datetime format

📌 *Median was used as it is robust to outliers.*

---

### 2️⃣ Data Type Conversion
Converted the following columns to numeric format:
- `price`
- `minimum_nights`
- `availability_365`

Invalid values were coerced into `NaN`.

---

### 3️⃣ Outlier Detection
- Used **Interquartile Range (IQR)** method
- Visualized outliers using boxplots
- Focused on:
  - `price`
  - `minimum_nights`

📌 *Null values were temporarily removed during visualization to avoid empty plots.*

---

### 4️⃣ Outlier Treatment
- Applied **capping technique**
- Values outside IQR limits were capped to upper/lower bounds

📌 *This avoids data loss while reducing the impact of extreme values.*

---

### 5️⃣ Final Validation
After cleaning:
- No unnecessary missing values
- Correct data types
- Outliers controlled

The dataset is now ready for analysis or machine learning.

---


---

## ✅ Conclusion
This project demonstrates real-world data cleaning skills, including problem identification, solution implementation, and clear documentation — essential for any data science role.

---


