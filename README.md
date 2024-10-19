# Sales Analysis of Dairy Products Across Various Locations in India
# Situation
The dairy sales analysis focuses on examining the performance of various dairy products across multiple locations in India, with a particular emphasis on inventory management, revenue generation, and sales trends. The dataset includes detailed information on product names, brands, sales channels, locations, shelf life, and storage conditions, providing a comprehensive overview of how different factors affect dairy product sales. The goal of the analysis is to identify key business insights, such as high-demand regions, top-performing brands, and potential risks of overstocking or stockouts, particularly with perishable products that have a short shelf life. This analysis helps address critical business challenges, such as optimizing inventory, aligning supply with regional demand, and maximizing profitability across different sales channels.
# Business Challenges to Address in This Project:
1.  How can we balance stock levels to minimize wastage from overstocking and prevent missed sales opportunities due to stockouts? Efficient inventory management is essential to meet customer demand while avoiding product expiration.
2.   How can we effectively manage dairy products with short shelf lives, ensuring they are sold before spoilage occurs? This challenge focuses on maintaining freshness and reducing losses from unsold perishable items.
3.   With different sales channels (retail, wholesale, and online) performing variably, how can we optimize product distribution and marketing strategies for each channel to maximize revenue?
4.   Given that demand for dairy products varies across different locations, how can we tailor our inventory supply and distribution strategies to align with regional demand patterns and improve overall sales efficiency?
# Task
As a skilled problem solver and critical thinker, my approach to the task involves thoroughly analyzing dairy sales data to identify and address key business challenges. I  assessed inventory levels to strike a balance between overstocking and stockouts, ensuring efficient management of perishable products to minimize spoilage. By examining sales performance across various channels, I  seeked to optimize marketing and distribution strategies tailored to each channel's effectiveness. Additionally, I  investigated regional demand variations to align supply with specific market needs, ultimately providing actionable insights that enhance profitability and operational efficiency in the dairy industry.
# Action
In executing the project, I utilized Power BI, Excel, and SQL to conduct a comprehensive analysis of the dairy sales data. I began by querying the dataset with SQL to extract relevant information, including sales figures, inventory levels, and product details. Next, I employed Excel for data cleaning and preliminary calculations, ensuring accuracy in the analysis. I then created interactive dashboards in Power BI to visualize key metrics such as sales performance by region, inventory turnover rates, and trends in perishable product sales. This integrated approach allowed me to identify critical insights, such as optimal stock levels and peak sales periods, which directly address the business challenges faced by the dairy industry.
- Here is the SQL query for products that have expired:

       SELECT 
   
        Product_Name, 

       DATEDIFF(DAY, GETDATE(), Expiration_Date) AS Days_Past_Expiration
      FROM 
      dairyproducts
      WHERE 
       Expiration_Date <= GETDATE();
- Results

![Sql exp products](https://github.com/user-attachments/assets/50ae34a9-ff8d-4f57-b73d-5554a6a83bad)
- A preview of the Power BI dashboard is available below:

![dairy dash](https://github.com/user-attachments/assets/776148ea-18db-4e57-a0f3-6ea9739b59a6)
# Result
- Here is the descriptive analysis of what happened in dairy sales
  - Top Brands: Amul and Mother Dairy dominate the market, generating the highest revenue.
  - High-Demand Locations: Chandigarh and Delhi have the highest demand for dairy products, indicating regional preferences.
  - Sales Channel Performance: Retail and wholesale channels dominate sales across most product categories. However, online sales outperform for Lassi.
  - Seasonal Trends: Sales peak in January, June, September, and December. A significant decline occurs from February to April, while sales fluctuate in other months.
  - Revenue by Storage Condition: Refrigerated products account for ₹34M in revenue, the highest among all storage conditions, followed by frozen products at ₹14M.
  - Weekday Sales Trends: Sales are stable across all weekdays, with Thursdays showing the highest peaks.
  - Perishable Products at Risk: Dairy products with a shelf life of 15 days or less, such as Lassi, Milk, Paneer, Buttermilk, and Curd, are at risk of spoiling if not sold quickly.

# Recommendations
 Solutions to Address Business Challenges Based on Descriptive Analysis
1. Implement a dynamic inventory management system that uses historical sales data to forecast demand more accurately, reducing the likelihood of overstocking and stockouts. For instance, leveraging the peak sales months identified (January, June, September, and December) can help adjust inventory levels in anticipation of higher demand. Seasonal promotions during these months could further optimize stock levels.
2. Establish a first-in, first-out (FIFO) inventory system for dairy products with short shelf lives, ensuring that older stock is sold first to minimize spoilage. Regular training for staff on inventory management practices can reinforce the importance of monitoring expiration dates. Additionally, consider implementing discount strategies for products approaching their expiration dates to encourage quick sales.
3. Tailor marketing strategies for each sales channel based on their performance. For example, since retail and wholesale dominate sales, strengthen partnerships with these channels through promotional campaigns. For Lassi, which performs well online, consider investing in targeted online advertising and social media campaigns to drive sales further. Regularly analyzing channel performance will allow for timely adjustments to marketing strategies
4. Conduct regular market research to understand the preferences of customers in high-demand locations like Chandigarh and Delhi. This information can help adjust inventory supply and distribution strategies, ensuring that popular products are readily available in these regions. Collaborating with local distributors can enhance supply chain efficiency and meet regional demand fluctuations effectively.
# Reflection

Reflecting on this dairy sales analysis project, I have gained invaluable insights into the complexities of inventory management and the dynamics of consumer behavior in the dairy market. The process of analyzing historical sales data not only enhanced my problem-solving skills but also deepened my understanding of how various factors, such as regional demand, sales channels, and product shelf life, influence overall performance. Through this project, I learned the importance of leveraging data-driven strategies to address business challenges effectively, such as balancing stock levels and optimizing marketing efforts across different channels. This experience has not only equipped me with practical analytical skills but also reinforced my commitment to continuous learning and adaptation in the ever-evolving landscape of data analytics
