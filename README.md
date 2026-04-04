# AgroFinance: Agricultural Mandi Price Analysis

## Overview  
AgroFinance is a data analytics project focused on analyzing agricultural mandi prices in India using real-time government data.  

The project demonstrates an end-to-end data pipeline, from API-based data extraction to data cleaning, analysis, visualization, and storage in a SQL database. It aims to uncover price variations across states, districts, markets, and commodities while building a reusable analytics workflow for agri-finance insights.

---

## Objectives  
- Fetch live mandi price data from the data.gov.in API  
- Clean and preprocess raw market data  
- Perform exploratory data analysis (EDA)  
- Visualize price trends and distributions  
- Store processed data in SQL Server for querying and dashboard integration  

---

## Tools and Technologies  
- **Python**  
- **Pandas**, **NumPy**  
- **Requests** for API integration  
- **Matplotlib**, **Seaborn** for visualization  
- **SQL Server**  
- **SQLAlchemy**, **PyODBC** for database connectivity  

---

## Data Source  
- Government of India – data.gov.in  
- Dataset: Agricultural Produce Market Committee (APMC) mandi prices  

### Data Fields  
- State  
- District  
- Market  
- Commodity  
- Variety and Grade  
- Arrival Date  
- Minimum, Maximum, and Modal Prices  

---

## Project Workflow  

### Data Extraction  
- Retrieved real-time data using API requests  
- Converted JSON responses into structured DataFrames  
- Stored raw data as CSV for reproducibility  

### Data Cleaning and Preprocessing  
- Removed missing values and duplicates  
- Standardized column names  
- Converted price fields to numeric format  
- Parsed date fields into datetime format  

### Exploratory Data Analysis  
- Compared prices across states, districts, markets, and commodities  
- Performed distribution and trend analysis  
- Conducted cross-tab analysis between commodities and regions  

### Data Visualization  
- Used bar plots, line plots, histograms, box plots, and violin plots  
- Identified price distributions and volatility patterns  
- Highlighted regional and commodity-based differences  

### Database Integration  
- Connected to SQL Server using Windows Authentication  
- Created a structured table for mandi price data  
- Inserted cleaned data into the database  
- Enabled further querying and integration with BI tools  

---

## Database Schema  

| Column Name   | Description            |
|--------------|------------------------|
| state        | State name             |
| district     | District name          |
| market       | Market name            |
| commodity    | Commodity name         |
| variety      | Commodity variety      |
| grade        | Quality grade          |
| arrival_date | Date of arrival        |
| min_price    | Minimum price          |
| max_price    | Maximum price          |
| modal_price  | Modal (average) price  |

---

## Key Insights  
- Significant price variation exists across markets for the same commodity  
- Certain states consistently show higher modal prices  
- Vegetables and spices exhibit higher price volatility compared to grains  
- Market-level analysis provides deeper insights than state-level averages  

---

## Business Value  
- Helps understand agricultural price dynamics across regions  
- Supports farmers, traders, and policymakers in decision-making  
- Enables better price forecasting and market planning  
- Provides a foundation for agri-finance analytics solutions  

---

## Use Case  
This project can be applied in agricultural analytics platforms, supply chain optimization, and financial planning systems to improve price transparency and market efficiency.

---

## Future Enhancements  
- Implement time-series forecasting for price prediction  
- Develop interactive dashboards using Power BI or Tableau  
- Automate daily API data ingestion  
- Add crop-wise and seasonal trend analysis  

---

## Author  
**Mrudul Paku**  
Aspiring Data Analyst | Python | SQL | Data Visualization  
