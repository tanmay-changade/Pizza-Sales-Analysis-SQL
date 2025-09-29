# Pizza Sales Data Analysis🧑‍💻: Comprehensive Performance Metrics and Customer Insights
<h2>Link🔗:</h2>
<a href="https://www.canva.com/design/DAGo1ApRWxc/0AiXL_H685R6pZXhCDEOGQ/view?utm_content=DAGo1ApRWxc&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h2034768c7f">Please Click Here to see queries and output</a>
<h2>Objective & Scope :</h2>
<b>
☑️Objective: The primary objective of this project is to use SQL (Structured Query Language) to analyze a relational database of pizza sales data.<br>
The analysis will cover key business metrics, product performance, and temporal trends to provide actionable insights for optimizing inventory, pricing, and promotional strategies.<br>
☑️Scope: The project addresses 12 distinct analytical questions, organized into three tiers of complexity: Basic, Intermediate, and Advanced.<br>
It requires joining four core tables: orders, order_details, pizzas, and pizza_types.<br>
</b>
<h2>Key Analytical Areas📊:</h2>
<b>
1. Sales & Revenue Tracking<br>
2. Product Performance<br>
3. Temporal Analysis<br>
4. Contribution & Segmentation<br>
</b>
<h2>Schema📁:</h2>
<img alt="file structure" src="https://github.com/tanmay-changade/Pizza-Sales-Analysis-SQL/blob/main/File%20Structure.png"/><br>
<b>order_details </b>Table: This file contains information about the individual pizzas within each order.<br>
<b><i>order_details_id:</i></b>	A unique identifier for each specific pizza item in an order.<br>
<b><i>order_id:</i></b>	The ID that links the pizza item to the overall customer order (connects to orders table).<br>
<b><i>pizza_id:</i></b>	The ID specifying the type and size of the pizza (e.g., hawaiian_m for Hawaiian Medium).<br>
<b><i>quantity:</i></b>	The number of pizzas of that exact type and size included in the order.<br>
<br>
<b>orders</b> Table: This file contains the high-level details for every customer order.<br>
<b><i>order_id:</i></b>	A unique identifier for the customer order (connects to order_details table).<br>
<b><i>date:</i></b>	The date the order was placed.<br>
<b><i>time:</i></b>	The time the order was placed.<br>
<br>
<b>pizza_types</b> Table: This file provides descriptive information for each unique pizza recipe.<br>
<b><i>pizza_type_id:</i></b>	A unique identifier for the type of pizza (e.g., bbq_ckn). This is used to link to pizzas table<br>
<b><i>name:</i></b>	The full, descriptive name of the pizza (e.g., 'The Barbecue Chicken Pizza').<br>
<b><i>category:</i></b>	The general category the pizza belongs to (e.g., 'Chicken', 'Classic', 'Veggie', 'Supreme').<br>
<b><i>ingredients:</i></b>	A text string listing all the ingredients used on that pizza type.<br>
<br>
<b>pizzas</b> Table: This file lists the available sizes and prices for every pizza type.<br>
<b><i>pizza_id:</i></b>	A unique identifier combining the pizza type and its size (e.g., bbq_ckn_s). This connects to order_details table.<br>
<b><i>pizza_type_id:</i></b>	The ID for the type of pizza (connects to pizza_types table).<br>
<b><i>size:</i></b>	The size of the pizza, typically 'S', 'M', 'L', and sometimes 'XL' or 'XXL'.<br>
<b><i>price:</i></b>	The price of the pizza for that specific size.<br>

<h2>Outcomes and Business Insights 🏆:</h2>
<b>1. Basic Metrics & High-Level Performance:</b><br>
<b>Total Orders & Revenue :</b> Quantifies the overall business volume and financial performance.<br>
<b>Highest-Priced Pizza :</b> Provides context for pricing strategy and premium product analysis.<br>
<b>Most Common Size :</b> Crucial for inventory management and production planning.<br>
<b>Top 5 Pizza Types :</b> Highlights the core product offerings driving sales volume.<br>
<br>
<b>2. Intermediate Analysis: Categorization and Trends:</b><br>
<b>Category Quantity : </b>Reveals which pizza categories are most popular, informing menu and promotional focus.<br>
<b>Order Distribution by Hour : </b>Identifies peak operational hours to better schedule staff and kitchen capacity.<br>
<b>Category-Wise Distribution : </b>Provides an understanding of product diversification across categories.<br>
<b>Average Pizzas Per Day : </b>Establishes a baseline for daily performance and forecasting.<br>
<b>Top 3 by Revenue : </b>Identifies the most financially valuable products, which may differ from the highest-volume products.<br>
<br>
<b>3. Advanced Analysis: Deep Segmentation and Time-Series:</b><br>
<b>Percentage Contribution : </b>Essential for Pareto analysis (80/20 rule) and strategic menu pruning or focus.<br>
<b>Cumulative Revenue : </b>Visualizes the growth trajectory and identifies periods of accelerated or slowed sales.<br>
<b>Top 3 by Revenue (Per Category) : </b>Allows for targeted marketing and promotions based on high-value products within a specific menu segment.<br>
