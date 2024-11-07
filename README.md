# Airline-Loyalty-Program-Analysis

https://medium.com/@kwanqi.yt/data-analysis-project-airline-loyalty-program-analysis-bd9b05e5def9

# About the Company
Northern Lights Air (NLA), an airline in Canada has a simple yet profound belief: everyone can fly. Dedicated to becoming the top choice for air travel, NLA continuously strives to serve its community better. To further this mission, they are harnessing the power of data analysis to transform their business vision into reality.

# Project Brief
In this project, I’ve taken a role of a Data Analyst for NLA. From February to April 2018, NLA launched a Customer Loyalty Program aimed at boosting membership enrolment. The airline now seeks to understand the campaign’s impact and identify the seasons when new members prefer to travel.

# Business Objectives
NLA’s primary goal is to compare enrollment counts before and after the campaign period. Using historical data from January 2016 to July 2018, they have outlined several key business questions:

1. Was the promotion program a success?

2. What impact did the campaign have on loyalty program memberships?

3. Did the campaign resonate more with certain demographic groups?

4. Which is the most popular season for the new members to travel in?

# About the Dataset
Dataset contains 3 CSV tables :

Calendar Table : Ensures consistency of date intervals for data modelling.

Customer Loyalty History Table: Contains details of 16,000 customers, including location, education background, membership status, and cancellation status.

Customer Flight Activity Table: Includes over 39,000 records including travel month and distance travelled per trip.

# Fact and Dimension Tables
Fact Table: The Customer Flight Activity table, containing numerical data without unique identifiers, serves as the fact table.

Dimension Table: The Calendar and Customer Loyalty History tables, each with primary keys (e.g., Loyalty Number), provide context and background information.

# Data Processing (ETL — Extract, Transform, Load)
Using Power BI, I started with data importing, preparing, and finally analysing the data. Here’s a snapshot of the key steps involved.

Once imported all 3 files, I performed the following tasks to ensure the data is well prepared for the analysis :

- Promoted headers for proper column naming.

- Created a YYYY-MM identifier in the Calendar table to connect with other tables.

- Merged Year and Month columns in the Customer Loyalty History and Customer Flight Activity tables.

- Ensured correct data types and removed duplicates and null values.

# Data Modelling

To establish relationships between the datasets, I used the YYYY-MM identifier, organizing the data into a star-schema model. This model enhances query performance by structuring data into a central fact table linked to dimension tables, resembling a star.

# Data Analysis & Insights

With data preparation complete, it was time to dive into the analysis and answer the business questions!

1. Is the promotion program a success?

Yes, it was. Before the promotion, monthly enrolment ranged from 185 to 210. Post-promotion (Feb-Apr 2018), enrolment consistently exceeded 230. Though data limitations exist, the trend suggests a positive impact.

2. What is the Year-On-Year (YoY) impact on loyalty program memberships? How did the campaign boost the enrolment count?

I used DAX to calculate the YoY Comparison. During the campaign period, membership enrolment surged by 30–70% compared to the same period the previous year. Despite a sharp drop in May, the overall YoY increase outperformed the mere 2% rise seen in January.

3. Was the campaign adoption more successful for certain demographics of loyalty members?

Education : 

Yes, among the new membership, 613 (64%) members hold a Bachelor’s degree and 238 (25%) hold College Certification.
We can assume those filled up Bachelor’s & College degree education background are all working adults, and these are also NLA’s main target customers where they have steady income stream and a thirst for travelling. This indicates NLA’s customer base have strong purchasing power. This can be further drilled down by the customer’s family background, whether they travel alone, in pair or with family.

Marital Status : 

Over 50% of the new members signed up during the campaign are married.Based on this, we can gather those who are married will be travelling in pairs (at least), and singles will either be travelling alone or with friends. Either way, this piece of analysis shares great insights to NLA on their marketing campaign.

Location : 

Ontario, British Columbia, and Quebec saw the highest membership sign-ups. This comes to no surprise to NLA. According to Wikipedia, Ontario, British Columbia, Quebec, Alberta accounts to approx. 85% of total population of Canada. Moreover, there are 2 main airports in Canada, YUL (Montreal, Quebec) and YVR (Vancouver, British Columbia) where the flights frequency is higher.

# Recommendation :
By combining all these 3 factors, NLA target market would be Married & Single, with Bachelor & College education background and based in 3 major cities (Quebec & British Columbia).

- NLA can develop different market strategy to cater to the market, for example creating promotion to travel for couples only during the month of February to celebrate the love month, or creating family promotion during Summer.

- NLA should consider create safety advertisement or ease travelling kids (like British Airline) to build confidence to the parents to travel with NLA.

- NLA can also consider developing a mystery destination travel package ,similar to Scandinavian airline did, in which this campaign can be targeted to the customer base who are single.

4. Which season is the most popular among the new members to travel in?

29.5km of travels have been booked to travel during Spring, while 14.4km of travels have been booked to travel in Winter.According to Durham Immigration Portal, Spring in Canada happens from Mar to May and Winter happens from December to February. Spring being the most popular season to travel in comes as a surprise. This unexpected trend highlights a preference for spring travel over the long summer holiday.

# Data Visualization

For further analysis and exploration, I have uploaded an interactive Power BI file here. This allows deeper insights and more nuanced understanding of the data.

# Next Step and other Recommendations

Data Collection : 
Collect data for at least six months post-event to better assess campaign effectiveness, as the current data timeframe is too short.

Marketing and Promotion Strategy : 
This campaign might not be a sustainable way to boost the enrolment for a long term, a targeted marketing campaign on certain demographics group would generate more impactful outcome.

Thank you for staying until the end. Should you need any collaboration, you can reach me on at kwanqi.yt@gmail.com.
