# Innomatics-Research-Labs-hackathon-
Hackathon Task: Restaurant Orders Analysis
Overview

This project analyzes transactional and master data from a restaurant ordering system. The goal is to gain insights into user behavior, restaurant performance, and city-wise revenue patterns.

The datasets include:

orders.csv – Transactional data of orders placed.

users.json – User master data, including membership details.

restaurants.sql – Restaurant master data, including cuisine and ratings.

The analysis involves merging these datasets, performing aggregation, and generating insights such as top restaurants, high-value users, and city-wise revenue.

Objectives

Identify restaurants with the highest average order values.

Calculate total orders and revenue by membership type and city.

Analyze restaurant performance based on ratings and cuisine.

Determine distinct users, repeat orders, and Gold member activity.

Provide insights useful for business strategy and marketing.

Steps Performed

Data Loading:

Loaded orders.csv and users.json into Pandas DataFrames.

Loaded restaurants.sql data into a DataFrame.

Data Cleaning:

Ensured numeric columns (total_amount) were properly typed.

Checked for missing values and handled accordingly.

Data Merging:

Joined orders.csv with users.json on user_id.

Joined the result with restaurant details on restaurant_id.

Analysis Performed:

Calculated average order value and total orders per restaurant.

Filtered restaurants with low order counts (<20).

Computed total orders and revenue for Gold members.

Determined city-wise revenue and top-performing cities.

Counted distinct users and high-rated restaurant orders.

Insights Extracted:

Restaurants with the highest average order value.

Total orders and revenue by membership type.

Orders for top-rated restaurants.

City-wise revenue contributions from Gold members.

Key Columns Used
Column	Description
order_id	Unique identifier for each order
user_id	Unique identifier for each user
restaurant_id	Unique identifier for each restaurant
membership	User membership type (e.g., Gold, Silver)
total_amount	Order value
restaurant_name_x	Name of the restaurant
cuisine	Type of food served
rating	Restaurant rating
city	City where the order was placed
Tools Used

Python 3

Pandas – For data cleaning, merging, and analysis

SQL – To extract restaurant master data

Jupyter Notebook – For interactive analysis

Deliverables

analysis_output.csv – Final merged and processed dataset.

insights_task.txt – Key insights from the analysis.

Jupyter Notebook with all code and visualizations.

Conclusion

This analysis provides actionable insights for restaurant performance, user behavior, and city-level revenue trends. It highlights top restaurants, high-value users, and membership-based ordering patterns, which can guide marketing and operational strategies.
