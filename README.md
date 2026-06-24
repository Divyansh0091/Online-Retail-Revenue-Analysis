# Online Retail Sales Revenue Analysis

## 📊 Project Overview
This project provides an end-to-end data analysis pipeline, starting from fetching raw transaction data from a **PostgreSQL** database to performing advanced data cleaning and generating business-critical sales trends. The goal was to transform raw retail transactions into actionable revenue insights.

## 🛠 Tech Stack
* **Database:** PostgreSQL (via SQLAlchemy)
* **Data Analysis:** Python (Pandas, NumPy)
* **Visualization:** Matplotlib, Seaborn
* **Environment:** Jupyter Notebook

## 🚀 Key Process Steps
1.  **Data Extraction:** Connected to the PostgreSQL database to query live transaction records.
2.  **Data Cleaning:** * Handled missing values (`Customer ID`, `Description`).
    * Identified and removed anomalies (negative quantity values which represent returns/cancellations) to ensure accurate calculation of gross demand.
3.  **Feature Engineering:**
    * Calculated `Total Revenue` per transaction (Quantity * Unit Price).
    * Transformed date data for time-series resampling.
4.  **Trend Analysis:** Resampled data into monthly intervals to visualize sales volume and revenue growth over time.

## 📈 Business Insights (Conclusion)
* **Revenue Growth:** The analysis highlights a clear revenue spike in November, suggesting strong seasonal holiday demand (Black Friday/Christmas impact).
* **Operational Health:** By separating 'Returns' from 'Gross Sales', we identified the true demand volume.
* **Strategic Recommendation:** The upward revenue trend suggests that marketing spend should be optimized during the Q4 period to capitalize on peak demand.

## 📂 Repository Structure
- `Retail_Sales_Analysis_SQL_Python.ipynb` : Main analysis notebook.
- `requirements.txt` : List of libraries used.

---
*Created by [Tera Naam Likha Yahan]*
