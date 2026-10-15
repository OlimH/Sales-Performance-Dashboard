# 📊 Sales Performance Dashboard — Power BI

A complete Power BI dashboard analyzing sales performance, customer behavior, product trends, and category insights.  
This project demonstrates data modeling, DAX calculations, interactive visuals, and AI-generated narrative insights.

---

## 🚀 Features
- Total Customers, Orders, Sales, Growth %, AOV  
- Monthly Sales Trend (Line Chart)  
- Customer Score vs Total Sales (Scatter Plot)  
- Category Sales Breakdown (Donut Chart)  
- Product-Level Sales (Bar Chart)  
- AI Narrative Insights (Auto-generated)  
- Interactive Filters (Country, Product Type, Date)

---

## 🖼️ Dashboard Preview

### Overview
![Dashboard Overview]([assets/dashboard_overview.png](https://github.com/OlimH/Sales-Performance-Dashboard/blob/main/Dashboard_Overview.png))

### Monthly Sales
![Monthly Sales](assets/monthly_sales.png)

### Category Sales
![Category Sales](assets/category_sales.png)

### Product Sales
![Product Sales](assets/product_sales.png)

### Customer Score Analysis
![Customer Score](assets/customer_score.png)

### AI Narrative
![AI Narrative](assets/ai_narrative.png)

---

## 🔗 Live Dashboard
👉 Add your Power BI link here once published.

---

## 🧠 Key Insights
- Sales trended down over the last 12 months.  
- Laptops contributed **57.32%** of total sales.  
- ThinkPad X1 is the top-performing product (8.1K).  
- The United States leads in customer total sales.  
- Customer scores vary significantly across countries.

---

## 🧮 DAX Measures Used
```DAX
Total Sales = SUM(Orders[Sales])
Total Orders = COUNTROWS(Orders)
Average Order Value = DIVIDE([Total Sales], [Total Orders])
Customer Total Sales = SUMX(RELATEDTABLE(Orders), Orders[Sales])
