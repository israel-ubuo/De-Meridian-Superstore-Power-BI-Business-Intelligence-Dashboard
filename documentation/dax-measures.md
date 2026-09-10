# DAX Measures — De Meridian Superstore Power BI Dashboard

## 1. Overview

DAX (Data Analysis Expressions) was used to create reusable analytical measures for the De Meridian Superstore Power BI Dashboard.

The measures form the calculation layer of the report and are used across KPI cards, charts, trend analysis, customer analysis, product analysis, location analysis, and operational analysis.

## 2. Core Business Measures

### Quantity Sold

Measures the total quantity of products sold.

**Purpose:**

* Monitor sales volume
* Support overall performance analysis
* Compare activity across dimensions

### Total Revenue

Measures the total revenue generated from sales.

**Purpose:**

* Monitor business income
* Compare revenue across customers, products, locations, and periods
* Support revenue trend analysis

### Total Profit

Measures the total profit generated from sales activity.

**Purpose:**

* Evaluate business profitability
* Identify profitable and less-profitable segments
* Support product, customer, location, and operational analysis

### Profit Margin

Measures profitability relative to revenue.

**Purpose:**

* Evaluate the efficiency of revenue generation
* Compare profitability across business dimensions
* Provide a more meaningful profitability indicator than revenue alone

## 3. Location-Based Measures

### Average Profit by Location

Calculates the average profit associated with locations.

**Purpose:**

* Compare geographical profitability
* Identify stronger and weaker locations
* Support regional performance evaluation

### Average Revenue by Location

Calculates average revenue across locations.

**Purpose:**

* Compare revenue performance geographically
* Identify locations with stronger or weaker revenue contribution
* Support location-level decision-making

## 4. Discount Analysis

### Average Discount

Measures the average discount applied across transactions.

**Purpose:**

* Monitor discount behavior
* Compare discount levels across products, locations, and shipping modes
* Investigate relationships between discounting and profitability

Discount analysis is particularly useful when evaluated alongside profit rather than in isolation.

## 5. Shipping & Operational Measures

### Shipping % Revenue

Measures shipping cost relative to revenue.

**Purpose:**

* Assess the proportion of revenue consumed by shipping
* Monitor logistics cost efficiency
* Compare operational cost pressure across shipping dimensions

### Shipping Cost

Shipping cost is used throughout the operational analysis to evaluate logistics performance.

It supports comparisons involving:

* Ship Mode
* Region
* Year
* Revenue
* Profit

## 6. Measure Usage Across Dashboard Pages

| Measure                    | Primary Analytical Use   |
| -------------------------- | ------------------------ |
| Quantity Sold              | Sales volume analysis    |
| Total Revenue              | Revenue performance      |
| Total Profit               | Profitability analysis   |
| Profit Margin              | Profitability efficiency |
| Average Profit by Location | Geographic profitability |
| Avg Revenue by Location    | Geographic revenue       |
| Average Discount           | Discount analysis        |
| Shipping % Revenue         | Shipping efficiency      |

## 7. DAX Design Approach

The dashboard uses measures rather than relying exclusively on manually calculated values within individual visuals.

This approach provides:

* Reusability
* Consistent business logic
* Easier report maintenance
* Dynamic calculations based on filter context
* Consistent KPI reporting

Because Power BI measures respond to the current filter context, the same measure can be evaluated across different customers, products, locations, shipping modes, and time periods.

## 8. Business Logic

The DAX layer connects the underlying data model to business questions.

For example:

**Revenue → Profit → Profit Margin**

allows the analysis to move beyond sales volume and investigate profitability.

Similarly:

**Shipping Cost → Shipping % Revenue → Profit**

allows operational costs to be evaluated alongside financial performance.

## 9. KPI Development

DAX measures were used to power the dashboard's major KPI cards, providing a high-level summary before users move into detailed analysis.

The major KPI areas include:

* Order activity
* Quantity sold
* Revenue
* Profit
* Profit margin
* Shipping cost
* Shipping cost as a percentage of revenue

## 10. Cross-Dimensional Analysis

The measures are designed to work dynamically with the report's dimensions.

This enables questions such as:

* Which customers generate the most profit?
* Which products contribute most to revenue?
* Which locations perform best?
* How does profit vary by ship mode?
* How does shipping cost compare with revenue?
* How does profitability change over time?
* What is the relationship between discounts and profit?

## 11. Conclusion

The DAX layer provides the analytical logic required to transform the underlying Superstore data into meaningful business indicators.

By combining reusable measures with Power BI's filter context, the dashboard supports interactive and multi-dimensional business analysis rather than static reporting.
