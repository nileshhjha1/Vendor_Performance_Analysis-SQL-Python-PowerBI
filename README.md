# Vendor Performance Analysis

## 📌 Project Overview  
This project aims to analyse the performance of vendors (suppliers) using a full-stack analytical workflow combining SQL, Python and Power BI. The goal is to extract, transform and load vendor/supply-chain data, perform descriptive and diagnostic analysis, compute key performance metrics and visualise insights to support vendor management decisions (selection, evaluation, improvement).

Key components:
- **Data ingestion & ETL** via SQL + Python  
- **Analysis & metric calculation** in Python  
- **Dashboarding & interactive visualisation** in Power BI  
- Modular folder structure for clarity (Ingestion, Summary, Dashboard, Scripts, Notebooks, Logs, Images)  
- Reusable SQL queries & Python scripts for vendor summary and deeper analytics  

---

## 🗂 Repository Structure  

```
/Dashboard/             → Power BI (.pbix) file(s) and supporting files
/Get_Vendor_summary/    → SQL & Python scripts to build vendor summary tables
/Images/                → Visualisations, screenshots, diagrams
/Ingestion/             → Raw data ingestion, staging, ETL scripts
/Logs/                  → Process logs, outputs, error tracking
/Notebooks/             → Jupyter notebooks (exploratory analysis, prototyping)
/Scripts/               → Stand-alone Python modules & utilities
requirements.txt        → Python dependencies
README.md               → This file
```

---

## 🧰 Technologies & Tools  
- **SQL** – Used for data extraction, transformation and loading (ETL) into staging and summary tables  
- **Python** – For data cleaning, feature engineering, aggregation, metric computations & automation  
- **Power BI** – For building interactive dashboards, visualising vendor performance KPIs, drilling into details  
- **Jupyter Notebooks** – For exploratory analysis, prototyping and documentation of findings  
- **Pandas / NumPy / Matplotlib / Seaborn** – Typical Python libraries for analysis  
- **requirements.txt** – Lists specific Python dependencies required for the scripts  

---

## 🚀 Getting Started  
Follow these steps to set up and run the analysis:

1. **Clone the repository**
   ```bash
   git clone https://github.com/nileshhjha1/Vendor_Performance_Analysis-SQL-Python-PowerBI.git
   cd Vendor_Performance_Analysis-SQL-Python-PowerBI
   ```

2. **Install Python dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Prepare your database / data warehouse**
   - Create a staging schema (e.g., `stg_vendor`) for raw ingestion
   - Create a summary schema (e.g., `sum_vendor`) for aggregated tables
   - Update connection parameters (host, database, user, password) in scripts/notebooks

4. **Run the ingestion & ETL**
   - In `/Ingestion/`, execute the SQL scripts to load raw vendor data
   - Run Python scripts in `/Scripts/` to clean, transform and load data into summary tables

5. **Summarise vendor performance**
   - Open `/Get_Vendor_summary/` scripts or notebook
   - Run the SQL and/or Python analysis to compute key vendor metrics (on-time delivery, quality defects, order-fill rate, cost variance, etc.)

6. **Open the Power BI dashboard**
   - In `/Dashboard/`, open the `.pbix` file
   - Connect to the summary tables in your database
   - Explore interactive visuals, filters and drill-downs

---

## 📊 Key Vendor Performance Metrics

Here are some of the sample metrics that this project tracks (you may customise as needed):

- On-time delivery rate
- Order fill/completeness rate
- Quality defect rate (number of defective units / total units)
- Cost variance (actual cost vs budgeted cost)
- Lead time variance
- Vendor ranking / scorecard
- Trend analysis (monthly/quarterly)
- Top / bottom vendor performance by category, region, product

---

## 🔧 Customising the Solution

- Update the database connection strings in the Python scripts and Power BI data source
- Modify / extend SQL scripts to incorporate new tables, new vendor KPIs
- Expand the Jupyter notebooks for deeper analysis (predictive modelling, clustering of vendor behaviours)
- Enhance the Power BI dashboard by adding new visuals, bookmarks, tooltips, drill-throughs
- Schedule the ingestion & metric pipelines via cron / Airflow / Windows Task Scheduler for automation

---

## ✅ Why This Approach Works

- Combines structured data (SQL) with flexible analytics (Python) and powerful visualisation (Power BI)
- Modular folder structure promotes re-usability and clarity
- End-to-end workflow from raw data to actionable insights
- Adaptable and scalable: you can plug in new data sources, metrics, vendors and visualisations

---

## 📚 References & Resources

- Python libraries: pandas, numpy, matplotlib, seaborn
- Microsoft documentation for Power BI
- SQL ETL best-practices (staging → summary → presentation layers)
- Vendor management and supply chain performance metrics literature

---

## 📝 Contributing & License

Feel free to fork this repository, raise issues, suggest improvements or add your own vendor KPIs and dashboards.
You may adapt this solution for your organisation's vendor performance analytics.
*(Add a licence if you wish — e.g., MIT License)*

---

## 🙋 Contact

For any questions or suggestions, please create an issue in the repository or contact me at **[nileshhjha1@gmail.com](mailto:nileshhjha1@gmail.com)**

---

Thanks for checking out this Vendor Performance Analysis solution!
Let's turn data into vendor management insights. 💡
