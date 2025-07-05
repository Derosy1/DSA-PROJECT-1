# DSA-PROJECT-1
# My excel project with DSA Incubator in Data Analysis
# Project Overview:Amazon Product Review Analysis
As a Junior Data Analyst at RetailTech Insights, I conducted a comprehensive analysis of Amazon product and customer review data to extract actionable insights that support product improvement, marketing strategies, and customer engagement. The dataset comprised 1,465 Amazon products, including details such as product category, price, discount, ratings, and aggregated customer reviews.

Using Excel tools such as pivot tables, calculated columns, and data visualizations, I explored key performance metrics across product categories. The analysis focused on uncovering trends in discounting, rating distributions, review volumes, and pricing strategies. Key objectives included identifying high-performing products, understanding rating-review dynamics, and estimating potential revenue contributions.

The project culminated in the creation of an interactive Excel dashboard, providing stakeholders with a clear and actionable view of product performance metrics, category-level insights, and customer engagement trends.
# Data Source
The dataset was sourced through web scraping of Amazon product pages, collecting publicly available information including product details (name, category, price, discount, and ratings) and customer engagement data (review counts, titles, and content). Each record represents a unique product with aggregated reviewer data stored in structured format.
# Tool Used
Ms Excel for data cleaning and pivot table for the data analysis [Download here](https://www.microsoft.com/en-us/microsoft-365/excel?msockid=3051be019ec16d900feaab689f5f6c24)
  * For data colection
  * For data cleaning
  * For data wrangling
  * For data manipulation
  * For data analysis
  * For datat sumerization
  * For data calculation
  * For data visualization
# Data Cleaning/preparation
* I loaded the data
* Checked for missing values
* Check for duplicate rows to ensure each product entry was unique
* I reviewed all 16 columns for missing data
* Data cleaning and formatting
* I changed data type by converting text-formatted numbers (e.g., price, discount, rating count) to proper numeric data
* I splitted product name by reducing the text and deleted other text to make it look more consized
* I deleted the uneccessary columns like about product, user ID, user name, review title, product link, img link,review content
* I applied ctl A to format adn fit text to width
# Exploratory Data Analysis
## Using Pivot Table
Pivot tables were essential for efficiently summarizing and analyzing the Amazon product dataset. They allowed for dynamic grouping, aggregation, and comparison of key metrics across product categories, price ranges, and review counts. Specifically, pivot tables were used to:
1. What is the average discount percentage by product category?

   (Using pivot table: Insert, click pivot table, select from table/range, new sheet, ok. Drag category to row and discount to value on pivot table dialoque box. Edit column names)
2. How many products are listed under each category?
  
   (Using pivot table: Insert, click pivot table, select from table/range, new sheet, ok. Drag category to row and product name to value on pivot table dialoque box. Edit column names)

 3. What is the total number of reviews per category?

 (Using pivot table: Insert, click pivot table, select from table/range, new sheet, ok. Drag category to row and review ID to value on pivot table dialoque box. Edit column names: right click on design, report layout, show in outline form)
   
4. Which products have the highest average ratings?

 (Using pivot table: Insert, click pivot table, select from table/range, new sheet, ok. Drag product name to row and rating to value on pivot table dialoque box, Then sort by decending order to get the highest rating, change value to average. Edit column names)
   
5. What is the average actual price vs the discounted price by category?

   (Using pivot table: Insert, click pivot table, select from table/range, new sheet, ok. Drag category to row,  Actual price and discount percentage to value on pivot table dialoque box, change value to average. Edit column names)
   
6. Which products have the highest number of reviews?

(Using pivot table: Insert, click pivot table, select from table/range, new sheet, ok. Drag product name to row and review ID to value on pivot table dialoque box, Then sort by highest order to get the product with the highest number of reviews, change value to average. Edit column names)
   
7. How many products have a discount of 50% or more?

   (Using pivot table: Insert, click pivot table, select from table/range, new sheet, ok. Drag product name to row and discount percentage to value on pivot table dialoque box, = countIF (select range, ">=50%) Edit column names)


8. What is the distribution of product ratings (e.g., how many products are rated 3.0, 4.0, etc.)?

 (Using pivot table: Insert, click pivot table, select from table/range, new sheet, ok. Drag rating to row and count of rating to value on pivot table dialoque box, = countIF(highlight rate, ">=3.0"), click rating, filter with values greater than or equal to input 3, ok)

 
9. What is the total potential revenue (actual_price × rating_count) by category?

   Create helper column = Potential Revenue (Actual price x rating count), set to number, removel decimal, category to row adn potential revenue to value.
   
10. What is the number of unique products per price range bucket (e.g., <₹200, ₹200–₹500, >₹500)?

    Create a column for price bucket
    = IF (D2 > 200, "<200", IF (D2<=500, "200-500", ">500"))
    Drage bucket to row and product name to value

    
11. How does the rating relate to the level of discount?

    Highlight both columns discount percentaeg and rating, insert scater plot, to view relationship, format where necessary
    
12. How many products have fewer than 1,000 reviews?

   
13. Which categories have products with the highest discounts?

  (Using pivot table: Insert, click pivot table, select from table/range, new sheet, ok. Drag category to row and count of product name to value on pivot table dialoque box, sort highest count of product name by category. Edit column names)
    
14. Identify the top 5 products in terms of rating and number of reviews combined.

(Using pivot table: Insert, click pivot table, select from table/range, new sheet, ok. Drag product name to row, count of review ID and sum of rating to value on pivot table dialoque box. Edit column names)

# Analysis


![Scater plot](https://github.com/user-attachments/assets/a8f62519-fd2d-400e-a40c-1464ced3c738)![Excel Dashboard](https://github.com/user-attachments/assets/50bc2814-fcd1-48a7-bb95-21eb5c3bcb0a)


