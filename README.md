# Assignment 4
Power BI Assignment 1 Data Transformation and Modelling
@ -0,0 +1,48 @@
E-Commerce Sales Analysis - Power BI Assignment

This project explores e-commerce sales data analysis using Power BI, following a structured workflow from data importation and transformation to modeling and aggregation.
 Dataset Files:-

 * List of Orders.csv
 * Order Details.csv
 * Sales Target.csv

 Project Workflow & Steps:-

1. Import Data
 * Imported "List of Orders", "Order Details", and "Sales Target" into Power BI and opened them in Power Query Editor.

2. Data Transformation
 * Row Restriction: Restricted the "List of Orders" table to the first 500 rows.
 * Data Type Formatting:
   * Ensured the "Order Date" column is set to the Date data type.
   * Changed the data type of "Amount" and "Target" columns to Fixed Decimal Number.
 * Text Formatting: Formatted the "CustomerName" column into proper case for consistent capitalization.
 * Column Merging: Merged the "State" and "City" columns to create a new column named "Location" in the format City, State.
 * Custom Columns:
   * Created a custom column "Profit Margin" calculated as the percentage of Profit divided by Amount.
   * Added a conditional column "Profit Status" based on the Profit column values:

     * Loss if profit < 0
     * Break-Even if profit = 0
     * Profit if profit > 0

3. Merging Data 
 * Merged the "List of Orders" and "Order Details" tables into a single table named "Orders Data" based on the Order ID relationship.

4. Handling Missing & Duplicate Data
 * Identified and addressed missing values within the dataset.
 * Checked for duplicate rows and cleaned them to ensure data integrity.

5. Sorting and Filtering Data
 * Sorted the Order Date in descending order within the "Orders Data" table to analyze recent trends.
 * Applied filters on the State column (e.g., Tamil Nadu) to conduct targeted regional analysis.

6. Grouping and Aggregating Data
 * Grouped the "Order Details" table to calculate the count of each Order ID, average profit by Category, and total amount by Sub-Category.
 * Aggregated the "Sales Target" table to get the total target amount by the Month of Order Date.

7. Data Modeling & Relationships
 * Established a relationship between "List of Orders" and "Order Details" tables using the Order ID column.
 * Built an active relationship between "Order Details" and "Sales Target" tables using the Category column.
