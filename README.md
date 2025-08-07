# Factory Performance and Shipping Efficiency Dashboard

This project presents an interactive Tableau dashboard to explore shipping efficiency and sales performance across candy factories in the U.S. Using a combination of sales, product, and factory location data, the dashboard helps identify bottlenecks, high-performing products, and strategic opportunities for expansion.

## Objectives
- Analyze factory performance and fulfillment efficiency
- Identify regional imbalances in sales and shipping
- Provide actionable recommendations for logistics and planning

## Key Visualizations
- **Maps**: Show geographic distribution of factories and customers
- **Pareto Chart**: Highlight top-selling candy products
- **Scatter Plot**: Reveal the relationship between shipping distance and sales variability
- **Histograms**: Show distributions of order frequency and shipping distances
- **Pie Chart**: Visualize regional sales contribution
- **Heatmap**: Show state-wise sales intensity and factory utilization

## Technical Features
- **Calculated Fields**:
  - `Shipping Distance (Miles)` (based on lat/long)
  - `Sales Variability` (STDEV of monthly sales)
  - `Running % of Total` and `Running Sales` for Pareto
  - `Region Highlight` for dynamic region emphasis

- **Parameters**:
  - `Select Region` — dynamically highlights a selected region in charts without filtering

- **Dashboard Actions**:
  - Map-to-Heatmap filter action
  - Highlight actions across views
  - Region parameter control in pie chart

## Dataset Sources
- `Candy_Sales.csv`: Order-level sales records
- `Candy_Factories.csv`: Factory locations
- `Candy_Products.csv`: Product metadata
- `uszips.csv`: Geographic lookup (zipcode → coordinates)

## Insights & Recommendations
- **Optimize shipping**: Factories like "Lot’s O’ Nuts" have inefficient fulfillment routes
- **Rebalance workloads**: Some factories are underutilized in certain regions
- **Targeted growth**: Use heatmap to identify low-penetration states
- **Sales stability**: Identify inconsistent products using variability plots
