 
# 🛫 Airline Ticket Price Analysis - Exploratory Data Analysis (EDA)

## 🔹 Project Overview  
### **Problem Statement**  
Airline ticket prices fluctuate based on multiple factors, including:  

- Travel dates  
- Booking time (early vs. last-minute)  
- Flight routes  
- Number of stops  
- Cabin classes (Economy, Business, First)  
- Airline carrier differences  

This analysis aims to understand price variations, correlations, and anomalies to help travelers book at the best time and assist airlines in optimizing pricing strategies.

## 🔹 Objectives  
This project aims to answer:  

1. How do ticket prices vary with booking time?  
2. How do travel dates impact ticket prices?  
3. Which routes have the highest/lowest fares?  
4. What are the pricing differences across cabin classes and airlines?  
5. How do flight stops, duration, and competition affect ticket prices?  
6. Do holiday and non-holiday travel trends affect pricing?  

---

## 🔹 Data Collection  

### 🛠 Tools Used:  
- **NumPy, Pandas** (for data manipulation)  
- **Matplotlib, Seaborn** (for visualization)  
- **BeautifulSoup, Selenium** (for web scraping)  
- **Regex** (for text cleaning)  

### 📊 Data Extraction & Cleaning:  
- Extracted **4,438 rows with 8 columns** using web scraping.  
- Data cleaning steps:  
  - Removed duplicates.  
  - Standardized column names.  
  - Converted price values into a consistent format (e.g., ₹29,384 → `29384.18`).  
  - Cleaned dates and converted them to datetime format.  
  - Added a derived column **"Days Until Travel"** for deeper insights.  
  - Converted flight durations into total minutes for analysis.  
- **Final cleaned dataset**:  
  - **📌 3,892 rows and 13 columns**, ensuring accurate analysis.  

---

## 🔹 Exploratory Data Analysis (EDA)  

### 📊 Key Observations from Visualizations  

### 1️⃣ General Price Distribution  
- Most ticket prices are **₹10,000 - ₹20,000**, but some exceed **₹100,000** (premium/last-minute bookings).  
- The **average price** is ₹30,434, but the **median price** is ₹19,105 (high-priced outliers affect the average).  

### 2️⃣ Outliers in Ticket Prices  
- **180 high outliers (₹100,000+)** exist due to premium classes & last-minute bookings.  

### 3️⃣ Impact of Booking Time  
- **Last-minute bookings** have the highest average price (₹39,073).  
- **Advance bookings** are the cheapes
