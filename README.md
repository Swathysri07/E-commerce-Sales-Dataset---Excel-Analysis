# E-Commerce Sales Analysis - Excel

## Project Overview

This project analyzes an e-commerce sales dataset using Microsoft Excel. The objective is to understand overall sales performance, customer and product trends, discount impact, regional performance, payment preferences, and store-level performance.

The workbook brings together data preparation, formula-based analysis, descriptive statistics, PivotTable analysis, charts, and an interactive-style dashboard.

## Project Objectives

- Organize and prepare the e-commerce sales dataset for analysis.
- Review data quality and prepare fields for reporting.
- Use Excel formulas and statistical measures to understand the dataset.
- Summarize business performance using PivotTables.
- Compare sales across years, quarters, months, categories, regions, products, payment methods, customer segments, and stores.
- Present key metrics and trends in a dashboard.

## Dataset

The analysis uses 2,000 sales transactions, covering:

- 500 customers
- 100 products
- 20 stores

The dataset includes the following fields:

| Column | Description |
|---|---|
| `Sales_ID` | Unique sales transaction identifier |
| `Order_Date` | Date of the transaction |
| `Order_Year` | Year extracted from the order date |
| `Order_MONTH` | Month extracted from the order date |
| `Customer_ID` | Customer identifier |
| `Product_ID` | Product identifier |
| `Store_ID` | Store identifier |
| `Quantity` | Quantity recorded in the transaction |
| `Quantity_F` | Prepared quantity field used in analysis |
| `Unit_Price` | Unit price |
| `Unit_Price_F` | Prepared unit-price field used in analysis |
| `Discount` | Discount information |
| `Discount_F` | Prepared discount field used in analysis |
| `Payment_Type` | Payment method |
| `Total_Amount` | Transaction amount |
| `Total_Amount_F` | Prepared transaction amount used in analysis |
| `Gross_Sales` | Sales amount before discount |
| `Discount_Amount` | Discount value |
| `Customer_Name` | Customer name |
| `Product_Name` | Product name |
| `Category` | Product category |
| `Region` | Sales region |
| `Store_Type` | Store-related field in the source data |
| `Loyalty_Level` | Customer loyalty segment |
| `Gender` | Customer gender field |

## Workbook Structure

The workbook contains the source sales data and analysis outputs, including descriptive analysis, PivotTable-based summaries, and a dashboard sheet.

- **Sales data:** Main transaction-level dataset.
- **Descriptive Analysis:** Statistical and descriptive review of the sales data.
- **Pivot Analysis:** Summaries used to compare business performance across different dimensions.
- **Dashboard:** Visual summary of important KPIs and sales trends.

*Use the actual worksheet names in the workbook if they differ from the labels above.*

## Data Preparation and Analysis Approach

The dataset was reviewed and prepared for analysis using Excel. Prepared fields such as `Quantity_F`, `Unit_Price_F`, `Discount_F`, and `Total_Amount_F` were used in the analysis outputs.

The analysis includes:
- Reviewing transaction, date, customer, product, store, category, region, and payment fields.
- Using prepared numeric fields for consistent calculations and summaries.
- Grouping sales by year, quarter, month, category, region, product, payment type, loyalty level, gender, and store.
- Comparing gross sales, discount amount, and net sales.

> Note: This README documents the fields and analysis outputs shared during the project discussion. Add or amend specific cleaning operations (such as duplicate removal, missing-value treatment, or Power Query steps) only if they were actually performed in the final workbook.

## Descriptive Statistics

Descriptive statistics were calculated for `Total_Amount`:

| Measure | Result |
|---|---:|
| Count | 2,000 |
| Sum | â‚¹21,74,394.70 |
| Mean | â‚¹1,087.20 |
| Median | â‚¹868.72 |
| Standard Deviation | â‚¹819.62 |
| Skewness | 0.8790 |
| Kurtosis | 0.0458 |
| Minimum | â‚¹18.46 |
| Maximum | â‚¹3,908.24 |

### Interpretation

- The average transaction value is approximately â‚¹1,087.20.
- The median is lower than the mean, indicating that some higher-value transactions pull the average upward.
- The positive skewness value indicates a right-skewed transaction-value distribution.
- Transaction values range from approximately â‚¹18.46 to â‚¹3,908.24.

## Key Performance Indicators

| KPI | Result |
|---|---:|
| Total Orders / Transactions | 2,000 |
| Total Customers | 500 |
| Total Products | 100 |
| Total Stores | 20 |
| Total Quantity Sold | 4,964 |
| Gross Sales | â‚¹25,56,367.56 |
| Total Discount Amount | â‚¹3,81,973.02 |
| Net Sales | â‚¹21,74,394.70 |
| Average Order Value (AOV) | â‚¹1,087.20 |

