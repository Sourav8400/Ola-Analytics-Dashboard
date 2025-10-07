# **Ola Data Analysis Project using Excel, SQL & Power BI**

## Recommended Structure and order

### 1. Project Overview
This project involves comprehensive analysis of Ola ride booking data to extract actionable insights regarding customer behavior, ride patterns, cancellations, and revenue trends. The objective is to perform data cleaning, conduct SQL-based analysis, and build interactive Power BI dashboards to support data-driven decision-making for ride-sharing platforms like Ola.

### 2. Tech Stack
• Power BI: Data visualization and dashboard creation
• MySQL / SQL: Data extraction, transformation, and analytical queries
• MS Excel / CSV: Dataset preparation and management
• Power Query: Data loading and modeling within Power BI

### 3. Data Source
The dataset was synthetically generated using ChatGPT prompts and contains 100,000 booking records for Bengaluru city over one month. Key data fields include:
• Booking details: Date, Time, Booking ID, Status
• Customer & Driver information
• Vehicle types: Auto, Mini, Prime Sedan, Prime SUV, etc.
• Ratings, ride distance, payment methods, and cancellation reasons

### 4. Key Features / Highlights
• Cleaning and modeling of 100,000+ Ola ride records
• SQL queries to analyze ride metrics, cancellations, and performance
• Interactive Power BI dashboards featuring :
    • Ride Volume Over Time
    • Booking Status Breakdown
    • Revenue by Payment Method
    • Top 5 Customers by Total Booking Value
    • Driver & Customer Rating Analysis
    • Cancellation Reasons (Customer vs Driver)
•Insights into ride demand trends, customer satisfaction, and vehicle performance

### 5. Example SQL Queries
```
-- Retrieve all successful bookings
SELECT * FROM bookings WHERE Booking_Status = 'Success';

-- Find the average ride distance for each vehicle type
SELECT Vehicle_Type, AVG(Ride_Distance) AS avg_distance
FROM bookings
GROUP BY Vehicle_Type;

-- Get the total number of rides cancelled by customers
SELECT COUNT(*) 
FROM bookings 
WHERE Booking_Status = 'cancelled by Customer';
```

### 6. Power BI Dashboard Insights
• Ride Volume Over Time: Identify peak hours and weekend trends
• Revenue Analysis: Compare payment methods (UPI, Cash, Card)
• Customer vs Driver Ratings: Understand correlation between service quality and ride experience•
• Top Vehicle Types: Analyze vehicle category performance

### 7. Power BI Dashboard Preview
![Ola Ride Analytics Dashboard](https://github.com/Sourav8400/Ola-Analytics-Dashboard/blob/main/Snapshot%20of%20the%20Dashboard.png)

### Conclusion
This project demonstrates an end-to-end data analytics workflow — from synthetic data generation and SQL-based analysis to Power BI visualization — enabling actionable insights into Ola’s operational performance and customer behavior.
