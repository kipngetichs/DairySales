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



