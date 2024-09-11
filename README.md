### Store data analysis and report using Excel

Scenerio: 

Create annual report 2022 for the Vrinda store based on the given data. So that, stakeholders can understand their sales data, extract valueable insights and excecute their marketing strategy for year 2023 to get high sale and more profit. 

![image](https://github.com/user-attachments/assets/afad25d8-d3df-415e-9198-fddba8719e6d)


The dataset consists of following columns:

- index: A sequential number indicating the row position in the dataset.
- Order ID: A unique identifier for each order.
- Cust ID: A unique identifier for each customer.
- Gender: The gender of the customer (e.g., Women, Men)
- Age: The age of the customer.
- Date: The date when the order was placed (formatted as DD-MM-YYYY).
- Status: The status of the order (e.g., Delivered).
- Channel: The platform or store where the order was made (e.g., Myntra, Amazon, Ajio, Meesho, Flipkart, Others).
- SKU: The Stock Keeping Unit, a unique identifier for the product.
- Category: The category of the product (e.g., kurta, Set, Top).
- Size: The size of the product (e.g., S, M, L, XL, XXL).
- Qty: The quantity of the product ordered.
- currency: The currency in which the transaction was made (e.g., INR).
- Amount: The total amount for the transaction.
- ship-city: The city where the order was shipped.
- ship-state: The state where the order was shipped.
- ship-postal-code: The postal code of the shipping address.
- ship-country: The country where the order was shipped (e.g., IN for India).
- B2B: A boolean indicator showing whether the transaction was business-to-business (TRUE) or business-to-consumer (FALSE).

#### Sample question
- Compare the sales and orders using single chart
- Which month got the highest sales and order
- Who purchased more- men or Women
- What are different order status
- List top 10 states contributing to the sales
- Relation between age and gender based on number of sale
- Which channel is contributing more sale

### Steps Followed

#### Data cleaning and exploration

1. Very first, I made the heading row freeze,that will allow me to scroll through the spreadsheet with the headings remaining fixed at the top. 
2. I applied filters to the columns to check the columns for their values, blanks, anomalies, etc.
3. In gender column, four values were present: M,Men,W,Women. To make it consistent I replaced M with Men and W with Women.
4. In Quantity column, all values were numerial, along with this at some places "One" and "Two" were present. I changed it to numeric form.
5. Checked the table for duplicates. No duplicates were found.
6. For further calculations, I extracted month names from date column. 
7. Also, I prepared Age-group column to classify the age in three categories Teenager(18-20), Adult(20-30) and Senior(50+). 

#### Analysis and reporting

1. Compare the sales and orders using single chart and Which month got the highest sales and order: I used pivot table to compare the orders and sales month wise. In that, I selected month in row section and sum of amount and count of order ID in values. Once the table is done, I converted it to pivot chart (combination of clustured column and area). 

![image](https://github.com/user-attachments/assets/ffb4dd84-e0d8-4d5e-96bd-04a98183abbc)

#### Observations
#### Monthly Sales Trends:

-  Peak Sales: **March had the highest sales amount at ₹1,928,066**.
- Lowest Sales: October recorded the lowest sales amount at ₹1,666,662.
- Sales Fluctuations: Sales showed a general downward trend from March through November, with some fluctuations. December experienced a slight rebound in sales.

#### Order Volume:

- Highest Orders: **March had the highest number of orders at 2,819** .
- Lowest Orders: October had the lowest number of orders at 2,424.
- Order Count Trends: There was a general decrease in the number of orders from March to November, with a small increase in December.

#### Monthly Performance Variability:

Sales amounts and order counts are somewhat correlated but not perfectly. For instance, while sales were highest in March, the number of orders in March was also the highest. However, in October, despite having one of the lowest sales figures, the drop in order count was more significant compared to other months.

### Suggestions: 
To enhance sales next year, start by analyzing the factors that led to high sales in March and aim to replicate those successful strategies. Launch targeted promotions in months with lower sales to stimulate demand and boost performance. Optimize inventory levels to align with anticipated monthly demand, avoiding stockouts and overstock situations. Implement seasonal pricing strategies and introduce new products during peak months to capture increased interest. Collect and act on customer feedback to improve the shopping experience and encourage repeat purchases. Finally, streamline operational processes to reduce costs and increase efficiency.

2. Who purchased more- men or Women: To find out this, I selected gender in rows and Amount in values of pivot table. 


![image](https://github.com/user-attachments/assets/b3167c3f-8b45-4950-b8b6-3dc8e7d0fece)

#### Observations:
Sales by Gender:

- Women: Sales amount to ₹13,562,773.
- Men: Sales amount to ₹7,613,604.
- Ratio: **Women’s sales are significantly higher, almost double that of men’s.**

- Gender Preference:

The higher sales figure for women suggests a stronger market presence or preference in women’s products.

#### Suggestions

To improve sales next year, focus on expanding and promoting women’s products to maintain strong performance. For men’s products, enhance the range and run targeted promotions to boost sales. Conduct customer research to tailor offerings and improve pricing strategies. Increase visibility and advertising efforts for men’s products to attract more buyers.

3. Different order status

![image](https://github.com/user-attachments/assets/df659191-d14c-4b65-831b-ab955814e82a)


To understand the order status, the pivot table was prepared status vs count of order ID. It is then trasformed to pivot pie chart. 

#### Observations:

Order Status Distribution:

- Delivered: The majority of orders (28,641) were successfully delivered, indicating strong fulfillment performance.
- Cancelled: There were 844 cancelled orders, which is relatively low compared to delivered orders but still noteworthy.
- Returned: There were 1,045 returned orders, indicating some level of post-purchase issues or dissatisfaction.
- Refunded: There were 517 refunded orders, reflecting a moderate number of refunds processed.
Order Issues:

The total number of orders not delivered (cancelled, returned, or refunded) is significantly lower than the delivered orders, suggesting overall effective handling of orders but areas for improvement in customer satisfaction.

4. List top 10 states contributing to the sales

![image](https://github.com/user-attachments/assets/d102c250-cf0f-484d-8dc2-629da3f2fd4c)

The clustered column pivot chart was prepared. 

#### Observations:
- Top Sales Regions: Maharashtra leads with the highest sales amount at ₹2,990,221, followed by Karnataka and Uttar Pradesh.
- Low Sales Regions: Haryana has the lowest sales amount among the listed states at ₹813,320.

#### Suggestions:
- Focus on High Sales Regions: Continue to strengthen marketing and distribution strategies in Maharashtra and Karnataka, where sales are highest.
- Expand in Low Sales Regions: Increase promotional activities and market research in lower-performing states like Haryana to boost sales.
- Tailor Strategies: Develop state-specific strategies based on local preferences and demand patterns to optimize performance across all regions.


5. Relation between age and gender based on number of sale: To find out relationship between age, gender and orders, I selected age group in rows, gender in columns and counter of order ID in values of pivot table. Pivot clustured column is prepared.  

![image](https://github.com/user-attachments/assets/0e9282fb-3156-4849-92a2-a598ca9c6029)


#### Observations:

Gender Distribution by Age:
- Adult: Women make up a larger percentage (52.39%) compared to men (23.29%).
- Senior: Women also have a higher percentage (13.70%) than men (5.91%).
- Teenager: Both men and women have lower percentages, with women (3.33%) slightly higher than men (1.38%).
#### Suggestions:
- Targeted Marketing: Focus on increasing appeal and engagement for men in the adult and senior categories, where they have lower representation.
- Product Development: Develop and promote products tailored to both men and women in their respective dominant age groups to boost sales.
- Promotional Campaigns: Implement targeted campaigns aimed at teenagers and seniors to increase their order volume.

6. Which channel is contributing more sale: the pivot table was prepared with channels vs percentage of sum of amount. Pivot 3D pie was prepared. 


![image](https://github.com/user-attachments/assets/2edbfa5a-a22e-4eb7-a554-9bd92260ad23)


#### Observations:
Top Sales Channels:
- Amazon leads with the highest sales share at 35.51%, followed by Flipkart (21.60%) and Myntra (23.34%).
- Other Channels: Ajio, Meesho, Nalli, and Others have lower sales shares, ranging from 4.10% to 6.29%.

#### Suggestions:
- Leverage Leading Channels: Strengthen partnerships and marketing efforts on Amazon, Flipkart, and Myntra to capitalize on their high sales shares.
- Expand Presence: Increase focus and promotional activities on lower-performing channels like Ajio, Meesho, and Nalli to diversify sales.
- Channel Strategy: Continuously analyze performance across all channels and adjust strategies to maximize overall sales.

Thank you.
