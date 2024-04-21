# Hospitality-Domain-Data-Analysis
A BI report on a hotels dataset that has 3 months of data



# Business Requirements:
Like any business, operating a hotel takes hard work and constant analysis. To survive in the hospitality industry, hotels must benchmark their performance throughout the year and compare it to their competitive set. Some of the requirements include:

- Revenue Management: Developing strategies to optimize room rates and occupancy rates throughout the year is essential. This may involve dynamic pricing, packages, and promotions. Data analysis is crucial for revenue management. By analyzing factors like booking patterns, competitor pricing, seasonality, and local events, hotels can develop dynamic pricing strategies to maximize revenue throughout the year.
  
- Digital Marketing Strategy: Having a strong online presence through a user-friendly website, social media engagement, and online travel agency (OTA) listings is vital to attract guests.  Data analytics helps target marketing campaigns to specific guest segments based on demographics, interests, and booking behavior. This leads to more qualified leads and a higher return on marketing investment (ROI).
  
- Competitive Analysis: Understanding competitor offerings and pricing helps hotels position themselves effectively in the market.  Data analysis allows hotels to compare their performance metrics (occupancy rate, average daily rate) with competitors. This helps them identify areas for improvement and develop a competitive advantage.

- Financial Planning and Budgeting: Creating a financial plan that forecasts revenue, expenses, and profitability is crucial. This helps determine pricing strategies and resource allocation. Analyzing historical data on revenue, expenses, and occupancy rates helps create more accurate financial forecasts. This allows for better budgeting and resource allocation across departments.





# Data transformations included:
- Checking data types
- Setting correct headers
- Removing unnecessary columns
- Cleaning of text values




# Data modeling:

- Applied a star schema, as we have two fact tables and three dim tables, established the correct relationships between the tables:

dim_hotels with both fact tables in a 1tomany using property_id column (which is common between the tables)

dim_date with both fact tables in a 1tomany using the date column (from dim_date) and check_in_date column (from both the fact tables)

dim_rooms with both fact tables in a 1tomany using room_id column (from dim_rooms) and room_category (from both fact tables)




# Building metrics using dax:

Your hotel metrics can be influenced by the performance of your employees and it’s helpful to use them to identify areas of improvement. 

- Created new week and day Calculated columns using date/time formulas

- Created 26 measures, varying in complexity and leveraging the various powerful dax formulas




# Example for insights:

- if your occupancy rate is declining, it may be an indication that your marketing team needs to rethink their strategies and campaigns
- Trends by weeks chart is very useful as it hepls the business quickly catch and take action on any interesting trend they find
-  you can identify what type of hotel brings more revenue, and potenitially finding plans to enhance the other types so they can match it
- identify the most preferred booking platforms by users and focus on them     
