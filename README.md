# 🛫 Airline Ticket Price Analysis  

## 🔹 Project Overview  
### 🛫 Problem Statement  
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
- How do ticket prices vary with booking time?  
- How do travel dates impact ticket prices?  
- Which routes have the highest/lowest fares?  
- What are the pricing differences across cabin classes and airlines?  
- How do flight stops, duration, and competition affect ticket prices?  
- Do holiday and non-holiday travel trends affect pricing?  

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
  - Converted price values into a consistent format (e.g., ₹29,384 → 29384.18).  
  - Cleaned dates and converted them to datetime format.  
  - Added a derived column "**Days Until Travel**" for deeper insights.  
  - Converted flight durations into total minutes for analysis.  
- **Final cleaned dataset:**  
  - 📌 **3,892 rows and 13 columns**, ensuring accurate analysis.  

## 🔹 Exploratory Data Analysis (EDA)  
### 📊 Key Observations from Visualizations  

**1️⃣ General Price Distribution**  
- Most ticket prices are **₹10,000 - ₹20,000**, but some exceed **₹100,000** (premium/last-minute bookings).  
- The **average price** is **₹30,434**, but the **median price** is **₹19,105** (high-priced outliers affect the average).  

**2️⃣ Outliers in Ticket Prices**  
- **180 high outliers (₹100,000+)** exist due to premium classes & last-minute bookings.  

**3️⃣ Impact of Booking Time**  
- **Last-minute bookings** have the highest average price (**₹39,073**).  
- **Advance bookings** are the cheapest (**₹24,831 on average**).  

**4️⃣ Travel Date Impact**  
- **Weekday flights** are the most expensive (**₹31,091**).  
- **Weekend flights** are cheaper (**₹30,575**).  
- **Holiday travel** is slightly cheaper (**₹29,580**).  

**5️⃣ Airline Comparison**  
- **Etihad Airways** has the highest average ticket price (**₹239,491**).  
- **IndiGo & Akasa Air** are the cheapest (~₹8,400).  

**6️⃣ Route-Based Price Variation**  
- **Costliest Route:** **Bangalore → Kolkata (₹26,808)**  
- **Cheapest Route:** **Delhi → Mumbai (₹11,443)**  

**7️⃣ Cabin Class Price Comparison**  
- **First Class:** ₹231,294 (most expensive)  
- **Business Class:** ₹49,612  
- **Economy Class:** ₹8,745 (cheapest)  

**8️⃣ Effect of Flight Stops**  
- **Direct flights** are the cheapest (**₹18,659**).  
- **1-stop flights** are the most expensive (**₹39,690**).  

**9️⃣ Duration vs. Price**  
- **Longer flights** generally have **higher prices**.  
- **1-stop flights** show bigger price variations.  

**🔟 Last-Minute Bookings Across Routes**  
- **Most expensive last-minute routes:**  
  - **Bangalore → Kolkata (₹42,954)**  
  - **Kolkata → Guwahati (₹40,287)**  
- **Advance bookings offer the biggest savings.**  

## 🔹 Key Insights  

### 📌 For Travelers:  
✔ **Book Early** → Advanced bookings save money.  
✔ **Choose Direct Flights** → They are cheaper and time-efficient.  
✔ **Compare Airlines** → Budget airlines offer lower prices.  

### 📌 For Airlines:  
✔ **Early Booking Discounts** → Encourage advanced ticket sales.  
✔ **Dynamic Pricing** → Adjust fares for high-demand routes.  
✔ **Promote Direct Flights** → As a cost-effective option.  

## 🔹 Recommendations  
Airline ticket prices are influenced by multiple factors, including booking time, travel duration, route, stops, and cabin class.  
### **Best ways to save money:**  
✅ **Book early**  
✅ **Choose direct flights**  
✅ **Opt for Economy class**  
✅ **Avoid last-minute bookings**  

### **Best times to travel:**  
✅ **Holidays and weekends** are slightly cheaper than weekdays.  
✅ Airlines should **optimize pricing models** to balance customer satisfaction and revenue management.  

## 🔹 Conclusion  
### 📌 Key Takeaways:  
- **Prices vary widely**, but early bookings are always cheaper.  
- **Weekday flights & 1-stop flights** are costlier.  
- **Bangalore → Kolkata** is the most expensive route.  
- **Economy** is the cheapest option, while **First Class** is the most expensive.  
- **Last-minute bookings remain the costliest across all routes.**  

By using these insights, **travelers can save money, and airlines can optimize pricing for better revenue.**  