## PivotTable Analysis

The following summaries were created to explore different aspects of business performance.

### 1. Year-wise Sales Analysis

| Year | Net Sales |
|---|---:|
| 2023 | â‚¹2,23,813 |
| 2024 | â‚¹10,93,912 |
| 2025 | â‚¹8,56,670 |

**Finding:** 2024 recorded the highest net sales among the three years shown.

### 2. Quarter-wise Sales Analysis

Quarterly sales were compared across 2023, 2024, and 2025 to identify seasonal patterns and changes in performance.

| Year | Q1 | Q2 | Q3 | Q4 |
|---|---:|---:|---:|---:|
| 2023 | â‚¹10,866 | â‚¹21,846 | â‚¹24,700 | â‚¹1,66,401 |
| 2024 | â‚¹2,86,691 | â‚¹2,58,587 | â‚¹2,73,878 | â‚¹2,74,756 |
| 2025 | â‚¹2,45,893 | â‚¹2,69,783 | â‚¹2,52,378 | â‚¹88,617 |

**Finding:** 2025 Q4 is notably lower than the earlier quarters shown. It may require further investigation, including checking the date coverage and whether the year contains a complete quarter.

### 3. Category-wise Sales Analysis

| Category | Quantity | Discount Amount | Net Sales |
|---|---:|---:|---:|
| Sports | 1,241 | â‚¹93,502 | â‚¹5,42,010 |
| Electronics | 1,165 | â‚¹88,113 | â‚¹5,04,311 |
| Home | 974 | â‚¹77,564 | â‚¹4,27,296 |
| Clothing | 846 | â‚¹64,037 | â‚¹3,79,216 |
| Beauty | 738 | â‚¹58,756 | â‚¹3,21,561 |

**Finding:** Sports is the highest-selling category by net sales in the summary, followed by Electronics.

### 4. Region-wise Sales Analysis

| Region | Quantity | Net Sales |
|---|---:|---:|
| North | 1,508 | â‚¹6,46,101 |
| South | 1,416 | â‚¹6,35,213 |
| East | 1,447 | â‚¹6,22,404 |
| West | 593 | â‚¹2,70,676 |

**Finding:** North recorded the highest net sales. West recorded the lowest sales among the four regions.

### 5. Top-Selling Products

The product summary was used to compare products by sales value and quantity sold.

| Product | Net Sales | Quantity |
|---|---:|---:|
| Portable Power Bank | â‚¹41,852.50 | 84 |
| Shin Guards â€“ Adult | â‚¹38,281.02 | 77 |
| Men's Casual Sneakers | â‚¹35,489.62 | 87 |
| Gaming Mechanical Keyboard | â‚¹34,699.83 | 84 |
| Women's High Heels | â‚¹33,993.66 | 67 |
| Wireless Mouse | â‚¹33,566.80 | 73 |
| Basketball | â‚¹31,070.46 | 63 |
| Men's Hair Styling Gel | â‚¹30,236.70 | 66 |
| Women's Formal Blazer | â‚¹28,572.69 | 45 |
| Soccer Training Cone Set | â‚¹28,324.05 | 70 |

**Finding:** Portable Power Bank generated the highest sales value in the displayed product list. Men's Casual Sneakers recorded the highest quantity among these ten products.

### 6. Payment Method Analysis

| Payment Type | Transactions | Sales |
|---|---:|---:|
| PayPal | 695 | â‚¹7,56,754.57 |
| Credit Card | 645 | â‚¹7,15,180.71 |
| COD | 660 | â‚¹7,02,459.42 |

**Finding:** PayPal had the highest transaction count and sales value among the payment methods shown.

### 7. Gender and Loyalty-Level Analysis

The PivotTable compared customer counts by gender across loyalty levels.

| Loyalty Level | Female | Male | Total |
|---|---:|---:|---:|
| Platinum | 366 | 240 | 606 |
| Bronze | 229 | 258 | 487 |
| Gold | 280 | 189 | 469 |
| Silver | 215 | 207 | 422 |
| Not Assigned | 6 | 10 | 16 |
| **Total** | **1,096** | **904** | **2,000** |

**Finding:** Platinum is the largest loyalty segment in the summary. The customer count is 1,096 female and 904 male.

### 8. Gross Sales vs Net Sales

| Year | Gross Sales | Net Sales |
|---|---:|---:|
| 2023 | â‚¹2,65,472 | â‚¹2,23,813 |
| 2024 | â‚¹12,86,139 | â‚¹10,93,912 |
| 2025 | â‚¹10,04,757 | â‚¹8,56,670 |
| **Grand Total** | **â‚¹25,56,367.56** | **â‚¹21,74,394.70** |

