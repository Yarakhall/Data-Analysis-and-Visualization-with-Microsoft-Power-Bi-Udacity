# **Create a Data Model for Seven Sages Brewing Company**

First Project of Udacity's [Data Analysis and Visualization with Microsoft Power BI Nanodegree Program](https://www.udacity.com/course/data-analysis-and-visualization-with-power-BI-nanodegree--nd331)
in **Introduction to Preparing and Modeling Data** course.

## Project Overvieww:
In this project, you'll create a data model and Power BI report for Seven Sages Brewing Company that combines information from all over the company. Your data model will make it possible for the company's CFO to quickly review and analyze what beers sell well and which ones generate the highest profitability.

At the end, you will have applied the key concepts of this course to combine and centralize data that was previously siloed, solving a very common issue facing many companies. More importantly, you'll have a solid foundation to build on when it comes to more complex reporting visualization demands, advanced DAX requirements, or larger data models. No matter how large the data models get as your career progresses, the core principles remain the same.

Below is a quick demonestration about project steps.

### STEP 1: Get the source files:
used files are `CFO Metrics Tracker.xlsx`, `Customer List (as of FY2021).txt`,
 `SSBC Product Offerings.pdf`, `USD-CAD Exchange Rates.csv`, 
 `Monthly Sales Logs/` 
 can be found on `Data Sources Files/` folder on this repositories


### STEP 2: Structure, Combine, and Clean the Data:
Before going any further, make sure you've done the following:
  - Promote first rows to headers as needed.
  - Review data types for each field to ensure that they are identified correctly (e.g., dates should be recognized as
"date type").
  - Similarly, rename any unclear columns so you can easily find and use them.
  - Merge dimension tables with a 1-to-1 relationship.
  - Ensure that the Sales folder has been correctly combined (or append the files if using the folders is causing difficulties).
  - Create any foreign keys that are needed to support your data model design but can be made from available data.
  - Remove any and all blank rows.
  - Delete unnecessary columns (remember--you can always undo overzealous deletions if you find you need a column later on).
  - Correct any obvious typos that will impact report results.
  - Address data gaps (when a logical solution exists to address them).


### STEP 3: Create Your Date Table:
You'll want to create a continuous table that covers each full calendar year in the sales data set (starting on January 1st and ending on December 31st. In addition, the table should include:
  - Calendar month name and number
  - Calendar year
  - Fiscal period
  - Fiscal year
  - Fiscal quarter -Quarter - FY (e.g., Q1 - FY2021)
  
> Note: Seven Sages' Fiscal year begins on October 1st and runs until September 30th. A transaction on Sept 20th 2020 would fall in FY 2020, but a transaction on October 20th would land in FY 2021


### STEP 4: Build Relationships Between Tables:
We ended up with one fact table `Full 2021 Sales` and four diminsion tables pointing towards it with an active one to many relationship.


### STEP 5: Write Your Measures:
To satisfy the CFO's requirements, we will need to calculate Sales, Cost of Sales and Gross Profit Margin in two different currencie
Here's what you'll need to do:
  - Sales in USD ($)
  - Cost of Sales USD ($)
  - Gross Profit Margin (or GPM) in USD (%)
  - Sales in CAD ($)
  - Unit Sales by Product (%)
  - Share of gross profit by Product type (%)


### STEP 6: Create a Report
we just need to create a visualization to summarize the output of your data model for the CFO.
The basic version of this report will have two tabs, one summarizing sales by customer and customer type across quarters. The second will simply summarize the percentages of gross profit and unit sales by product.
In both instances, the CFO would like a very brief Executive Summary at the bottom of the tab.



