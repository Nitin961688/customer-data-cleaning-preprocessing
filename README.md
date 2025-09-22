# customer-data-cleaning-preprocessing
## 📌 Project Overview
This repository contains the solution for **Task 1: Data Cleaning and Preprocessing**, using a raw **Customer Dataset**.  
The objective was to clean, preprocess, and prepare the dataset for further analysis or modeling.

## 🛠️ Tools Used
- Python (Pandas, NumPy)
- Jupyter Notebook
- Dataset: `sample_customer_data.csv`

## 📂 Files in Repository
- `Customer_data_TasK1.ipynb` → Jupyter Notebook with step-by-step cleaning process.  
- `sample_customer_data.csv` → Raw dataset.  
- `customer_data_cleaned.csv` → Final cleaned dataset.  
- `README.md` → This documentation file.

## 🔍 Steps Performed
1. **Loaded the raw dataset** into Pandas.  
2. **Checked missing values** using `.isnull()`.  
   - Filled categorical nulls with `"Unknown"`.  
   - For numerical columns, filled missing values with mean/median.  
   - For critical fields like `date`, rows with missing values were dropped.  
3. **Removed duplicate records** using `.drop_duplicates()`.  
4. **Standardized column names** → lowercase, no spaces (`customer_id` instead of `Customer ID`).  
5. **Standardized text values** (e.g., gender → `Male`, `Female`).  
6. **Converted date formats** to `datetime` (`dd-mm-yyyy`).  
7. **Checked and fixed data types**:  
   - Age → integer  
   - Date → datetime  
   - Income/Spending → float  
8. **Exported the cleaned dataset** as `customer_data_cleaned.csv`

## 📊 Key Learnings
- Handling **missing values** (drop vs. fill).  
- Removing **duplicates** for reliable analysis.  
- Importance of **standardizing text and column names**.  
- Handling **date formats** and ensuring correct data types.  
- Preparing a dataset that is **structured, consistent, and analysis-ready**

## Deliverables

Cleaned Dataset: customer_data_cleaned.csv

Notebook: Customer_data_TasK1.ipynb

Documentation: README.md

👨‍💻 Author

Task completed by Nitin Kumar as part of a Data Cleaning and Preprocessing exercise.
