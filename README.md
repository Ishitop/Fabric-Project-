📊 Population Analysis with Microsoft Fabric
This project analyzes global population data using Microsoft Fabric. It covers the full data pipeline — from ingestion to reporting — using Lakehouse, Spark, and Power BI.

🔧 Tools & Services Used
Microsoft Fabric

Lakehouse

Apache Spark (Notebooks in Fabric)

Power BI

GitHub (Data Source)

📁 Project Workflow
🔄 Data Ingestion
Used Copy Data activity (HTTP connector) to pull a population dataset from a public GitHub URL.

Loaded the raw data into Microsoft Fabric Lakehouse.

🧹 Data Transformation
Opened the raw data using a Spark Notebook in Fabric.

Cleaned the dataset: removed nulls, renamed columns, and fixed data types.

Stored the cleaned data in a new table in the Lakehouse.

📈 Reporting
Connected Power BI directly to the Lakehouse.

Built visualizations showing population trends by country, region, and year.

Published an interactive Power BI report for stakeholders.

📊 Sample Insights
Top 10 most populous countries

Population growth trends over time

Regional population comparisons

🗂️ Folder Structure (Fabric)
swift
Copy
Edit
/Lakehouse/
  ├── Raw/
  │   └── population_raw.csv
  ├── Cleaned/
  │   └── population_cleaned.parquet
/Spark Notebooks/
  └── transform_population_data.ipynb
/Power BI/
  └── population_analysis.pbix
✅ How to Use
Clone or fork the repository.

Update the Copy Data activity to point to the latest GitHub dataset URL.

Run the Spark notebook to transform the data.

Open the Power BI report and refresh the data source.

📌 Notes
Make sure you have access to a Fabric workspace with Lakehouse, Notebooks, and Power BI.

This project can be extended with forecasting, demographic breakdowns, or integration with other datasets.
