📊 AdventureWorks Sales & Customer Performance Dashboard

## 1. Project Overview
This Power BI project provides a **comprehensive view of sales, customer behavior, and product performance** for AdventureWorks.  
The dashboards help management monitor **revenue growth, customer value, returns, and refunds**, while identifying areas for optimization through **what-if analysis and root cause analysis**.

<img width="639" height="361" alt="Screenshot 2025-09-07 183655" src="https://github.com/user-attachments/assets/8db59837-36a2-48ae-81e2-ec40576407bb" />


<img width="637" height="399" alt="Screenshot 2025-09-07 183718" src="https://github.com/user-attachments/assets/aad88da3-950b-49ea-9c57-c57105fef041" />


<img width="640" height="360" alt="Screenshot 2025-09-07 183729" src="https://github.com/user-attachments/assets/db25732c-f8a4-4e5c-8a16-77403c80028b" />



## 2. Key KPIs
The following KPIs were defined and tracked:

### **Sales & Profitability**
- **Revenue**: $24.9M  
- **Profit**: $10.5M  
- **Total Orders**: 25.2K  
- **Return Rate**: 2.2%  

### **Customer Metrics**
- **Total Customers**: 17.4K  
- **Revenue per Customer**: $1,431  
- **Top Customer**: Maurice Shan → 6 orders, $12.41K revenue  

### **Refund & Returns (Root Cause)**
- **Total Refunds**: $21,256  
- **Total Returns**: 1,115  
- **Most Refunded Category**: Accessories (Tires & Tubes, Helmets, Hydration Packs)

---


<img width="632" height="348" alt="Screenshot 2025-09-07 183750" src="https://github.com/user-attachments/assets/f4220dbd-3fea-497e-a397-5c6a41b478b4" />




## 3. Data Preparation (Power Query Steps)
Data was imported from **AdventureWorks sales tables** and cleaned using Power Query:

1. **Data Cleaning**
   - Removed duplicates, null values, and unused columns.
   - Standardized date formats.
   - Created calculated columns for *Year, Month, Week*.

2. **Transformations**
   - Transformed sales, products, and customer tables.
   - Normalized product categories and subcategories.
   - Added **income level** and **occupation segmentation** for customer analysis.

3. **Modeling**
   - Established **star schema** .
   - Relationships set to *single direction* for optimized performance.

---

## 4. Insights

### **Revenue & Orders**
- Revenue shows steady growth with a **spike in mid-2021**.
- Monthly revenue reached **$1.83M**, up **+3.31%** from the previous month.
- Orders slightly declined (-0.88%), while returns increased (+1.78%).

### **Customer Performance**
- Professional customers generated the highest revenue segment.
- Top 100 customers contributed **$615K** in revenue.
- **Maurice Shan** was the top customer with **$12.41K** revenue.

### **Product Performance**
- Bestselling: **Mountain Bikes (200 Black, 38 & 42)**.
- Most ordered product type: **Tires and Tubes**.
- Most returned product type: **Shorts**.

### **Refund Analysis**
- Refunds concentrated in **Accessories ($21,256)**.
- Within Accessories, **Tires and Tubes** and **Helmets** had the largest share.

---

## 5. What-If Analysis
- Simulated scenarios with price adjustments, cost rates, and order quantity.

---

<img width="640" height="363" alt="Screenshot 2025-09-07 183739" src="https://github.com/user-attachments/assets/4bf63fd3-6dba-44d3-b56c-26a04c7ecf9a" />



## 6. Root Cause Analysis (Refunds)
- Accessories caused **90%+ of refunds**.
- Within Accessories:
  - **Tires & Tubes ($7.7K refunds)**
  - **Helmets ($4.1K)**
  - **Hydration Packs ($1.2K)**

**Insight:** Product quality or supply chain issues in **bike accessories** are driving refunds.

---

## 7. Business Recommendations
1. **Customer Retention**: Focus on high-value professional customers with loyalty offers.
2. **Product Improvement**: Investigate refund root causes in **Tires & Tubes and Helmets**.
3. **Order Growth**: Encourage cross-selling with bundles to raise orders per customer.
4. **Returns Control**: Enhance product descriptions/quality checks to reduce return rate below 2%.
5. **What-If Scenarios**: Use price and cost simulations for pricing strategy.

---



