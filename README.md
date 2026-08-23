# Customer Purchasing Behavior analysis 

### Project Overview 

This is an E-commerce Customer behavior and consumer insight Dashboard built with Microsoft Power BI to analyze the shopping behavior across 254 E-commerce customer's, this analysis focuses particularly on identifying high value customer segments, growth opportunities and patterns that can support marketing and business strategy.

### Data Sources 


### Tools 
 - Power query - Data cleaning, transformation, text trimming and conditional columns. 
 - Dax - KPI measures, calculated columns and aggregation. 
 - Power BI - Dashboard development, slicers and dat visualization.


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

