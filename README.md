# Descriptive Analysis 
## Project Description: Descriptive Analysis of Consulting Business License Applications in Vancouver

## Project Title: Descriptive Analysis of Consulting Business License Applications in Vancouver
## Objective:
- The primary objective of this project is to conduct a descriptive analysis of consulting business license applications in Vancouver for the years 2023 and 2024. This analysis will summarize key characteristics of license applications, identify trends, and generate insights that can help inform decision-making for city planners, business analysts, and other stakeholders.
## Dataset:
The dataset contains consulting business license application data from the City of Vancouver, specifically focusing on consulting businesses. The key features include:
- Application ID: Unique identifier for each license application.
- Licence RSN: License record serial number (sensitive information).
- Licence Number: Unique license number for each business (sensitive information).
- Business Name: Name of the business applying for the license.
- Business Trade Name: Trade name (if different from the business name).
- Status: Current Status of the license (e.g., Issued, Inactive, Gone Out of Business).
- Issued Date: Date when the license was issued.
- Expired Date: Expiration date of the license.
- Business Type: The type of business, which in this case is "Consulting and Management Services."
- Location Information: House number, Street, City, Province, Country, and postal code.
- Number of Employees: Number of employees for each company.
- Fee Paid: Amount of fee paid for the license by the companies.
## Methodology:
1.	Data Collection and Preparation:
Data Source: The dataset for business license applications for the years 2023 and 2024 was collected from publicly available City of Vancouver records.
2.	Tools Used: 
 - Amazon S3: The unstructured dataset is stored in the Landing folder of the S3 bucket. Cleaned and structure datasets were stored in the Raw and Curated folders of the S3 buckets for easy access and querying.
- AWS Glue DataBrew & AWS Glue: Data cleaning and preparation were performed to handle missing values, correct data types, and remove duplicates.
- Amazon Athena: The dataset was queried using SQL to prepare for analysis.
Data Cleaning:  Addressed missing values (e.g., business trade name, number of employee). And removed duplicates and corrected inconsistent data types (e.g., converting dates to a standard format).
## Descriptive Statistics:
### Key Metrics Calculated:
1.	Number of Licenses Issued: Total count of business licenses issued each year.
2.	License Status Breakdown: Distribution of licenses by status (active, inactive, or out of business).
3.	License Duration: Analyzed the gap between issued and expired dates to assess how long businesses remained active.
4.	Employee Count and Fee Paid (2024): Summarized the total fees paid by businesses and correlated them with the size of the business.
## Data Visualization:
Detailed visual representations were created to summarize the descriptive statistics of our findings:
- Time-Series Graph: Shows the number of licenses issued each month in 2023 and 2024, highlighting trends in business activity.
- Pie Chart: Represents the distribution of business statuses (e.g., active, inactive, gone out of business).
- Bar Chart: Compares the total license fees paid by consulting businesses based on the number of employees (for 2024).
## Customer Segmentation and Analysis:
Although not directly related to customer purchases, businesses were segmented based on:
- Size (Employee Count): Analyzed businesses by employee count to compare how larger vs. smaller consulting firms behaved in terms of license status and fee paid.
- Status Trends: Analyzed how the license status changed over time, identifying peak periods of business activity and closures.
## Insights and Findings:
- Peak Licensing Periods: There were noticeable peaks in the number of licenses issued in early 2023 and mid-2024, corresponding to business growth periods.
- License Expiration and Closure Trends: Many businesses that received licenses in 2023 had expired by early 2024, suggesting a high turnover rate in the consulting industry.
- Fee Insights: Larger consulting firms (with more employees) paid higher license fees in 2024. However, a significant number of smaller firms still constituted the bulk of issued licenses.
## Recommendations:
Based on the descriptive analysis, the following recommendations were made:
- Support for Small Businesses: The City of Vancouver could consider providing additional support to smaller consulting businesses to reduce their high closure rates.
- Targeted Marketing and Services: The licensing department could provide more targeted services and marketing based on the business size to improve renewal rates.
- Policy Adjustments: Adjust fee structures to ensure fairness and provide incentives for businesses to maintain active status over a longer period.
## Tools and Technologies:
 (https://github.com/SKrishna003/Data-Analyst-SaiKrishna/blob/main/Consulting%20Business-Drawio.jpg)
 
AWS Services Used:
1.	Amazon S3: To store the raw, processed, and cleaned datasets, S3 bucketsa re 
2.	AWS Glue DataBrew: To automate the cleaning and preparation of the dataset.
3.	AWS Glue:
- ETL Process: AWS Glue was used to automate the ETL processes which includes extracting the data from the raw folder of S3 bucket, transform the cleaned data curated to ensure consistency across both 2023 and 2024 datasets, and load the transformed data back into the curated folder of the Amazon S3 buckets for further querying and analysis.
- Glue Job: Automated data transformation jobs to handle changes in schemas and formats.
- Glue Data Catalog: Managed metadata and organized datasets to ensure efficient querying with Amazon Athena.
4.	Amazon Athena: To run SQL queries and calculate descriptive statistics for analysis.
5.	AWS Lambda: For automating ETL (Extract, Transform, Load) tasks in data pipelines.
6.	AWS Identity and Access Management (IAM): For secure access control.
7.	AWS Key Management Service (KMS): To encrypt data stored in S3, ensuring security compliance.
## Deliverables:
1. Detailed Report:
 - A comprehensive report summarizing the entire descriptive analysis process, insights, and findings.
 - Includes statistics on the number of licenses issued, business statuses, licensing trends, and fee analysis.
   
2. Visualizations and Dashboards:
- Time-Series Graph: Monthly trend of license applications.
- Pie Chart: Status distribution (active, inactive, gone out of business).
- Bar Chart: Fee analysis based on employee count.
3. Presentation for Stakeholders:
  A summarized presentation with key findings, recommendations, and visualizations. This presentation is meant to guide city officials and other stakeholders in understanding the consulting business landscape in Vancouver and taking informed actions.
# Conclusion:
This descriptive analysis provides valuable insights of identifying the business licenses that are about to expire, and we can predict the number of applications to expect for renewal based on the consulting business license applications in Vancouver for the years 2023 and 2024. By analyzing licensing trends, and business statuses, stakeholders can make data-driven decisions to optimize licensing planning.
