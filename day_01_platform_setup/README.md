# Day 1 – Platform Setup & First Data Load  
**Databricks + Unity Catalog + Spark**

---

## 🎯 Objective
Set up the Databricks environment with Unity Catalog and successfully load raw e-commerce event data into Spark.

---

## 🧠 Key Learnings

### Databricks Runtime
- SparkSession (`spark`) is auto-created in Databricks notebooks
- No need to manually initialize `SparkSession`

### Storage & Governance
- Public DBFS root (`/FileStore`) is disabled in Unity Catalog environments
- All governed file access must use:
