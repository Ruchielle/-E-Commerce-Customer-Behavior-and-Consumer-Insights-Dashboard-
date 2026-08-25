# Customer Purchasing Behavior analysis 

### Project Overview 
An e-commerce retail business, wanted to better understand its customers and the factors influencing their shopping behavior. However, it lacked clear insights into which customer segments spend the most, which products and categories are most preferred, how shopping patterns vary across age, gender, financial status, and city tiers, and where the strongest customer opportunities lie.
Using Power BI, this project analyzes data from 254 customers to uncover key purchasing patterns, identify high-value customer segments, and highlight growth opportunities that can support more targeted marketing, product, and business decisions.


### Project Objectives 
The main objectives of this project were to:
 - Understand customer purchasing behavior patterns.
 - Identify high value customer segments.
 - Analyze demographic influences on shopping preferences.
 - Understand spending behavior across city tiers.
 - Analyze product preferences by gender.
 - Support data driven marketing and business strategy decisions.
 


### Tools 
 - Power query - Data cleaning, transformation, text trimming and conditional columns. 
 - Dax - KPI measures, calculated columns and aggregation. 
 - Power BI - Dashboard development, slicers and dat visualization.


### Data Workflow 
 - Source 
    - Where did the data come from?
        - The dataset was sourced from Kaggle and contains 254 e-commerce customer records with information on customer demographics, shopping behavior, product preferences, spending, and other customer attributes.

 - Ingestion 
     - How was the data brought in?
         - The dataset was imported into Microsoft Power BI for data preparation, modeling, analysis, and visualization.

 - Cleaning 
     - What issues did you find and fix?
         - The data was reviewed for missing and inconsistent values. Missing values in the City field were identified and handled by categorizing them as “Unknown” to prevent the missing records from being excluded from the analysis.

 - Transformation 
     - What new fields, aggregations, or structures did you create?
         - Missing values in the City field were handled by replacing the 31 blank entries with “Unknown.” Spending-related data was also structured into meaningful spending categories to support customer segmentation and comparison in Power BI.

 - Analysis 
      - What statistical structures, queries, or visuals did you use?
          - The analysis focused on customer demographics, product-category preferences, shopping frequency, spending behavior, financial status, gender, age, marital status, and city tier. Power BI measures, aggregations, and interactive visualizations were used to identify patterns and compare customer segments.

 - Output 
      - What form did the results take?
           - The results were presented as an interactive Microsoft Power BI dashboard containing KPI cards, charts, and visual breakdowns of customer behavior and purchasing patterns. The dashboard provides insights into high-value customer segments, product preferences, and potential growth opportunities.



### Key Metrics
 - Total Customers
      - Measures the total number of customers analyzed in the dataset.
 - Average Spending 
      - Shows the average amount spent by customers and helps indicate overall customer value.
 - Average Shopping Frequency
      - Shows how often customers shop and helps measure customer engagement.
 - Brand Preference
      - Identifies the brands most preferred by customers and highlights customer preferences.
 - Top Product Category
      - Identifies the product category with the highest customer preference or demand



### Data Cleaning and Transformation 
Before creating the dashboard the raw data was reviewed and cleaned to ensure that the analysis and visualization were reliable. 
Here are the steps that i took:
 - Column review 
    - All 18 columns were reviewed to determine which fields were relevant to the business objectives.

 - Removed Irrelevant Columns 
    - Two columns were removed because they were not relevant to the project’s shopping behavior focus and they are: 
        - OTT Subscription
	      - Book Type

 - Renamed Columns 
    - Long survey question fields were renamed into shorter, professional column names to improve readability within the Power BI data model.

 - Handled Missing Values 
   - This prevented missing responses from being incorrectly interpreted as blank records,missing values were addressed as follows:
	 - Missing City values → Unknown
	 - Missing Electronics Preference values → Not Applicable
	 - Missing Fashion Preference values → Not Applicable
     - Missing Clothing Preference values → Not Applicable

 - Duplicate Check 
    - The dataset was checked for duplicate rows an no duplicate rows were identified.

 - Age data Cleaning 
   - The Age column required additional cleaning.
     - One entry recorded as "50 years" and was corrected to 50
     - An invalid entry containing the name "Anurag Dubey" was found in the Age field and replaced with a blank/null value.
      - The Age column was then converted from text to a whole number in Power Query and this also resolved downstream DAX comparison issues.



### Exploratry Data Analysis 
 - Who are our customers? 
     - What age, gender, income level, and location make up our customer base?

 - How often do customers shop, and who shops the most? 
     - Which age group and income group are the most active buyers?
 
 - How much do customers spend, and who are the high value customers? 
     - Which segments are Low, Medium, or High spenders, and where are they concentrated. 
 
 - What do customers prefer to buy? 
     - Which product categories are most popular overall, and does that preference change by gender?
 
 - Do customers care more about brand or price? 
     - Are they loyal to brands, or are they price driven shoppers?
 
 - How fast do customers decide to buy? 
     - Do they make quick decisions, or take time to research before purchasing?
 
 - Where are our customers located, and what kind of city do they live in? 
     - Which states have the most customers, and are they in big cities (Tier 1) or smaller ones (Tier 2/3)?



### Key Insights and Visuals
 - Product Category Distribution 
      - Clothing is the strongest product category
           - The Product Category visual shows that Clothing had the highest number of respondents, with 85 customers selecting it as their preferred product category.

 - Spending Category by City Tier 
      - Medium spenders represent the biggest opportunity
           - The Spending Category by City Tier visual shows that medium-spending customers (customers who spend between 1,000 and 5,000) form the largest spending group across every city tier. Tier 2 is particularly important, with 46.7% of respondents falling into the medium-spending category.

 - Shopping Frequency by Age Group 
      - Younger customers shop more frequently
             - The Shopping Frequency by Age Group visual shows that shopping frequency is strongest among customers aged 20–39, while customers aged 50+ have the lowest average shopping frequency.

 - Product Category by Gender 
      - Gender influences secondary product preferences
              - The Product Category by Gender visual shows that both men and women prefer Clothing, but their secondary preferences differ:
                     - Men Electronics
                     - Women Fashion

 - Purchase Decision Time 
      - Most customers make purchasing decisions quickly
             - The Purchase Decision Time visual shows that the majority of customers make their purchasing decisions within a day, indicating relatively short consideration periods for many products.