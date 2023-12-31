![Project's Image](images/SQL_portfolio_project.png)

<br>

# PIZZA DATABASE AND DASHBOARD

---
This document contains details about my approach to this project with details from the brief and my approach to creating the dashboard. It also includes my choice of tools and approach to using them!

<br>




## PROJECT BRIEF: Designing a Relational Database for a Pizzeria
---


### Overview:
---
The project involves designing and building a tailor-made bespoke relational database for a new Pizzeria that will allow capturing and storing all important information and data generated by the business. The database will help monitor business performance in dashboards that will be built later. The three main areas of concentration include customer orders, stock levels, and staff.


<br>


### Objectives:
---
- Design and build a relational database for customer orders that will capture and store all important information and data generated by the business.
- Normalize the data, add more related tables, and define table relationships.
- Design and build dashboards to monitor business performance.
- Design and build databases for stock control data and staff data.

<br>


### Scope:
---
The project will cover the following areas:

- **Customer orders:** The database will capture and store item name, item price, quantity, customer name, delivery address, order ID field, delivery address split out into different parts, different sizes of pizzas and beverages as a separate field, and product category.

- **Stock control data:** The database will capture and store information on what ingredients go into each pizza, their quantity based on the size of the pizza, and the existing stock level.

- **Staff data:** The database will capture and store information on which staff members are working when and how much each pizza is actually costing in terms of ingredients, chefs making the pizza, and the cost of delivery based on the time it took to deliver.
   

<br>

   
### Approach:
---
The approach to designing the database involves specifying all fields for the data that need to be collected, normalizing the data, adding more related tables, and defining table relationships. Quick Database Diagrams (Quick DBD) is used as a tool to make the job of designing and building the database easier.


<br>


### Deliverables:
---
1. A tailor-made bespoke relational database for customer orders that captures and stores all important information and data generated by the business.

2. Dashboards to monitor business performance.  
    - __Dashboard 1 - Order Activity__  
    > For this, we will need a dashboard with the following data:  
        - Total Orders \n  
        - Total Sales  \n
        - Total Items  
        - Average Order Value  
        - Sales By Category  
        - Top Selling Items  
        - Orders By Hour  
        - Sales By Hour  
        - Orders By Address  
        - Orders By Delivery/Pick Up

    
    - __Dashboard 2 - Inventory management__  
    > We need to see how much invemtory we're using and then identify inventory that needs reordering. We also want to see how much each pizza costs to make based on the cost of the ingridients so we can keep an eye on pricing and P/L. Here is what we need:  
           - Total Quantity by Ingredients  
           - Total Cost of Ingredients  
           - Calculated Cost of Pizza  
           - Percentage Stock remaining by Ingredient  
           - List of Ingredients To Re-order based on Remaining Inventory

    - __Dashboard 3 - Staff__
    > We want to be able to monitor who was working on any given day or shift and what our overall staff costa are. Here is what we need:
            - Total Staff Costs  
            - Total Hours Worked  
            - Hours Worked by Staff Memeber  
            - Cost per Staff Member
    
3. Databases for stock control data and staff data.

<br>


### Timeline:
---
The project is expected to be completed within 2 weeks.

<br>


### Budget:
---
The budget for the project is $5,000.

<br>


### Assumptions:
---
<ul>
    <li> The front-end ordering system will be built by someone else.</li>
    <li> The project will be completed within the specified timeline and budget.</li>
    <li> No external tools or services will be used to design or build the database.</li>
</ul>


<br>


### Data Dashboard
---
Kindly find the link to the dashboard [here](https://lookerstudio.google.com/embed/reporting/d027f0ed-fd15-4e17-a219-174a3f72c9ea/page/KYHdD)

<br>
<br>


## Project Building
---


### The steps I took
---
1. Build a SQL database
2. Write custom SQL queries
3. Build interactive dashboards

<br>


### Tools
---

1. I also used the Navicat MySQL instance because of its simplicity in creating my database and importing CSV files to populate my tables, in just a few clicks.  
2. I used Quick DBD to create the diagram of the database and the tables.  
3. I also normalized the table to achieve the following:  
   - Reduce redundancy  
   - Improve efficiency
    
<br>


### Main Areas of Focus
---
1. Orders
2. Stock control
3. Staffs
    

> __Orders data Requirement__  
The following are requirements to be achieved with the orders data:  
        1. Item name  
        2. Item price  
        3. Quantity  
        4. Customer name  
        5. Delivery Address
    

> __Stock Control Requirements__  
The following are the requirements to be achieved for stock control:  
        1. I want to be able to know when it's time to order new stock.  
        2. To do this, we're going to need more information about:  
           - What ingredients go into each pizza  
           - Their quantity based on the size of the pizza  
           - The existing stock level  
        3. We'll assume the lead time for delivery by suppliers is the same for all ingredients.

    

> __Statf Data Requirements__  
        1. Want to know which staff members are working when.  
        2. Based on the staff salary information, how much each pizza costs (ingredients + chefs + delivery).

<br>
    


### Creating The Dashboard
---
I used Google Data Studio (Looker Studio) for creating the Dashboard and Report. I changed the columns' data type so that it conforms to the necessary norms like GEO Address for Addresses and Date & Time for date and time columns, etc.

The dashboard focuses on the ten items requested in the brief above. The dashboard was built in two phases:

- **Phase 1:** Queries
- **Phase 2:** Design

<br>
    
### Dashboards To Be Built
---

#### Dashboard 1 - Orders

![Dashboard_pg_1](images/db_pg1.png)

#### Dashboard 2 - Inventory

![Dashboard_pg_2](images/db_pg2.png)

#### Dashboard 3 - Staff

![Dashboard_pg_3](images/db_pg3.png)

 







