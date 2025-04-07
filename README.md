# Day_1
## 🧹 Data Cleaning Overview

This document outlines the comprehensive data cleaning procedures applied to the dataset to ensure high data quality and consistency for reliable analysis.

---

### 🔧 Data Cleaning Steps

#### 1. Column Header Standardization
- Converted all column names to lowercase  
- Replaced spaces with underscores  
- Removed special characters  
- Ensured consistent naming conventions across all fields  

#### 2. Missing Value Handling
- Identified and quantified missing values across all columns  
- Applied appropriate imputation strategies:  
  - **Numerical columns:** Median imputation  
  - **Categorical columns:** Mode imputation or added an "Unknown" category  
- Removed columns with more than 70% missing values  

#### 3. Duplicate Detection and Removal
- Detected duplicate records using invoice IDs and key business fields  
- Removed exact duplicates, keeping the first occurrence  
- Flagged potential fuzzy duplicates for manual review  

#### 4. Data Type Conversion
- Converted date fields to proper datetime format  
- Ensured numerical fields used appropriate numeric types  
- Standardized categorical variables  

#### 5. Outlier Detection and Treatment
- Identified outliers using the Interquartile Range (IQR) method  
- Capped extreme values at reasonable thresholds  
- Flagged records with potential data entry errors for further review  

#### 6. Text Data Cleaning
- Standardized text to consistent casing  
- Trimmed extra whitespace  
- Addressed inconsistencies in categorical text values  
- Applied basic text normalization techniques  

#### 7. Data Validation Rules
- Applied business logic checks to ensure data integrity  
- Validated numerical fields against acceptable ranges  
- Ensured referential integrity where applicable  
- Flagged records that violated established validation rules  
