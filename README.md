# 🌍 Travel & Tourism Analytics Dashboard

An interactive **Travel & Tourism Analytics Dashboard** developed using **Microsoft Power BI and DAX** to analyze bookings, customers, destinations, transportation, trip costs, ratings, and cancellations.

## 📊 Project Overview

This project converts travel booking data into an interactive dashboard that helps identify important travel and customer trends.

The dashboard provides a clear view of:

- Booking performance
- Customer and traveller trends
- Popular destination countries and cities
- Transportation preferences
- Trip costs
- Customer ratings
- Booking and cancellation status
- Travel trends over time

## 🛠️ Tools & Technologies

- **Power BI**
- **DAX (Data Analysis Expressions)**
- **Power Query**
- **CSV Dataset**

## 📌 Key KPIs

- Total Bookings
- Total Customers
- Total Travellers
- Total Trip Cost
- Average Trip Cost
- Cancellation Rate
- Average Customer Rating

## 📈 Dashboard Features

### 📅 Booking Trend
Analyzes booking activity over time.

### 🌍 Destination Analysis
Identifies the most popular destination countries and cities based on bookings.

### 💰 Trip Cost Analysis
Compares total and average trip costs across destinations.

### 🚗 Transportation Analysis
Analyzes bookings and customer ratings by transportation type.

### ⭐ Customer Rating Analysis
Tracks average customer ratings and compares ratings across travel categories.

### 📋 Booking & Cancellation Analysis
Shows booking status and cancellation patterns.

### 🗺️ Destination Map
Provides a geographical view of travel destinations.

### 🎛️ Interactive Filters
The dashboard includes interactive slicers for:

- Booking Date
- Destination Country
- Destination City
- Transportation Type
- Booking Status
- Gender
- Meal Plan
- Cancellation Status

## 🧮 DAX Measures

Some of the key DAX measures used in the dashboard:

```DAX
Total Bookings =
COUNT('Travel And Tourism'[Booking_ID])

Total Customers =
DISTINCTCOUNT('Travel And Tourism'[Customer_ID])

Total Travellers =
SUM('Travel And Tourism'[Number_of_Travellers])

Total Trip Cost =
SUM('Travel And Tourism'[Total_Trip_Cost])

Average Trip Cost =
AVERAGE('Travel And Tourism'[Total_Trip_Cost])

Average Customer Rating =
AVERAGE('Travel And Tourism'[Customer_Rating])

Cancelled Bookings =
CALCULATE(
    [Total Bookings],
    'Travel And Tourism'[Cancellation_Status] = "Cancelled"
)

Cancellation Rate =
DIVIDE(
    [Cancelled Bookings],
    [Total Bookings],
    0
)
```

## 📂 Project Files

```text
Travel-Tourism-PowerBI/
│
├── travel and tourism.pbix
├── Travel And Tourism(1).csv
└── README.md
```

## 🚀 How to Use

1. Download or clone this repository.
2. Open `travel and tourism.pbix` in **Power BI Desktop**.
3. If required, reconnect the report to `Travel And Tourism(1).csv`.
4. Refresh the data.
5. Use the interactive slicers and visuals to explore the dashboard.

## 💡 Business Questions Answered

This dashboard helps answer questions such as:

- Which destinations have the highest number of bookings?
- Which cities are most popular?
- What is the total trip cost?
- What is the cancellation rate?
- Which transportation type has the highest average rating?
- How do bookings change over time?
- Which destinations contribute the most to trip cost?
- How do booking patterns vary across customers?

## 👩‍💻 Author

**Medisetti Navya Sri**

**Data Analytics Trainee | Power BI | DAX | SQL | Python**

---

⭐ **If you find this project useful, consider giving the repository a star!**
