# Company-Sales-Methods-Analysis
Uncover the Key to the Most Effective Sales Strategies for an Office Stationery Company

**Author: Abraham Saenz Sigala**

**Date: December 21, 2024**

:floppy_disk: File: [Python Jupyter Notebook](Product_Sales_Project_Jupyter_Notebook_2.ipynb)

##

### Scenario: 

The Sales Representative for an office stationery supply company has urgently requested an analysis from the Head of Analytics to assess the effectiveness of various sales methods, with the goal of identifying the best approach for launching a new product line. The analysis must address several key questions:

1. The number of customers for each sales approach.
2. The overall revenue distribution, as well as for each method.
3. Any differences in revenue over time for each approach.
4. A recommendation for which method to continue using, considering time efficiency.

The Sales Rep emphasizes that some methods take more time, so if the results are similar, those methods may not be the best choice. Additionally, they request insights into any differences between customer groups to provide context for the analysis. The analysis should be presented to the Sales Rep within the next four weeks for reporting to the executive team.

##

### :construction: Dataset Limitations:

- We are working with 6 weeks worth of data as this is what the stakeholder provided.
- We have no information on the time of day the sale was made.
- They haven’t included numbers for how much time was spent on each customer.

##

### :soap: Data Cleaning:

🛠️ Tool: Python Jupyter Notebook (Packages: Pandas)

Data Validation:
 
The dataset contains **15,000 rows and 8 columns** before cleaning and validation:

- week: Week sale was made, counted as weeks since product launch. Numeric, 6 different weeks total. No missing values. No cleaning needed.
- sales_method: Character, which of the three sales methods were used for that customer. 5 sales methods in dataset, cleaned for consistency. 3 unique values after cleaning. No missing values.
- customer_id: Character, unique identifier for the customer. No missing values or duplicates. No cleaning needed.
- nb_sold: Numeric, number of new products sold. No missing values. No cleaning needed.
- revenue: Numeric, rounded to 2 decimal places. 1,074 missing values. Fill NaN with the average revenue grouped by sales method and items sold. Cleaned, no missing values.
- years_as_customer: Numeric, number of years the customer has been buying from us (company founded in 1984). Assuming data is from 2023, there are 2 values that exceed the company’s founding date (< 39 years). Drop these two rows as we do not know the true years as customer.
- nb_site_visits: Numeric, number of times the customer has visited our website in the last 6 months. No missing values. No cleaning needed.
- state: Character, location of the customer i.e. where orders are shipped. 50 unique values (50 states). No missing values. No cleaning needed.

After the data validation and cleaning, the dataset contains **14,998 rows and 8 columns** without missing values or duplicates.

##

### :microscope: Data Analysis

Analyze the data to discover insights and answer the questions for the stakeholder.

🛠️ Tool: Python Jupyter Notebook (Packages: Pandas, Matplotlib, Seaborn) 

:floppy_disk: File: [Python Jupyter Notebook](Product_Sales_Project_Jupyter_Notebook_2.ipynb)

##

###  :clipboard: Visualize, Report and Present:

Once the analysis was complete, we shared our insights on what the most effective sales method was with stakeholders by providing a detailed report in Markdown format, along with a presentation to effectively convey our findings to a non-technical audience.

:pencil: [Markdown Report](Sales_Method_Analysis_Report.pdf)

:bar_chart: [Presentation](SalesMethod_Presentation.pdf)

##

### :unlock: Business Metrics and Recommendations:

:chart_with_upwards_trend: *Business Metrics*

I recommend focusing on two key metrics to evaluate the effectiveness of our analysis for the new product line:

**1. Number of Customers Reached per Sales Method**

- A rise in customer reach through the Email + Call approach, along with a decline for the Call-only method, confirms that we are prioritizing the most effective sales strategies. For example, a 5% increase in Email + Call reach resulted in 373 additional customers, directly contributing to higher revenue.

**2. Increase in Weekly Revenue**

- An increase in weekly revenue for the Email and Email + Call approaches specifically—by a certain percentage—indicates positive progress toward our goals. For instance, a 10% rise in weekly revenue each week for Email + Call demonstrates strong progress toward our objectives.

:bulb: *Recommendations*

Over the next six weeks, I would recommend:

1. Eliminate the Call-Only Sales Method:
   
- Although it has a decent success rate due to the time invested, it generates the least revenue and consumes more time. I recommend not eliminating it entirely in the future.

2. Prioritize the Call + Email Approach:
   
- This method consistently delivers the highest revenue per sale. Focus on maximizing returns and improving its rough start.

3. Optimize the Email-Only Sales Method:
   
- While it has been effective in terms of success and revenue, aim to avoid drastic drops in weekly revenue over time.

4. Reduce Call Duration in the Call + Email Approach:
   
- Lower the average call time from 10 minutes to save time and costs. Complete optimization efforts by combining the Email + Call approaches to enhance efficiency.

5. Further Analysis Recommendations
    
- Regional Suitability:
Determine if sales methods perform differently across states.

- Customer Preferences:
Align strategies based on customer preferences. For example, consider customers who prefer certain sales methods and ask for emails if a call is preferred.

6. Enhance Data Quality:
   
- Include customer demographic details, such as age.
- Track sales duration to evaluate time-efficiency for each sales method.
- Record the time of day to identify optimal periods for each sales approach.



