# Data Model — De Meridian Superstore Power BI Dashboard

## 1. Overview

The De Meridian Superstore Dashboard uses a structured analytical data model designed to support business performance analysis across customers, products, locations, orders, shipping, and time.

The model provides the foundation for the dashboard's KPI calculations, interactive filtering, trend analysis, and cross-dimensional business analysis.

## 2. Analytical Areas

The data model supports analysis across the following major dimensions:

* **Orders** — transactional and order-level information
* **Customers** — customer names and customer segments
* **Products** — product-level performance
* **Locations** — geographical information including region and state/province
* **Shipping** — shipping events, shipping cost, and ship modes
* **Calendar** — time-based analysis

## 3. Key Fields Used in Analysis

Important fields referenced throughout the dashboard include:

| Area      | Fields / Attributes                    |
| --------- | -------------------------------------- |
| Orders    | Row ID, Quantity Sold, Revenue, Profit |
| Customers | Customer Name, Customer Segment        |
| Locations | Region, State or Province              |
| Shipping  | Shipping Cost, Ship Mode               |
| Calendar  | Year, Quarter                          |
| Products  | Product-level attributes               |

## 4. Measures

The dashboard uses DAX measures to create reusable business calculations.

Key measures include:

* **Quantity Sold**
* **Total Revenue**
* **Total Profit**
* **Profit Margin**
* **Average Profit by Location**
* **Avg Revenue by Location**
* **Average Discount**
* **Shipping % Revenue**

These measures are used across KPI cards, charts, comparisons, and operational analyses.

## 5. Time Intelligence

The dashboard includes a dedicated **Calendar** table to support time-based analysis.

Time-based visualizations allow performance to be evaluated across periods such as:

* Year
* Quarter
* Time trends

This supports analysis of revenue, profit, shipping cost, and other business indicators over time.

## 6. Model Design Approach

The data model was designed to support:

* Interactive filtering
* Cross-dimensional analysis
* Reusable DAX measures
* KPI reporting
* Time-based analysis
* Customer and product analysis
* Geographical analysis
* Operational and shipping analysis

The model provides a centralized analytical foundation for the dashboard rather than relying on isolated calculations within individual visuals.

## 7. Analytical Flow

The overall analytical structure can be represented as:

**Business Performance → Customer → Product → Location → Operations**

Users can move from high-level KPIs into more detailed dimensions of business performance.

## 8. Data Model Validation

The model was developed to support consistent calculations across the dashboard. Measures and dimensions are reused across multiple report pages to maintain consistency in analytical reporting.

## 9. Dashboard Pages Supported

The data model supports the following report pages:

1. **Overview**
2. **Customer Performance**
3. **Product Performance**
4. **Location Performance**
5. **Operational Analysis**

## 10. Conclusion

The data model serves as the analytical backbone of the De Meridian Superstore Power BI Dashboard. By organizing business information around transactional, customer, product, geographical, shipping, and time-based analysis, the model enables interactive reporting and supports data-driven business interpretation.
