# Excel
Excel Sales Analysis
## Data Analysis and Report Building Plan

### 1. Data Cleaning and ETL Process:
   a. **Source Data Handling:**
      - Retrieve sales and finance data from data sources.
   b. **Initial Data Inspection:**
      - Open data files in Excel Power Query Editor.
      - Change the first row as headers.
   c. **Data Cleaning:**
      - Check for missing values.
      - Ensure all dimension tables have unique values.
      - Randomly check for errors and spelling mistakes.
   d. **Column Distribution Check:**
      - Navigate to View -> Column Distribution to analyze data distribution.

### 2. Database Setup:
   a. **Star Schema Creation:**
      - Connect tables using primary and foreign keys.
   b. **Date Table:**
      - Create a date table using `Number.From(#date(2018,1,1))..Number.From(#date(2018,12,31))`.
      - Convert calendar year to fiscal year (Sep 1 to Aug End).

### 3. Components for Report Building:
   a. **Database Components:**
      - Netsales
      - Year
      - Division
      - Country
      - Region
   b. **Star Schema Implementation:**
      - Connect dimension tables using primary and foreign keys.

### 4. Customer Performance Report:
   - Include information for 2019, 2020, and 2021.
   - Components: Region, Country, Division.
   - Compare market performance vs. target.
   - Display data for each country: 2019, 2020, 2021, Target, Data 2021, Target %.

### 5. Profit and Loss Statement:
   - Calculate Net Sales, Cost of Goods Sold (COGS), Gross Margin, and Gross Margin Percentage.
      - Net Sales - 25
      - COGS - 20
      - Gross Margin = Net Sales - COGS = 25-20 = 5
      - Gross Margin % = (Gross Margin / Net Sales) * 100 = (5 / 25) * 100 = 20%

### 6. Formatting:
   - Use the Avenir Next LT Pro font for the report.

### 7. Time-based Analysis:
   - Add Quarter information: "Q" & ROUNDUP([FY_Month_number]/3,0).
   - Add Month Name: FORMAT([date],"MMM").
   - Add Month Number: Month([date]).

### 8. Feasibility and Impact Matrix:
   - Create a matrix to assess the feasibility and impact of various actions.

### 9. Additional Considerations:
   - Ensure exclusive reference to Atliq data.
   - Check and fix Altig Excelusive.
   - Verify and handle NaN values in region values in the market.
   - Perform a final check on data cleanliness and uniqueness.

### 10. Report Design:
   - Organize the report in a clean and visually appealing layout.
   - Utilize the specified font (Avenir Next LT Pro).
   - Consider color-coding and visual elements for better presentation.

### 11. Data Pipeline:
   - Implement a data pipeline for seamless data flow and updates.

By following this organized plan, you can efficiently clean the data, set up a database, and create a comprehensive report that covers customer performance, market analysis, and financial insights for Atliq.
