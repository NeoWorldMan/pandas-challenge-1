# Wholesale Data Analysis

This Jupyter notebook provides a comprehensive analysis of a wholesale client dataset. The dataset contains information about clients, their orders, and specific items ordered. The analysis aims to uncover insights about the clients, item categories, and overall sales performance.

## Dataset

The dataset used in this analysis is `client_dataset.csv`, which includes the following columns:
- `first`: First name of the client
- `last`: Last name of the client
- `job`: Job title of the client
- `phone`: Phone number of the client
- `email`: Email address of the client
- `client_id`: Unique identifier for the client
- `order_id`: Unique identifier for the order
- `order_date`: Date the order was placed
- `order_week`: Week of the year the order was placed
- `order_year`: Year the order was placed
- `item_id`: Unique identifier for the item
- `category`: Category of the item
- `subcategory`: Subcategory of the item
- `unit_price`: Unit price of the item
- `unit_cost`: Unit cost of the item
- `unit_weight`: Unit weight of the item
- `qty`: Quantity of items ordered
- `line_number`: Line number in the order

## Analysis Steps

1. **View the column names in the data**
   - Displayed the column names to understand the structure of the dataset.

2. **Basic statistics**
   - Used the `describe` function to gather basic statistics about the dataset.

3. **Familiarize with the data**
   - Explored the dataset using the `info` method to understand data types and missing values.

4. **Top item categories**
   - Identified the three item categories with the most entries.

5. **Top subcategory**
   - Determined the subcategory with the most entries for the top item category.

6. **Top clients**
   - Found the five clients with the most entries in the dataset.

7. **Top clients list**
   - Stored the client IDs of the top 5 clients in a list.

8. **Total units ordered by top client**
   - Calculated the total units ordered by the client with the most entries.

9. **Subtotal column**
   - Created a column to calculate the subtotal for each line using `unit_price` and `qty`.

10. **Shipping price column**
    - Created a column for the shipping price based on the weight of the items.

11. **Total price column**
    - Created a column for the total price using the subtotal, shipping price, and sales tax.

12. **Line cost column**
    - Created a column for the cost of each line using `unit_cost`, `qty`, and `shipping_price`.

13. **Profit column**
    - Created a column for the profit of each line using the line cost and total price.

14. **Total calculations**
    - Checked the work by summing up the totals for three orders.

15. **Top clients spend**
    - Calculated the total spend for each of the top 5 clients. 

16. **Summary DataFrame**
    - Created a summary DataFrame for the top 5 clients showing for each total units purchased, total shipping price, total revenue, total cost, and profit.

17. **Format and rename columns**
    - Formatted the data and renamed columns to names suitable for presentation.

18. **Sort data by profit**
    - Sorted the data by total profit from highest to lowest and assigned the sort to a new DataFrame.

## How to Run the Notebook

1. Ensure you have Python installed along with the necessary libraries: `pandas` and `nbformat`.
2. Download the `client_dataset.csv` and place it in the `Resources` directory.
3. Open the notebook using Jupyter Notebook or JupyterLab.
4. Run each cell in the notebook to perform the analysis step by step.

## Conclusion

This notebook provides a detailed analysis of the wholesale client dataset, uncovering valuable insights about client behavior, item categories, and sales performance. The analysis can be further extended to include more complex operations and visualizations to gain deeper insights.

## Summary of Findings

The analysis revealed that the top three item categories with the most entries were "consumables," "furniture," and "software," with "bathroom supplies" being the leading subcategory in "consumables." Additionally, the top five clients contributed significantly to total sales, with one client ordering the a significantly higher quantity of units, leading to substantial revenues and profits.
