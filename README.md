🌾 AgroFinance: Agricultural Mandi Price Analysis
📌 Project Overview

AgroFinance is a data analytics project focused on analyzing agricultural mandi prices in India using real-time government data.
The project demonstrates an end-to-end data pipeline — from API data extraction to visualization and SQL database storage.

The goal is to understand price variation across states, districts, markets, and commodities, and to build a reusable analytics workflow for agri-finance insights.

🎯 Objectives

Fetch live mandi price data from data.gov.in API

Clean and preprocess raw market data

Perform exploratory data analysis (EDA)

Visualize price trends and distributions

Store processed data in SQL Server for future querying and dashboards

🧰 Tech Stack

Python

Pandas, NumPy

Requests (API integration)

Matplotlib, Seaborn

SQL Server

SQLAlchemy & PyODBC

📥 Data Source

Government of India – data.gov.in

Resource: Agricultural Produce Market Committee (APMC) mandi prices

Data includes:

State

District

Market

Commodity

Variety & Grade

Arrival Date

Minimum, Maximum & Modal Prices

🔄 Project Workflow
1️⃣ API Data Extraction

Used requests to fetch JSON data from the government API

Converted API response into a Pandas DataFrame

Stored raw data locally as CSV for reproducibility

2️⃣ Data Cleaning & Preprocessing

Removed missing values and duplicates

Standardized column names

Converted price columns to numeric format

Parsed date fields into datetime objects

3️⃣ Exploratory Data Analysis (EDA)

Price comparison across:

States

Districts

Markets

Commodities

Visualizations used:

Bar plots

Line plots

Histograms

Box plots

Violin plots

Cross-tab analysis between commodities and states

4️⃣ Data Visualization

Identified:

Markets with high price volatility

State-wise commodity price differences

Distribution patterns of minimum and maximum prices

5️⃣ SQL Database Integration

Connected to SQL Server using Windows Authentication

Created a structured table for mandi prices

Inserted cleaned DataFrame into SQL database

Enabled further querying and BI tool integration

🗄️ Database Schema (Mandi Prices Table)
Column Name	Description
state	State name
district	District name
market	Market name
commodity	Commodity name
variety	Commodity variety
grade	Quality grade
arrival_date	Date of arrival
min_price	Minimum price
max_price	Maximum price
modal_price	Modal (average) price
📊 Key Insights

Significant price variation exists across markets for the same commodity

Certain states show consistently higher modal prices

Vegetables and spices exhibit higher volatility compared to grains

Market-level analysis is more informative than state-level averages

🚀 Future Enhancements

Add time-series forecasting for price prediction

Integrate Power BI / Tableau dashboards

Automate daily API data ingestion

Add crop-wise and seasonal trend analysis

👤 Author

Mrudul Paku
Aspiring Data Analyst | Python | SQL | Data Visualization
