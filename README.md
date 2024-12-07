#  Consumer Complaint Pattern: Insights and Recommendations for Better Customer Experience

## Project Overview 

This project focuses on analyzing a dataset of consumer complaints to extract meaningful insights and actionable recommendations. By utilizing Microsoft Excel for data cleaning, analysis, and visualization, i aim to address key questions about consumer dissatisfaction, company performance, and customer service efficiency.


![Dashboard](https://github.com/user-attachments/assets/c7323687-992b-4e1c-ad99-9fa352ad59fb)


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

  ### Outputs 
  - Visualizations:
   - Line chart: Complaint trends over time.  
   - Bar chart: Complaint distribution by product, issue, and Untimely Company Responses to Consumer Complaints 
   - Column chart: Complaint distribution by state.
   - Pie chart: Submission modes and their effectiveness.  

   ### Results/Findings
   - Consumer complaints increased significantly between the year 2019 to 2022 and later dropped in 2023.
   - The most common complaint issues is managing an account. 
   - The product with the highest complaints counts is cheecking account.
   - The sub product with the highest complaint counts is checking or savings account.
   - States with higher complaint.
   - Web submission channel has the highest untimely response.

   ### Recommendations

  Based on the analysis imrecommend the following actions:

   - Identify specific trends in states with higher complaint volumes and tailor solutions accordingly. Strengthen regional customer service centers to improve accessibility and efficiency.
     - Collaborate with local branches to address state-specific challenges proactively. Addressing the 2019–2022 Complaint Spike.
    
   - Conduct a root cause analysis of complaints related to checking and savings accounts.
     - Enhance training for frontline staff to address common issues tied to these products.
     - Offer additional support channels, such as live chat or priority service, for customers experiencing account-related challenges.
     - Improving Service in High-Complaint States
    
   - Develop user-friendly guides and tutorials for managing accounts effectively.
    - Implement robust account management features on digital platforms to minimize issues.
    - Regularly audit account management services to identify and resolve process inefficiencies.

   - Increasing Awareness and Support for Web Submissions
     - Since the web submission channel has the highest untimely responses, streamline the process by implementing automated 
       acknowledgment messages for complaints submitted via the web.
     - Allocate more resources to the web team to ensure timely handling of complaints.
  
   
 
  

  










  
  
