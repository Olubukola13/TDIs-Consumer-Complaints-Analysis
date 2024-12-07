#  Financial Complaints Detective: Unlocking Insights for Customer Advocacy

## Project Overview 

This project focuses on analyzing a dataset of consumer complaints to extract meaningful insights and actionable recommendations. By utilizing Microsoft Excel for data cleaning, analysis, and visualization, i aim to address key questions about consumer dissatisfaction, company performance, and customer service efficiency

## Data Source

Consumer Complaints: The primary dataset used for this dataset is the "Consumer_Complaints_xlsx" file containing detailed information about each compplaint made by consumer.

## Problem Statement
Consumer complaints provide valuable insights into the challenges faced by customers across different products and sub product. However, organizations often struggle to identify actionable trends due to the volume and complexity of the data. 

The key challenges are:
- Identifying trend in consumer complaint by year.
- Identifying the most common issues faced by consumers and the products with the most complaint.
- Understanding the timeliness of company responses and its impact on customer satisfaction.
- Analyzing complaint trends across different states and submission channels to uncover regional or operational inefficiencies.

This project aims to analyze consumer complaint data to uncover trends, evaluate company response times, and provide actionable insights to improve customer experience and operational efficiency.


## Tools
- Microsoft Excel: For data cleaning, analysis, and visualization.
- GitHub: For project documentation and sharing.

## Data Cleanining/Preparation
In the initial data preparation phase, i perform the following tasks:
1. Load the dataset into Excel.
2. Clean and preprocess the data (e.g format dates, handle missing values).
3. Perform exploratory data analysis using PivotTables, charts, and formulas.
4. Document key insights and recommendations based on the analysis.


## Exploratory Data Analysis

EDA involved exploring the consumer complaints data to answer key question, such as: 

- What is the overall trend in consumer complaint by year?
- What is the common issue faced by consumers?
- Which states has the highest number of complaint?
- Which product ha sthe highest complaint?

## 1. Data Analysis

Here are some Excel funtions and techniques i applied during the project.

### Data Cleaning
- `TEXT()` Function:
  - Used to standardize date formats into a consistent format
    ```excel
    =TEXT(C2, "MM/DD/YYYY")
    ```
### 2. Calculated Field 
- Year Extract from Dates:
  - Extracted the year from the complaint submission date to analyze trends:  
    ```excel
    =TEXT([@[Date submitted]],"yyyy")
    ```
    
- Month Name Extract from Dates:  
  - Generated the month name from the complaint submission date:  
    ```excel
    =TEXT([@[Date submitted]],"mmmm")
    ```
- Reception Days:
  - Gotten from the diffrence between complaint submission date and date the complaint was received:
    ```excel
    ==DAYS([@[Date received]],  [@[Date submitted]])
    ```

  ### Visualisations
  - Dynamic Pivot Tables:
    - Created pivot tables to analyze the number of complaints and response patterns across various dimensions (e.g., product, company, state).
    - Used slicers to dynamically filter complaints by state, product, and submission channel.
  - Charts
     - Created charts to present key insights,

  ### Results/Findings

  The analysis results are summerized as follows:

  










  
  
