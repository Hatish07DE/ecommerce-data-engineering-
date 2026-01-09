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


---

## 🔄 Day-1 Workflow

1. Download dataset using Kaggle CLI
2. Extract files in cluster `/tmp`
3. Move CSV files into Unity Catalog volume
4. Read CSV into Spark DataFrame
5. Validate load with `count()` and `show()`

---

## 🧪 Validation Performed
- Verified record count
- Parsed event timestamp
- Confirmed data accessibility through governed volume

---

## 📁 Notebook
All executable code for Day-1 is available here:

➡️ **`day1_data_load.ipynb`**



