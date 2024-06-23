# POWER_BI_INVENTORY_CONTROL
Utilize Power BI to calculate, modeling, build and visualize dashboard
## I. Introduction
### 1. Business question
A production department is a collection of roles within a company that is in charge of producing products. This can range from a small department that converts raw materials, assembles components into finished products, and packages them to a fully functional department that converts raw materials, assembles components into finished goods, and packages them.

AdventureWorks is a business that has a production department which has lots of components in inventory which are placed in different countries, states,... AdventureWorks mainly produced bicycles which are friendly to the environment.
The process starts with a production request, which is usually initiated by another process, such as delivery, which must complete a customer order (make-to-order strategy), or material preparation, which has decided that the company needs to raise inventory levels (make-to-stock strategy). The production department identified the following requirements want Data team support:

Inventory controlling: Help users review the inventory status of each category of product in a quicker and more convenient way. Support quantity control so that Sales Department could be informed about the current stock of each product and know which product is going to be out of stock. It helps users start doing marketing strategies for products and schedule production and business operations to maximize sales and profit.
### 2. Dataset
Dataset: **adventureworks2019** (public Google BigQuery dataset)

Dataset dictionary: Please reach file "Data Dictionary" attached above

Dataset Schema: https://i0.wp.com/improveandrepeat.com/wp-content/uploads/2018/12/AdvWorksOLTPSchemaVisio.png?ssl=1

Dataset access: 
- Log in to your Google Cloud Platform account and create a new project.
- Navigate to the BigQuery console and select your newly created project.
- In the navigation panel, select "Add Data" and then "Star a project by name".
- Enter the project name "adventurework2019"

## II. Apply design thinking mindset
**1. Empathize**

![image](https://github.com/anhailee/Image/assets/150501087/a9ccbf69-9ba8-41b0-ae0b-d64829920d75)

**2. Define point of view**

![image](https://github.com/anhailee/Image/assets/150501087/8860a11c-251b-4f00-a074-c7536d231d80)

**3. Ideate**

![image](https://github.com/anhailee/Image/assets/150501087/3875e673-ffc0-4d5e-ab6b-97774d8e3bfb)

**4&5. Prototype and review**

![image](https://github.com/anhailee/Image/assets/150501087/0c633120-de97-4562-beb5-5b4e3136e46f)

## III. Dashboard

**1. Inventory Overview Dasboard**

![image](https://github.com/anhailee/Image/assets/150501087/d9a581f2-b174-4c0a-8aa5-0ee83726a163)

**2. Storage Dasboard**

![image](https://github.com/anhailee/Image/assets/150501087/1c9432dc-52bb-4275-88c1-9f4265dbdecd)

**3. Product Detail Information Dasboard**

![image](https://github.com/anhailee/Image/assets/150501087/1781f8bf-6438-4a42-b0b9-1f637f796668)

## IV. Insights

**1. Inventory items:**

Inventory levels remained quite stable from 2011 to 2013 (with some increase, but not significant). However, there was a sharp increase in 2014, specifically about a 270% increase compared to 2013. The "Others" category was the main reason for this sudden change.

**2. Inventory Status:**

In warehouse management, there is a concept known as the minimum inventory level. The number of items not meeting the minimum inventory level standards increased nearly 20-fold in mid-2014 compared to 2013.

The "Others" category accounted for the majority of items not meeting the minimum inventory level requirements. Specifically, there were up to 55 types of items, making up 25% of the inventory in 2014.

**3. Revenue and Costs:**

**Costs:**
- **2013:** Inventory levels were low, but costs were high because the items belonged to the "Components" and "Bikes" categories (the two categories with the highest average production costs).
- **2014:** Although inventory levels were high, they mainly consisted of items from the "Others" category (the category with the lowest average production costs).

=> The discrepancy in average production costs led to an inverse correlation between inventory levels and total costs.

**Revenue:**
- Over time, revenue has always been higher than costs.
- However, a deeper analysis of the correlation between revenue, costs, and categories reveals a critical point: the "Components" category has lower revenue compared to costs. (Previous slides have shown that "Components" is the category with the highest average production costs).

## V. Recommendations

**1. On Inventory items and inventory status:** 

Firstly, it's crucial to categorize the "Others" category in more detail. Avoiding lumping them together will facilitate better management and the formulation of suitable sales programs. Here are some classification criteria:

+ Product-based classification: Based on the type of product or service they represent.
+ Value-based classification: Based on the price level of the product.
+ Origin or production time-based classification.
+ Classification based on condition, size, weight, etc.

Secondly, regular monitoring of inventory data in the system and organizing frequent physical inventories is necessary to:

+ Limit discrepancies between inventory records and actual stock to prevent losses and control minimum inventory levels for each item.
+ Minimize inventory damage during storage, promptly identify unintended incidents affecting inventory quality, and forecast shortages based on estimated actual production times to replenish deficient stock on time.

**2. On Revenue and costs:**

Several methods to reduce costs and optimize revenue for inventory:

+ Optimize inventory levels: Besides checking if inventory levels meet minimum requirements, pay attention to items significantly exceeding minimum levels. Excessive stock incurs unnecessary storage costs, similar to the case of the "Others" category.
  
+ Prioritize selling older inventory: For categories like "Others" with excessive inventory, ensure that older stock is sold first to minimize depreciation over time.
  
+ Addressing high costs of "Components": Continuously seek potential suppliers to negotiate prices proactively with current suppliers or switch suppliers as needed.

+ Research competitive alternatives: Explore other manufacturers who can supply components for the "Components" category. Compare prices and quality from competitors to find the best solution for cost minimization.
  
+ Cost-value analysis: For the "Components" category, evaluate whether all components are essential. Eliminate or replace less essential components to reduce overall costs.

+ Promotional strategies: Implement promotional campaigns such as bundling high-price items from the "Others" category with additional products or offering buy-two-get-one-free deals or discounts.

+ Reuse and recycle: Consider ways to reuse or recycle parts of inventory to save money on purchasing new raw materials.
