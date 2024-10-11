# Analysis the online store annual report.						


## Problem Statement

This dashboard helps businesses gain deeper insights into their sales performance and customer behavior. By analyzing various metrics, businesses can identify key areas for improvement in sales strategies and operational efficiency. The dashboard provides valuable information, such as:

- Top 5 States by Sales: It identifies the top-performing states, allowing the business to focus marketing and sales efforts on regions with the highest revenue potential.

- Orders by Age Group: The dashboard categorizes orders by customer age group, helping businesses better understand the demographics of their customer base and tailor products or services accordingly.

- Annual Order Status Report: By analyzing order statuses (e.g., completed, pending, cancelled), businesses can track operational performance and identify inefficiencies in order management throughout the year.

- Monthly Sales and Orders Trends: The dashboard visualizes sales and orders trends over time, allowing businesses to identify peak seasons and make data-driven decisions for inventory and resource planning.

- Sales Percentage by Gender: By calculating sales contributions based on gender, businesses can target specific customer segments and optimize marketing strategies.

- Sales by Channel: The dashboard organizes sales data by sales channel (e.g., online, in-store), providing insights into which channels contribute the most revenue and helping the business refine its omnichannel strategy.

Overall, this dashboard helps businesses improve their sales performance, streamline operations, and better understand their customers, leading to more informed decision-making and enhanced customer satisfaction.




### Steps followed 

### Step 1 : Import Data into Excel
- The dataset was imported into Excel from external sources.
- The Data tab was used to import the file via options like:
    - i) From CSV: for reading data stored in CSV format.
    - ii) From Excel Workbook: for importing data from another Excel file.
    - iii) From Database: to extract data directly from SQL servers or web-based APIs.
- The data was loaded into a structured table format for easier processing and analysis.

### Step 2 :Review Data
- Reviewed the dataset to ensure completeness and correctness.
- Checked for missing values, nulls, and inconsistent data formats.
- Verified that the necessary fields (columns) for the analysis were present and - in the correct format.

### Step 3 : Data Cleaning
- Applied the following cleaning techniques to make the data analysis-ready:
    - i) Filters were applied on relevant columns to sort the data, remove null values, and replace inconsistent values.
    - ii) Data sorting was used to identify and organize the data for easier review.
    - iii) Find & Replace functions were used to remove unwanted values (e.g., "N/A")  and replace them with zeros or relevant placeholders.



 ###  Step 4 :Data Processing According to Problem Statement
 - Based on the problem requirements, specific columns were created to enable analysis:
     - i) Age Grouping: A new column was added to categorize customers into different age groups (Child, Young Adult, Adult, Senior). This was achieved using conditional formulas in Excel.
    - ii) Month Column: Extracted the month from the Order Date column using Excel formulas to enable time-based trend analysis. This was part of the ETL (Extract, Transform, Load) process.


### Step 5 :  Analysis Using Pivot Tables and Charts
- i) Top 5 Sales by State:

    - a) A PivotTable was created to show the top 5 states based on sales. The State column was added to the Rows field, and the Sales column was added to the Values field. The data was sorted in descending order to find the top 5 performing states.

![Screenshot 2024-10-11 232141](https://github.com/user-attachments/assets/4f585d01-39fa-4883-bd13-69a00968b8ab)

- ii) Sales by Age Group:

   - a) A PivotTable was used to group orders by the newly created Age Group column. The Age Group column was placed in the Rows field, and the count of orders was placed in the Values field.


![Screenshot 2024-10-11 232434](https://github.com/user-attachments/assets/a9dbb506-5a5e-4318-968f-88b93af890aa)

- iii) Sales by Gender:

    - a) Another PivotTable was created to analyze sales by gender. The Gender column was placed in the Rows field, and the Sales column in the Values field to track the sales performance across different genders.

![Screenshot 2024-10-11 232625](https://github.com/user-attachments/assets/0debe8f2-6949-490a-ac3c-1168cf37f1ee)

- iv) Sales and Orders Trend Analysis Using Charts:

    - a) Monthly sales and order trends were analyzed using charts generated from PivotTables. The Month column was placed in the Rows field to plot sales and orders over time. The charts provided insights into peak and low sales months.
The charts were customized with line graphs and bar charts for better visual representation.


### Filters

![Screenshot 2024-10-11 233029](https://github.com/user-attachments/assets/a5cab6bd-785c-4811-b536-3d8342ec8670)


# Snapshot of Dashboard

![Screenshot 2024-10-11 233336](https://github.com/user-attachments/assets/aa7ded01-c00b-4868-9554-c3c712cf104f)



# Insights

A single page report was created on Excel & it was then published on github.

Following inferences can be drawn from the dashboard;

### [1] Top-5 Sales Accoroding to State = 129880

   MAHARASTRA = 2990221

   KARNATAKA = 2646358

  UTTAR PRADESH = 2104659

  TELANGANA = 1711827

  TAMIL NADU = 1678877


           thus, higher sales  on Maharstra state .
           
### [2] Sales per acc. to age group.

    a) Adult(men = 19.35% , women = 43.57%)

    b) Senior Citizen (men = 5.19%, women = 19.70% )

    c) Youth (men = 5.32% , women = 12.15% )

   
  while calculating average , null values have been ignored as they were not relevant for some customers. 
  
  These ratings will change if different visual filters will be applied.  
  
  ### [3] Top -3 channels accoroding to sales  
  
      a) Amazon  - 35.48%
      b) Myntra - 23.37%
      c) Flipkart - 21.59%
      
Values  will change if different visual filters will be applied.

 ### [4] Sales accoroding to gender

     a) Men  - 35.95%
     b) Women - 64.05%
 
 
        
### My Conclusions

According to previous data our final conclusion is "Target the woman customer(25-50) in the hot summer session, who is living in the MH, KA, & UP, and run marketing campaine in Amazon, Myntra and Flipkart".
