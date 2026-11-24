# Experiment 1.B : Product Price Analysis Using Python Functions

## Aim
To analyze quarterly product sales data across multiple products and quarters using 2D NumPy arrays and Python statistical functions.

## Algorithm

1. **Start** the program.
2. **Import Library**: Import the `numpy` module as `np` for numerical array operations.
3. **Initialize 2D Sales Matrix**: Create a $3 \times 4$ NumPy array `sales` containing quarterly sales figures for 3 products across 4 quarters.
4. **Compute Product-Wise Totals**: Calculate the sum of sales across columns (`axis=1`) for each product using `np.sum(sales, axis=1)`.
5. **Compute Quarter-Wise Totals**: Calculate the sum of sales across rows (`axis=0`) for each quarter using `np.sum(sales, axis=0)`.
6. **Compute Overall Statistical Metrics**:
   * Calculate the overall mean sales across all entries using `np.mean(sales)`.
   * Identify the maximum sales figure using `np.max(sales)`.
   * Identify the minimum sales figure using `np.min(sales)`.
7. **Display Analysis Summary**: Print the original sales matrix, product-wise totals, quarter-wise totals, overall average, highest sale, and lowest sale.
8. **Stop** the program.
## Program

# Step 1: Create 2D array (Rows = Products, Columns = Quarters)
<<Enter your code>>

import numpy as np  

# Create 2D sales array (3 Products × 4 Quarters)  
sales = np.array([
    [120, 150, 170, 200],
    [90, 110, 130, 160],
    [150, 140, 180, 210]
])

print("Quarterly Sales Data:")  
print(sales)  

# Step 2: Calculate Aggregations and Summary Statistics
<<Enter your code>>


# Calculate product-wise totals
product_totals = np.sum(sales, axis=1)  

# Calculate quarter-wise totals
quarter_totals = np.sum(sales, axis=0)  

# Calculate overall statistics
average_sales = np.mean(sales)  
highest_sales = np.max(sales)  
lowest_sales = np.min(sales)  

# Step 3: Display Summary
<<Enter your code>>


print("\nProduct-wise Sales Totals:")  
print(product_totals)  

print("\nQuarter-wise Sales Totals:")  
print(quarter_totals)  

print("\nOverall Average Sales:", average_sales)  
print("Highest Sales:", highest_sales)  
print("Lowest Sales:", lowest_sales)  

## Output


Quarterly Sales Data:
[[120 150 170 200]  
 [ 90 110 130 160]  
 [150 140 180 210]]  

Product-wise Sales Totals:
[640 490 680]  

Quarter-wise Sales Totals:
[360 400 480 570]  

Overall Average Sales: 150.83333333333334  
Highest Sales: 210  
Lowest Sales: 90  

## Result

The program successfully analyzes quarterly product sales using 2D NumPy arrays and Python statistical aggregation functions.