**Finding:** Total gross sales were â‚¹25,56,367.56 and total net sales were â‚¹21,74,394.70. The difference represents approximately â‚¹3,81,973.02 in discounts.

### 9. Store-wise Sales Performance

Store-level sales were compared using transaction count and net sales.

- Highest sales in the displayed list: Thompsonborough â€“ â‚¹1,58,971 across 127 transactions.
- Second in the displayed list: Hoodberg â€“ â‚¹1,25,012 across 114 transactions.
- Lowest sales in the displayed list: New Michaelchester â€“ â‚¹81,344 across 83 transactions.

*The source PivotTable heading was described as Store Type, but the values supplied were location-like names. This README therefore refers to them as store/location entries rather than assuming they are store-type categories.*

### 10. Monthly Sales Trend

Monthly sales were summarized to observe changes over time and identify peaks or dips. The monthly trend can be used to monitor sales movement throughout the reporting period.

## Dashboard and Visualizations

A dedicated Dashboard worksheet was created to bring key business metrics and analysis charts together.

The dashboard setup included:
- A dedicated worksheet named `Dashboard`.
- Gridlines hidden for a cleaner presentation.
- Zoom set to 80%.
- A consistent dashboard working area across columns A to L.
- A merged title area with the heading **E-COMMERCE SALES PERFORMANCE DASHBOARD**.
- A subtitle: **BUSINESS PERFORMANCE OVERVIEW | 2023 â€“ 2025**.

The planned chart mapping for the analysis is:

| Analysis | Suggested Chart |
|---|---|
| Year-wise Sales | Clustered Column |
| Top 10 Best-Selling Products | Clustered Bar |
| Category-wise Sales | Pie |
| Monthly Sales Trend | Line |
| Region-wise Sales | Clustered Bar |
| Payment Method Analysis | Doughnut |
| Gender vs Loyalty Level | Stacked Column |
| Quarterly Sales Analysis | Clustered Column |
| Gross Sales vs Net Sales | Clustered Column |
| Store-wise Sales Performance | Bar |

*Keep only the charts that are present in the final workbook. The chart types above document the chart plan discussed during the project.*

## Macros and Dashboard Controls

VBA macros were discussed for dashboard convenience.

### Refresh All

The refresh macro used for refreshing workbook connections and PivotTable data:

```vb
Sub Refresh_Dashboard()

    ThisWorkbook.RefreshAll

    MsgBox "Dashboard refreshed successfully!", vbInformation

End Sub
```

### Toggle Full-Screen View

A toggle macro was prepared to switch between full-screen dashboard view and normal Excel view:

```vb
Sub Toggle_Dashboard_FullScreen()

    Application.DisplayFullScreen = Not Application.DisplayFullScreen

    If Application.DisplayFullScreen = True Then
        ActiveWindow.DisplayHeadings = False
        ActiveWindow.DisplayGridlines = False
    Else
        ActiveWindow.DisplayHeadings = True
    End If

End Sub
```

*These macros are documented because their code was prepared during the project. Confirm that the buttons are assigned and working in the final `.xlsm` workbook before describing them as tested features.*

## Overall Business Insights

1. **Annual performance:** 2024 recorded the highest net sales in the three-year summary.
2. **Category performance:** Sports led the category-wise sales summary, with Electronics in second place.
3. **Regional performance:** North led the regions, while West had the lowest sales and quantity.
4. **Product performance:** Portable Power Bank had the highest sales value in the displayed top-product list.
5. **Payment preference:** PayPal recorded the highest sales value and transaction count among the payment methods shown.
6. **Customer segmentation:** Platinum was the largest loyalty segment in the gender-versus-loyalty summary.
7. **Discount impact:** The difference between gross and net sales was approximately â‚¹3.82 lakh.
8. **Quarterly movement:** 2025 Q4 was notably lower than the earlier quarters shown and should be checked against the dataset's date coverage.

## Excel Skills Demonstrated

- Spreadsheet organization and data handling
- Excel formulas and calculated fields
- Descriptive statistics
- PivotTable-based summarization
- Comparative and trend analysis
- KPI reporting
- Chart selection and dashboard layout
- Basic VBA macro preparation for refresh and full-screen controls

## Conclusion

This project demonstrates how Excel can be used to move from transaction-level sales data to meaningful business summaries. Descriptive statistics help understand the distribution of transaction values, while PivotTables make it easier to compare performance across products, categories, regions, time periods, payment methods, customer segments, and stores. The dashboard brings the key results together in a single reporting view.

The analysis highlights the strongest-performing year, category, region, products, and payment method, while also identifying areasâ€”such as West region sales and the 2025 Q4 declineâ€”that may deserve further investigation.

---

**Tools:** Microsoft Excel, PivotTables, Excel formulas, charts, and VBA macros (where enabled in the final workbook).

