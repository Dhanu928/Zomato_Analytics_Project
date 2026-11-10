# Zomato Restaurant Data Analytics | End-to-End Business Intelligence Project

## Project Overview

This project focuses on performing end-to-end data analysis on a Zomato restaurant dataset containing **9,551 restaurant records**. The objective is to explore restaurant distribution, customer ratings, cuisine preferences, pricing patterns, and geographical trends to identify meaningful business insights.

The project uses **MySQL, Advanced Excel, Power BI, and Tableau** to transform raw restaurant data into meaningful insights and interactive visualizations.

Through data cleaning, SQL queries, exploratory data analysis, KPI calculations, and dashboard development, this project demonstrates how data analytics can support business decision-making in the food and restaurant industry.

## Business Objectives

The primary objectives of this project are:

- Analyze the geographical distribution of restaurants across different countries and cities.
- Identify the most popular cuisines and restaurant categories.
- Evaluate customer ratings and voting patterns.
- Analyze average cost for two people across different locations.
- Identify the cities with the highest restaurant concentration.
- Understand restaurant availability of online delivery and table booking services.
- Examine restaurant pricing patterns and customer preferences.
- Develop interactive dashboards to communicate business performance and insights.

## Tools & Technologies Used

| Tool | Purpose |
|---|---|
| MySQL | Data extraction, querying, transformation and analysis |
| Advanced Excel | Data cleaning, validation, exploratory analysis and calculations |
| Power BI | Interactive dashboards, KPI analysis and visualization |
| Tableau | Data visualization and interactive business dashboards |

## Dataset Information

- **Dataset:** Zomato Restaurant Dataset
- **Total Records:** 9,551 restaurant records
- **Data Type:** Structured restaurant and business information

### Key Dataset Attributes

The dataset includes information such as:

- Restaurant ID
- Restaurant Name
- Country Code
- City
- Address
- Locality
- Cuisines
- Average Cost for Two
- Currency
- Has Table Booking
- Has Online Delivery
- Price Range
- Aggregate Rating
- Rating Color
- Rating Text
- Votes
- Restaurant Location (Latitude and Longitude)

## Project Workflow

The project follows an end-to-end data analytics workflow:

1. Data Collection – Obtained the Zomato restaurant dataset.
2. Data Understanding – Examined the dataset structure, columns, data types and records.
3. Data Cleaning – Identified and handled missing values, duplicate records, inconsistent entries and data quality issues.
4. Data Processing – Prepared and transformed data for analysis.
5. SQL Analysis – Used MySQL to perform data extraction, filtering, aggregation and business analysis.
6. Exploratory Data Analysis – Investigated restaurant distribution, ratings, pricing and cuisine trends.
7. KPI Development – Analyzed key business performance indicators.
8. Dashboard Development – Created interactive dashboards using Power BI and Tableau.
9. Business Insights – Interpreted analytical results to identify business trends and opportunities.

## Data Cleaning & Preparation

Data preparation was an important part of the project to improve data quality and ensure accurate analysis.

The following activities were performed:

- Inspected the dataset for missing and null values.
- Identified duplicate restaurant records.
- Checked data types and corrected inconsistencies.
- Reviewed geographical information, including city and country details.
- Standardized relevant categorical values.
- Examined restaurant ratings and pricing information.
- Prepared the dataset for SQL analysis and dashboard development.

**Objective:** To ensure data consistency, accuracy and reliability before performing business analysis.

## SQL Analysis Using MySQL

MySQL was used to query the restaurant dataset and extract business insights.

The analysis focused on restaurant counts, geographical distribution, cuisine popularity, customer ratings, pricing and service availability.

### Key SQL Analysis Areas

1. Total number of restaurants.
2. Country-wise restaurant distribution.
3. City-wise restaurant distribution.
4. Top 10 cities with the highest number of restaurants.
5. Most popular cuisines.
6. Restaurant ratings and rating categories.
7. Average cost for two across different locations.
8. Restaurants offering online delivery.
9. Restaurants offering table booking.
10. Restaurant distribution by price range.

### Sample SQL Queries

**1. Total Number of Restaurants**

```sql
SELECT COUNT(*) AS Total_Restaurants
FROM zomato;
```

**2. Country-wise Restaurant Distribution**

```sql
SELECT
    CountryCode,
    COUNT(*) AS Total_Restaurants
FROM zomato
GROUP BY CountryCode
ORDER BY Total_Restaurants DESC;
```

**3. Top 10 Cities by Restaurant Count**

```sql
SELECT
    City,
    COUNT(*) AS Restaurant_Count
FROM zomato
GROUP BY City
ORDER BY Restaurant_Count DESC
LIMIT 10;
```

**4. Top 10 Cuisines**

```sql
SELECT
    Cuisines,
    COUNT(*) AS Restaurant_Count
FROM zomato
GROUP BY Cuisines
ORDER BY Restaurant_Count DESC
LIMIT 10;
```

**5. Average Cost for Two by City**

```sql
SELECT
    City,
    ROUND(AVG(Average_Cost_for_two), 2)
        AS Average_Cost
FROM zomato
GROUP BY City
ORDER BY Average_Cost DESC;
```

**6. Restaurant Rating Distribution**

```sql
SELECT
    Rating_Text,
    COUNT(*) AS Restaurant_Count
FROM zomato
GROUP BY Rating_Text
ORDER BY Restaurant_Count DESC;
```

**7. Restaurants Offering Online Delivery**

