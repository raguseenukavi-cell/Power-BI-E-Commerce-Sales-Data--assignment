# # E-Commerce Sales Data Preparation & Modeling Using Power BI

## 📌 Project Overview

This project focuses on preparing, cleaning, transforming, and modeling e-commerce sales data using **Microsoft Power BI and Power Query Editor**.

As an aspiring Data Analyst, I am developing practical skills by working with multiple related datasets containing order information, product details, and monthly sales targets. The objective is to transform raw data into a clean, consistent, and structured data model suitable for business intelligence and reporting.

## 🎯 Project Objectives

- Import multiple CSV files into Power BI.
- Clean and transform data using Power Query Editor.
- Handle missing values and duplicate records.
- Create custom and conditional columns.
- Merge tables using common keys.
- Perform grouping and aggregation.
- Establish and validate relationships between datasets.
- Prepare data for further analysis and dashboard development.

## 🗂️ Datasets Used

### 1. List of Orders
Contains customer and order-level information.

- Order ID
- Order Date
- Customer Name
- City
- State
- Category
- Amount
- Profit

### 2. Order Details
Contains product-level transaction information.

- Order ID
- Category
- Sub-Category
- Quantity
- Amount
- Profit

### 3. Sales Target
Contains monthly sales target information.

- Category
- Month of Order Date
- Target

## 🛠️ Tools & Technologies

- Microsoft Power BI
- Power Query Editor
- Data Cleaning and Transformation
- Data Modeling and Relationships
- Data Aggregation
- CSV Data Import

## 🔄 Project Workflow

### 1. Data Import
- Imported the List of Orders, Order Details, and Sales Target datasets.
- Opened Power Query Editor using the Transform Data option.

### 2. Data Transformation
- Restricted the List of Orders dataset to the first 500 rows.
- Converted Order Date to the Date data type.
- Converted Amount and Target to Fixed Decimal Number.
- Applied Proper Case formatting to Customer Name.
- Created a Location column by combining City and State.

### 3. Custom Column Creation

**Profit Margin**

Calculated the profit margin using:

`Profit Margin = Profit / Amount`

The result represents profit as a proportion of sales. It can be formatted as a percentage for easier interpretation. Rows with zero or missing Amount values require appropriate handling.

**Profit Status**

Created a conditional column using the following business rules:

| Condition | Profit Status |
|---|---|
| Profit < 0 | Loss |
| Profit = 0 | Break-Even |
| Profit > 0 | Profit |

### 4. Data Merging
- Merged List of Orders and Order Details using Order ID.
- Named the merged output table `Orders Data`.
- Used the common key to combine order-level and product-level information.

### 5. Data Cleaning
- Identified missing values across all three datasets.
- Considered suitable methods for handling missing values, including replacement, removal of invalid records, and retaining null values when appropriate.
- Identified duplicate rows and considered business rules before removing records.

### 6. Sorting and Filtering
- Sorted Orders Data by Order Date in descending order.
- Applied a state filter, such as Tamil Nadu, to analyze orders from a selected location.

### 7. Grouping and Aggregation

**Order Details Analysis**

Prepared grouped summaries for:

- Count of Order ID
- Average Profit by Category
- Total Amount by Sub-Category

**Sales Target Analysis**

Prepared a grouped summary of total Target by Month of Order Date.

These summaries help organize transaction data for further analysis.

### 8. Data Modeling
Planned the following relationships:

- List of Orders ↔ Order Details using Order ID.
- Order Details ↔ Sales Target using Category.

Used Manage Relationships to review relationship activity, keys, and cardinality.

**Modeling consideration:** Relationship cardinality must match the actual data. If both tables contain repeated Category values, a direct many-to-many relationship may not be the best design. A suitable category dimension or bridge table may be required to ensure accurate filtering and aggregation.

## 📈 Expected Outcomes

This project is designed to demonstrate practical understanding of:

- Data preparation and cleansing.
- Power Query transformations.
- Custom and conditional columns.
- Table merging and grouping.
- Aggregation of sales and profit data.
- Relationship modeling in Power BI.
- Preparing structured data for business reporting.

## 📁 Repository Structure

The repository can be organized as follows:

```text
ecommerce-sales-powerbi-data-modeling/
│
├── README.md
├── power-bi-assignment.pbix
├── documentation/
│   └── project-documentation.pdf
│
└── screenshots/
    ├── data-transformation.png
    ├── data-cleaning.png
    ├── grouped-data.png
    └── data-model-view.png
```

*Add the folders and files as you prepare them. The names above are suggested examples.*

## 🚀 Future Improvements

- Build an interactive E-commerce Sales Dashboard.
- Analyze total sales, profit, and profit margin.
- Compare monthly sales targets with actual sales.
- Explore category-wise and state-wise performance.
- Add KPI cards, charts, and interactive slicers.
- Develop actionable business insights from the prepared data.

## 👨‍💻 About Me

I am an **Aspiring Data Analyst** building my skills through practical projects and hands-on learning.

I am interested in data cleaning, data transformation, data modeling, data visualization, and business intelligence using tools such as Microsoft Excel and Power BI.

This project is part of my learning journey and the development of my data analytics portfolio on GitHub.

## 🏷️ Skills Demonstrated

`Power BI` `Power Query` `Data Cleaning` `Data Transformation` `Data Modeling` `Data Aggregation` `Business Intelligence` `E-Commerce Analytics`

---

**Project Type:** Data Analytics Assignment  
**Tool:** Microsoft Power BI  
**Focus:** Data Preparation and Modeling
Power-BI-E-Commerce-Sales-Data--assignment
