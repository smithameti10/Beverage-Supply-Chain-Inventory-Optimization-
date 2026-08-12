# Beverage Supply Chain & Inventory Optimization

## 📌 Project Overview

This project analyzes beverage distribution data to understand **supplier performance, inventory movement, product activity, and supplier dependency**.

The analysis focuses on three major inventory movements:

- **Retail Sales** – products sold through retail operations
- **Retail Transfers** – inventory moved between retail locations/channels
- **Warehouse Sales** – products moved or sold through the warehouse channel

The main objective is to **optimize supplier relationships, improve inventory movement, identify high-performing and inactive products, and reduce supply-chain risk**.

---

## 🎯 Business Problem

The company works with hundreds of suppliers and thousands of beverage products.

The key business questions are:

- Which suppliers contribute the most to sales and inventory movement?
- How dependent is the business on its major suppliers?
- Which product categories have the highest inventory movement?
- Which products show little or no activity?
- How are retail sales, transfers, and warehouse sales related?
- Where are potential supplier and inventory-management risks?

---

## 📊 Dataset

The dataset contains **330,080 records and 9 columns**.

| Column | Description |
|---|---|
| `year` | Year of activity |
| `month` | Month of activity |
| `supplier` | Product supplier |
| `item code` | Product identifier |
| `item description` | Product description |
| `item type` | Product category |
| `retail sales` | Retail sales activity |
| `retail transfers` | Retail transfer activity |
| `warehouse sales` | Warehouse sales activity |

---

## 🛠️ Tools & Technologies

- **Python**
- **Pandas** – data cleaning and analysis
- **NumPy** – numerical operations
- **Matplotlib** – visualization
- **Seaborn** – statistical visualization
- **Jupyter Notebook** – analysis environment

---

## 🔍 Analysis Performed

### Data Cleaning

- Standardized column names
- Converted sales and transfer fields into numeric format
- Handled missing values
- Preserved negative movements for investigation
- Checked data types and data quality

### Exploratory Data Analysis

- Dataset structure and summary statistics
- Missing-value and zero-activity analysis
- Correlation analysis
- Distribution and skewness analysis
- Outlier analysis

### Inventory Activity Classification

Records were classified into:

- Multiple Activities
- Warehouse Sales Only
- Retail Sales Only
- Retail Transfer Only
- No Activity

<img width="1243" height="588" alt="image" src="https://github.com/user-attachments/assets/920e9845-84de-478d-bdc2-9e353cbbe8ff" />


### Supplier Analysis

- Top suppliers by retail sales
- Top suppliers by warehouse sales
- Supplier contribution
- Top-20 supplier concentration
- Supplier specialization by category

### Product & Category Analysis

- Inventory movement by item type
- High-volume categories
- Inactive/dead-stock records
- Product-level sales distribution
- Outlier identification

### Trend Analysis

Yearly comparison of:

- Retail sales
- Retail transfers
- Warehouse sales
  
<img width="705" height="567" alt="image" src="https://github.com/user-attachments/assets/011606db-5fc1-4ed2-b7c9-f734b7771aa6" />


---

## 📈 Key Findings

### Inventory Activity

| Activity Type | Records | Share |
|---|---:|---:|
| Multiple Activities | 143,548 | 43.49% |
| Warehouse Sales Only | 127,182 | 38.53% |
| Retail Sales Only | 56,281 | 17.05% |
| Retail Transfer Only | 1,921 | 0.58% |
| No Activity | 1,148 | 0.35% |

Warehouse-related activity is a major part of the supply chain, and a large proportion of records involve multiple activity types.

### Category Movement

**Beer** is the largest-moving category, with approximately **6.55 million units of total movement** in the multiple-activity analysis.

It is followed by:

1. Wine – ~2.47 million
2. Liquor – ~1.83 million
3. Other categories – substantially lower movement

<img width="1235" height="735" alt="image" src="https://github.com/user-attachments/assets/cf974f45-2e48-4e01-88bb-43368c3feec1" />


### Supplier Concentration

The top 20 suppliers contribute approximately:

- **67.49%** of retail sales
- **79.16%** of warehouse sales
- **67.82%** of retail transfers

<img width="828" height="493" alt="image" src="https://github.com/user-attachments/assets/c153cd03-0364-4d94-80a9-786468d9fbbf" />


This indicates significant dependency on a group of major suppliers, particularly for warehouse activity.

### Supplier Leaders

- **Top retail-sales supplier:** E & J GALLO WINERY
- **Top warehouse-sales supplier:** CROWN IMPORTS

### Inactive Inventory

The analysis identified **1,148 records with no retail sales, retail transfers, or warehouse sales**.

Largest inactive categories:

- Wine – 767
- Beer – 164
- Liquor – 106
- Kegs – 102

These may represent slow-moving, obsolete, discontinued, temporarily inactive, or problematic records.

### Sales Distribution

Retail sales are highly **right-skewed**: most records have low or zero activity, while a relatively small number of products generate very high sales.

<img width="903" height="315" alt="image" src="https://github.com/user-attachments/assets/e3848d7f-f4b2-46f8-900b-aa7f1dfefa33" />

---

## 💡 Business Recommendations

### 1. Manage Supplier Dependency

Create a supplier-risk matrix using:

- Sales contribution
- Warehouse contribution
- Category dependency
- Product breadth
- Alternative-supplier availability

### 2. Diversify Critical Suppliers

Identify alternative suppliers for high-volume and strategically important products.

### 3. Negotiate with Major Suppliers

Use purchasing scale to negotiate:

- Better purchase prices
- Lower freight costs
- Volume discounts
- Better payment terms
- Improved service levels

### 4. Optimize Beer Inventory

Prioritize Beer for:

- Demand forecasting
- Replenishment planning
- Warehouse capacity planning
- Supplier monitoring

### 5. Investigate Inactive Products

Review zero-activity products and determine whether they should be:

- Reordered
- Discounted
- Transferred
- Returned
- Discontinued

### 6. Use Product Segmentation

Classify products into groups such as:

- High Sales / High Movement
- High Sales / Low Movement
- Low Sales / High Movement
- Low Sales / Low Movement

---

## 🚀 Future Enhancements

The project can be extended with:

- Supplier profitability analysis
- Gross margin analysis
- Bulk purchasing and unit-cost analysis
- Inventory turnover analysis
- ABC product classification
- Supplier risk scoring
- Product-level profitability
- Demand forecasting
- Inventory replenishment optimization
