# Python Diwali Sales Analysis

This project performs Exploratory Data Analysis (EDA) on Diwali sales data to understand customer behavior and sales patterns across demographics, geography, occupation, and product categories.

## Project Structure

- `Diwali Sales Data.csv`
  Main dataset used for analysis.
- `.ipynb_checkpoints/Diwali Sales Analysis-checkpoint.ipynb`
  Jupyter notebook checkpoint containing all data cleaning, EDA steps, visualizations, and conclusion.

## Dataset Overview

The dataset includes customer and transaction-level fields such as:

- `User_ID`
- `Cust_name`
- `Product_ID`
- `Gender`
- `Age Group`
- `Age`
- `Marital_Status`
- `State`
- `Zone`
- `Occupation`
- `Product_Category`
- `Orders`
- `Amount`
- `Status`
- `unnamed1`

## Analysis Workflow In Notebook

The notebook follows this sequence:

1. Import libraries: NumPy, Pandas, Matplotlib, Seaborn.
2. Load CSV using `unicode_escape` encoding.
3. Inspect shape, head, and data info.
4. Clean data:
   - Drop unrelated/blank columns: `Status`, `unnamed1`
   - Handle missing values with `dropna()`
   - Convert `Amount` to integer type
5. Perform descriptive statistics (`describe`).
6. Run EDA with visualizations for:
   - Gender
   - Age Group
   - State
   - Marital Status
   - Occupation
   - Product Category
   - Top selling Product IDs

## Key Insights From Notebook

- Most buyers are female.
- Female customers show higher purchasing power than male customers.
- Highest buyer segment: women in the 26-35 age group.
- Top contributing states include Uttar Pradesh, Maharashtra, and Karnataka.
- Married women contribute significantly to sales.
- Strong buyer occupations include IT, Healthcare, and Aviation.
- Most purchased categories include Food, Clothing, and Electronics.
- Overall target profile noted in notebook conclusion:
  Married women aged 26-35 from UP, Maharashtra, and Karnataka, especially in IT/Healthcare/Aviation, are more likely to purchase in Food/Clothing/Electronics.

## How To Run

1. Install Python 3.9+.
2. Install required libraries:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

3. Open Jupyter Notebook:

```bash
jupyter notebook
```

4. Open and run notebook:

- `.ipynb_checkpoints/Diwali Sales Analysis-checkpoint.ipynb`

## Notes

- The notebook currently available is a checkpoint file inside `.ipynb_checkpoints`.
- Some text values in the CSV (for example `Andhra Pradesh`) may appear with encoding artifacts depending on viewer settings.
