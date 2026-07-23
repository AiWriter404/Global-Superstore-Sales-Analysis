# 📊 Global Superstore - Sales & Profit Analysis

Exploratory data analysis and business insights on global retail sales data — uncovering trends in sales, profit, discount impact, and regional performance across 51,000+ transactions using Python (Pandas, Matplotlib, Seaborn).

## 🏆 Key Business Insights

- **Overall Profit Margin:** 11.6% ($1.47M profit on $12.64M in sales)
- **Growth:** Sales grew ~90% and profit grew ~100% from 2011 to 2014
- **Category issue:** Furniture has the weakest margin (6.9%) vs Technology/Office Supplies (~14%)
- **Root cause:** Furniture carries the highest average discount (16.8%)
- **Universal pattern:** Discounts above ~30-40% consistently push orders into a loss, across every category
- **Regional gap:** Canada is the standout market (26.6% margin); EMEA is the weakest (5.4% margin)
- **Product-level culprit:** *Tables* is the only sub-category losing money overall (-$64,083), driven by a 29.1% average discount — causing 57.6% of Table orders to be unprofitable

## 📁 Dataset

**Global Superstore Sales Data** — 51,290 orders across 24 columns, covering:
- Order/shipping details (dates, ship mode, priority)
- Geography (Country, Market, Region, State, City)
- Product info (Category, Sub-Category, Product Name)
- Financials (Sales, Discount, Profit, Shipping Cost, Quantity)
- Customer info (Customer Name, Segment)

## 🔍 Analysis Workflow

1. **Data Loading & Exploration**
   - Dataset shape, column overview, data types, sample rows

2. **Data Cleaning**
   - Dropped `Postal Code` (80.5% missing, not needed for analysis)
   - Converted `Order Date` / `Ship Date` to proper datetime format
   - Extracted `Order Year` and `Order Month` for time-based analysis

3. **Business KPI Overview**
   - Total sales, total profit, total orders, average discount, overall profit margin

4. **Category & Sub-Category Analysis**
   - Sales and profit breakdown by Category
   - Identified Furniture as the weakest-margin category
   - Drilled down to Sub-Category level — found *Tables* as the sole loss-making product line

5. **Discount Impact Analysis**
   - Compared average discount vs profit across categories
   - Visualized Discount vs Profit relationship (scatter plot) showing losses accelerate past ~30-40% discount

6. **Regional / Market Analysis**
   - Compared profit margins across Markets (APAC, EU, US, LATAM, Africa, EMEA, Canada)
   - Highlighted Canada as the best performer and EMEA as needing urgent review

7. **Time Trend Analysis**
   - Year-over-year sales and profit growth (2011–2014)

8. **Root Cause Analysis — Tables**
   - Verified Tables' average discount (29.1%) vs all other products (14.0%)
   - Found 57.6% of Table orders result in a loss

9. **Executive Summary & Recommendations**
   - Consolidated key metrics into a single summary table
   - Translated findings into actionable business recommendations

## 💡 Business Recommendations

1. **Cap discounts on Tables** — bring the ~29% average down toward the ~15% seen on other products
2. **Set a company-wide discount ceiling** (e.g., 30%) — orders beyond this threshold are consistently unprofitable
3. **Investigate EMEA operations** — review pricing, shipping costs, and discounting practices in this region
4. **Study and replicate Canada's model** — its unusually high margin may reveal practices worth applying elsewhere
5. **Sustain the growth trajectory** while addressing the margin issues above to improve overall profitability

## 🛠️ Tech Stack

- **Python**
- **Pandas / NumPy** — data manipulation
- **Matplotlib / Seaborn** — visualization

## 📁 Repository Structure

```
├── Global_Superstore_Sales_Analysis.ipynb   # Full notebook (EDA → Insights)
├── Global_Superstore2.csv                    # Dataset
└── README.md
```

## 🔗 Links

- **Kaggle Notebook:** [Global Superstore Sales Analysis](https://www.kaggle.com/code/muhammadumer7804/global-superstore-sales-analysis)
- **GitHub Repository:** [Global-Superstore-Sales-Analysis](https://github.com/AiWriter404/Global-Superstore-Sales-Analysis)

## 👤 Author

**Muhammad Umer**

---

*This project was built as a hands-on exercise in exploratory data analysis and translating raw data into clear, actionable business insights.*
