# OLA-Data-Analyst-Project-Power-BI-And-SQL

# 🚖 OLA Data Analyst Project — Power BI & SQL

Welcome to the **Ola Data Analyst Project**, a complete end-to-end data analytics solution combining **SQL** and **Power BI**.  
This project analyzes ride-booking data to uncover insights into **ride volumes, customer behavior, cancellations, vehicle types, and revenues.**

![Project Demo](Ola%20DA%20Project%20DEMO.gif)

---

🎯 Project Objectives

- 📊 Track ride volumes and booking statuses over time
- 🚗 Analyze vehicle type performance
- 🧾 Understand payment method preferences
- ❌ Investigate ride cancellation reasons
- 🌟 Explore customer and driver ratings
- 💰 Identify top customers by booking value

---

🛠️ Tools Used

- **SQL** — For querying, aggregating, and creating reusable views
- **Power BI** — For dynamic dashboards and visualizations
- **Excel/CSV** — For preprocessing and data cleaning

---

 📂 Project Components

| 📁 File | 📄 Description |
|---------|----------------|
| `Bookings.csv` | Raw dataset containing ride booking records |
| `Ola DA Project SQL.sql` | SQL script to create views and extract insights |
| `Ola DA Project.pbix` | Power BI dashboard file |
| `Ola DA Project DEMO.gif` | Animated demo of the dashboard |

---

 🧩 SQL Analysis

✅ Key Queries & Views**

- Retrieve Successful Bookings
- Find Average Ride Distance by Vehicle Type
- Count Customer and Driver Cancellations
- Top 5 Customers by Rides
- UPI Payments
- Revenue from Successful Rides
- Incomplete Rides with Reasons

✅ Example: Get Total Revenue from Successful Rides
```sql
CREATE VIEW total_successful_booking_value AS
SELECT SUM(Booking_Value) AS total_revenue
FROM bookings

📈 Power BI Dashboard
The Power BI report includes multiple interactive pages:

✨ Overall
Ride Volume Over Time 📈

Booking Status Breakdown 🟢⚫️🔴

🚗 Vehicle Type
Top 5 Vehicle Types by Ride Distance

💰 Revenue
Revenue by Payment Method

Top Customers by Booking Value

Ride Distance Distribution

❌ Cancellation
Cancellation Reasons by Customer and Driver

🌟 Ratings
Driver Rating Distribution

Customer Rating Distribution

🔍 Key Insights
✅ Ride Volume Trends: Peaks and troughs in demand
✅ Cancellations: 62% rides completed successfully; 18% canceled by drivers
✅ Revenue Distribution: Payment methods and booking values
✅ Vehicle Popularity: Sedans and Autos as top performers
✅ Ratings: Customer and driver satisfaction metrics

🚀 How to Run This Project
1️⃣ SQL

Import Bookings.csv into MySQL Workbench

Run Ola DA Project SQL.sql to create all views

2️⃣ Power BI

Open Ola DA Project.pbix in Power BI Desktop

Refresh the data connections if needed

Explore dashboards interactively


WHERE Booking_Status = 'Success';

