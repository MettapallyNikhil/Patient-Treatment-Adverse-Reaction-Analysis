# 🧠 Patient Treatment & Adverse Reaction Analysis (KNIME)
## 📌 Project Overview
This project presents a complete data preprocessing and integration pipeline built using KNIME to analyze patient treatment data alongside adverse reactions.
The workflow transforms raw, unstructured healthcare data into a clean, structured dataset by applying data cleaning, feature engineering, and dataset merging techniques.

## 🎯 Objective
* Clean and structure raw patient treatment data
* Extract meaningful features (e.g., HbA1c change)
* Integrate adverse reaction data with treatment records
* Prepare dataset for analysis, visualization, or machine learning

## 🛠 Tools & Technologies
* KNIME Analytics Platform
* CSV Data Processing
* UTF-8 Encoding
* Data Transformation & Feature Engineering
* Data Integration (Join / Lookup)

## 🔄 Workflow Steps
### 1. Data Import
* Loaded raw dataset using CSV Reader with UTF-8 encoding
* Ensured compatibility and proper parsing

### 2. Data Structuring (Column Splitting)
* Applied Cell Splitter nodes
* Converted merged columns into structured attributes

### 3. Column Reconstruction
* Used Column Combiner
* Rebuilt meaningful fields from split data

### 4. Data Cleaning
* Applied String Cleaner nodes
* Removed noise and standardized text

### 5. Column Standardization
* Used Column Renamer
* Improved readability and consistency

### 6. Data Refinement
* Applied Column Filter
* Retained only relevant attributes

### 7. Feature Engineering
* Calculated:
  * **HbA1c Change = End Value – Start Value**
* Implemented using Expression node

### 8. Column Organization
* Used Column Resorter
* Structured dataset for better interpretability

### 9. Data Integration (Adverse Reactions)
* Imported adverse reaction dataset
* Merged using Value Lookup (VLOOKUP logic)

### 10. Post-Merge Cleanup
* Removed unnecessary columns
* Applied Missing Value handling

### 11. Row Identification
* Generated unique Row IDs
* Ensured traceability of records

### 12. Final Output Preparation
* Final column arrangement using Column Resorter
* Produced clean dataset ready for analysis

## 📊 Results
* Clean and structured patient dataset
* Computed HbA1c change values
* Integrated adverse reaction information
* Dataset ready for:
  * Predictive modeling
  * Statistical analysis
  * Healthcare insights

## 📷 Workflow Preview

Add your workflow screenshot here:

<img width="1755" height="461" alt="image" src="https://github.com/user-attachments/assets/1b0cadbd-f4fd-4334-b308-3003785f704a" />

## 🧩 Key Concepts Demonstrated

* Data Cleaning
* Feature Engineering
* Data Transformation
* Data Integration (Join Logic)
* Workflow Automation

## 🚀 How to Run

1. Clone the repository:
```bash
git clone https://github.com/your-username/knime-patient-treatment-analysis.git
```
2. Open KNIME
3. Import workflow:

```
File → Import KNIME Workflow
```
4. Select the `workflow/` folder

5. Execute all nodes

## 💡 Future Improvements

* Add visualization dashboards (KNIME / Python)
* Apply machine learning models
* Automate anomaly detection in adverse reactions
* Integrate real-time data pipelines