```sql
SELECT
    Has_Online_delivery,
    COUNT(*) AS Restaurant_Count
FROM zomato
GROUP BY Has_Online_delivery;
```

## Key Performance Indicators (KPIs)

The following analytical metrics were considered to understand restaurant industry performance:

| KPI | Business Purpose |
|---|---|
| Total Restaurants | Measures the number of restaurants in the dataset |
| Average Restaurant Rating | Evaluates overall customer rating levels |
| Total Votes | Measures customer engagement |
| Average Cost for Two | Understands restaurant pricing patterns |
| Restaurant Count by City | Identifies geographical concentration |
| Restaurant Count by Cuisine | Identifies cuisine distribution |
| Online Delivery Availability | Evaluates delivery service availability |
| Table Booking Availability | Evaluates reservation service availability |
| Price Range Distribution | Understands restaurant pricing categories |

## Power BI Dashboard

Developed interactive Power BI dashboards to present restaurant analytics through meaningful visualizations and KPIs.

### Dashboard Analysis

- Overall restaurant distribution.
- Country-wise and city-wise restaurant analysis.
- Top 10 cities by restaurant count.
- Top 10 cuisine analysis.
- Restaurant rating distribution.
- Average cost for two analysis.
- Online delivery and table booking availability.
- Restaurant price range distribution.

**Dashboard Preview:**

Add your actual Power BI dashboard screenshots here.

`![Power BI Dashboard](images/powerbi-dashboard.png)`

## Tableau Dashboard

Created Tableau visualizations to explore restaurant performance and geographical trends through interactive charts and analytical views.

### Key Visualizations

- Restaurant distribution by country and city.
- Top-performing cities based on restaurant count.
- Cuisine popularity analysis.
- Restaurant ratings and customer engagement.
- Average cost comparison.
- Restaurant service availability.
- Geographical restaurant distribution.

**Dashboard Preview:**

Add your actual Tableau dashboard screenshots here.

`![Tableau Dashboard](images/tableau-dashboard.png)`

## Business Insights & Observations

The analysis was designed to identify the following business patterns:

1. **Geographical Distribution:** Identifying cities and countries with higher restaurant concentrations helps understand market presence and expansion opportunities.

2. **Cuisine Preferences:** Analyzing cuisine distribution helps identify popular food categories and potential opportunities for restaurant businesses.

3. **Customer Ratings:** Examining restaurant ratings and votes helps understand customer satisfaction and engagement patterns.

4. **Pricing Analysis:** Comparing average costs across locations provides insights into restaurant pricing strategies and market positioning.

5. **Service Availability:** Analyzing online delivery and table booking availability helps understand restaurant service adoption.

6. **Market Opportunities:** Combining geographical, pricing and customer-rating information can help identify potential areas for business growth.

## Challenges & Learnings

During the project, the following technical and analytical areas were addressed:

- Handling missing and inconsistent data.
- Working with geographical and categorical information.
- Managing data types during data import.
- Writing SQL queries for business-oriented analysis.
- Combining multiple analytical approaches.
- Selecting appropriate KPIs for dashboard development.
- Transforming raw data into meaningful visualizations.
- Presenting analytical findings in a business-friendly format.

### Key Learnings

- Improved practical knowledge of MySQL and SQL querying.
- Gained experience in data cleaning and exploratory data analysis.
- Strengthened understanding of business KPIs and analytical methods.
- Developed skills in Power BI and Tableau dashboard creation.
- Improved ability to interpret data and communicate business insights.

## Project Repository Structure

Suggested repository organization:

```text
Zomato-Restaurant-Data-Analytics/
│
├── Dataset/
│   └── zomato.csv
│
├── SQL/
│   └── zomato_analysis.sql
│
├── Excel/
│   └── zomato_analysis.xlsx
│
├── PowerBI/
│   └── zomato_dashboard.pbix
│
├── Tableau/
│   └── zomato_dashboard.twbx
│
├── Images/
│   ├── powerbi-dashboard.png
│   └── tableau-dashboard.png
│
└── README.md
```

*Note: The structure above is a suggested organization. Include only files that are actually available in your repository.*

## Project Outcomes

This project demonstrates the application of data analytics tools to a real-world restaurant dataset.

Key outcomes include:

- Analyzed 9,551 restaurant records.
- Explored restaurant distribution across geographical locations.
- Examined cuisine preferences, customer ratings and pricing patterns.
- Performed data cleaning and SQL-based business analysis.
- Developed interactive dashboards using Power BI and Tableau.
- Identified business trends and potential opportunities through data-driven analysis.

## Skills Demonstrated

- SQL & MySQL
- Advanced Microsoft Excel
- Data Cleaning & Data Transformation
- Exploratory Data Analysis (EDA)
- Business Intelligence
- KPI Development
- Data Visualization
- Power BI
- Tableau
- Business Insights & Reporting
- Analytical Thinking
- Data-Driven Decision Making

## Conclusion

The Zomato Restaurant Data Analytics project demonstrates an end-to-end approach to solving business problems using data analytics.

By combining MySQL, Advanced Excel, Power BI and Tableau, the project transforms raw restaurant data into structured information, meaningful business insights and interactive dashboards.

The analysis provides a better understanding of restaurant distribution, cuisine trends, customer ratings, pricing patterns and service availability, demonstrating how data-driven insights can support strategic business decisions.

---

**Project Category:** Data Analytics | Business Analytics | Business Intelligence

**Tools:** MySQL | Advanced Excel | Power BI | Tableau

**Dataset Size:** 9,551 Restaurant Records

**Author:** Dhanunjaya
