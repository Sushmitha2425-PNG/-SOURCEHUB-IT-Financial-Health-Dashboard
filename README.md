# 💰 Financial Health Dashboard

## 🎯 **Goal**

The goal is to help **individuals or businesses evaluate financial performance**, **identify spending patterns**, and **make better budgeting decisions**.

## 📘 **Project Overview**

The **Financial Health Dashboard** analyzes and visualizes an organization’s financial performance across various departments and employees.
It focuses on understanding how **income flows into deductions, expenses, savings, and profit**, providing insights into financial strengths and weaknesses.

---

## 🧩 **Step-by-Step Project Workflow**

### **Step 1: Collecting the Raw Dataset**

* Collected the raw dataset from **Kaggle**.
* Dataset includes key financial data such as:

  * Monthly Salary, Income Tax, PF Contribution, Insurance Deduction, Other Deductions, Savings, Investments, and Profit.

---

### **Step 2: Data Preprocessing in Excel**

* Cleaned and refined the raw data using **Microsoft Excel**:

  * Removed unnecessary columns and duplicates.
  * Filtered out invalid or missing entries.
  * Verified correct data types (especially numeric and date fields).
  * Ensured column names were consistent and meaningful.

---

### **Step 3: Importing Data into Power BI**

* Imported the **cleaned dataset** into **Power BI Desktop**.
* Used the **Power Query Editor** to:

  * Reconfirm column names and data types.
  * Check for null values or formatting errors.
  * Validate that no data inconsistencies remained.

---

### **Step 4: Creating DAX Calculations**

Created a calculated column for **Total Deductions** using DAX:

```DAX
Total Deductions =  
SUM(employee_financial_data[Income_Tax]) +
SUM(employee_financial_data[Insurance_Deduction]) +
SUM(employee_financial_data[Other_Deductions]) +
SUM(employee_financial_data[PF_Contribution])
```

🧮 This helped measure total employee deductions for accurate profit computation and performance comparison.

---

### **Step 5: Building Visuals and Designing the Dashboard**

After verifying data integrity, visualization was started in **Power BI** using different chart types to represent various financial metrics.

| Visualization                                               | Purpose                                                                         |
| ----------------------------------------------------------- | ------------------------------------------------------------------------------- |
| **KPI Cards**                                               | Display Total Expenditure, Profit, Deductions, Savings, Investments, and Salary |
| **Donut Chart – Financial Balance**                         | Show percentage distribution of Expenditure, Savings, and Investments           |
| **Bar Chart – Savings by Department**                       | Compare how each department saves                                               |
| **Pie Chart – Total Expenditure by Department**             | Visualize departmental spending share                                           |
| **Line Chart – Profit by Department**                       | Identify departments with profit or loss trends                                 |
| **Column Chart – Profit by Employee_ID**                    | Track profit contribution at employee level                                     |
| **Dual Line Chart – Savings vs Investments by Employee_ID** | Compare financial growth trends for employees                                   |
| **Slicer – Class (High, Medium, Low)**                      | Filter financial performance categories interactively                           |

---

### **Step 6: Interpreting and Analyzing the Results**

#### **🔹 Overall Financial Metrics**

* **Total Expenditure:** 2M
* **Average Profit:** -918.74 (negative profit indicates losses)
* **Total Deductions:** 49M
* **Total Savings:** 615K
* **Total Investments:** 404K
* **Total Salary:** 976K

🟣 *Insight:* High expenditure and deductions cause profit decline despite positive savings and investments.

---

#### **🔹 Financial Balance (Donut Chart)**

* **Expenditure:** 61.63%
* **Savings:** 23.16%
* **Investments:** 15.2%

📊 *Insight:* Over 60% of income goes into expenditure, leaving less for savings and investments — shows spending dominance.

---

#### **🔹 Department-Level Findings**

* **Tech Department:** Highest expenditure (31.2%) but lowest profit — potential overspending.
* **Finance Department:** Lowest expenditure (9%) — efficient management.
* **Tech Department** also leads in savings, possibly due to higher salary structure.

---

#### **🔹 Employee-Level Findings**

* **Profit by Employee_ID:** Shows wide variation — many employees incur losses, some show high profit.
* **Savings vs Investments:** Employees with higher savings also invest more — positive correlation.

---

## 📊 **Dashboard Summary**

| Aspect                    | Observation                                | Insight                                                |
| ------------------------- | ------------------------------------------ | ------------------------------------------------------ |
| **Profitability**         | Average Profit is negative                 | Indicates need to control expenses or increase revenue |
| **Expenditure Pattern**   | Tech Department uses 31% of total spending | Spending optimization needed                           |
| **Savings & Investments** | 23% and 15% respectively                   | Financially aware, but needs higher saving ratio       |
| **Employee Contribution** | Inconsistent profit distribution           | Suggests unequal cost or performance levels            |

---

## 💡 **Conclusion — How the Title “Financial Health” is Proven**

The dashboard accurately reflects **financial health** by:

1. Tracking **income, expenses, deductions, savings, and profit** through dynamic KPIs.
2. Highlighting **spending patterns and imbalances** between departments.
3. Providing a **clear picture of where costs can be reduced** and profits improved.
4. Enabling **data-driven financial planning** for future budgeting and resource allocation.

✅ **Result:**
The dashboard clearly demonstrates that while the organization shows positive saving and investment behavior, **profitability suffers due to high expenditures**.
This comprehensive visualization provides a roadmap for **improving financial stability and performance**.

---

## 🧰 **Tools & Technologies Used**

* **Excel** → Data cleaning and preprocessing
* **Power BI Desktop** → Data modeling and visualization
* **DAX (Data Analysis Expressions)** → Custom calculations and KPIs
* **Kaggle** → Dataset source

---

## 🧠 **Key Learnings**

* Importance of **data preprocessing** before visualization.
* Creating **custom DAX measures** for financial KPIs.
* Designing dashboards with **clear storytelling and data insight flow**.
* Interpreting visual data to assess **financial strength and weakness**.

---

## 🚀 **Final Takeaway**

The **Financial Health Dashboard** provides actionable insights into how an organization manages its funds — tracking expenditures, analyzing deductions, and identifying areas for improvement.
It serves as a valuable tool for **financial decision-making**, **budget optimization**, and **long-term business planning**.

---


