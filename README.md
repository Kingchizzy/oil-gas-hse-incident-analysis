# Oil & Gas HSE Incident Analysis Using Python

## Project Overview

This project explores simulated Health, Safety and Environment (HSE) incident data from oil and gas operations using Python. The analysis focuses on incident types, severity, primary causes, work activities, site distributions, near misses, and monthly incident patterns.

The objective is to demonstrate how data analytics can support safety monitoring, identify recurring incident patterns, and inform preventive HSE interventions.

**Note:** The dataset is simulated for portfolio and learning purposes. The findings do not represent the actual safety performance of any oil and gas company.

## Business Problem

Oil and gas operations involve activities with varying levels of occupational and operational risk. Analysing incident records can help HSE teams identify recurring patterns, investigate areas requiring attention, and prioritise preventive measures.

This project addresses the following questions:

- Which incident types occur most frequently?
- How are incidents distributed across severity levels and operational sites?
- What causes and work activities are associated with reported incidents?
- Where are near misses most frequently recorded?
- What patterns appear in the monthly incident data?
- What preventive actions could be considered based on the findings?

## Project Objectives

- Load, inspect, and clean the incident dataset.
- Standardise inconsistent categorical values.
- Assess missing values, duplicate records, and data quality issues.
- Perform exploratory data analysis (EDA).
- Examine incident types, severity, causes, sites, and work activities.
- Analyse near-miss patterns and monthly incident trends.
- Develop practical, data-informed HSE recommendations.

## Tools and Technologies

- **Python** — data analysis and processing
- **Pandas** — data cleaning, transformation, and aggregation
- **NumPy** — numerical operations and data quality corrections
- **Matplotlib and Seaborn** — data visualisation
- **Jupyter Notebook** — interactive analysis and documentation
- **GitHub** — project versioning and portfolio presentation

## Dataset Description

The simulated dataset initially contained 302 rows and 14 columns. After exact duplicate rows were removed, 300 records remained.

The dataset includes fields relating to:

- Incident identification and date
- Operational site and department
- Incident type and severity
- Work activity and primary cause
- Body part affected
- Lost workdays and corrective-action days
- Work shift and contractor
- Incident status

Data preparation also involved standardising categories, converting date values, assessing missing information, and reviewing invalid numerical values.

## Key Findings

The exploratory analysis identified the following patterns in the cleaned dataset:

- **Near misses were the most frequently recorded incident type**, with 105 records.
- **First aid incidents accounted for 62 records**, followed by property damage with 45 records.
- **Low severity was the most common recorded severity category**, with 142 records; 4 records had missing severity values.
- **Offshore Platform B recorded 26 near misses**, followed by Gas Processing Plant with 23.
- **Hot work recorded 16 near misses**, the highest count among the listed work activities.
- **Pipeline Operations recorded 22 high- or critical-severity incidents**, the highest site count in this category.

These are counts from simulated records, not incident rates. Comparisons between sites would require additional information, such as workforce size, hours worked, or activity exposure. Monthly trends should also be interpreted cautiously because some source dates are ambiguous and the final month may be incomplete.

## Recommendations

Based on the patterns observed, the following actions could be considered in a real HSE setting:

1. **Strengthen near-miss reporting and follow-up:** Review reported near misses, document corrective actions, and assess whether similar events recur.
2. **Review higher-count work activities:** Examine controls, procedures, and supervision for activities such as hot work, lifting operations, and equipment maintenance.
3. **Investigate site-level patterns:** Review high incident counts alongside workforce exposure and operational activity before prioritising interventions.
4. **Improve data quality:** Standardise incident categories, investigate missing fields, validate dates, and review unusual numerical values.
5. **Monitor corrective actions:** Track action closure, overdue items, and recurring causes to support continuous improvement.
6. **Use exposure-adjusted metrics:** Where reliable operational data is available, calculate appropriate incident rates rather than relying on counts alone.

These recommendations are analytical suggestions, not conclusions about the performance of a real organisation.

## Project Structure

```text
oil-gas-hse-incident-analysis/
│
├── HSE_Python_Project_Consolidated.ipynb
├── oil_gas_hse_raw_data.csv
└── README.md
```

## How to Run the Project

1. Download or clone this repository.
2. Ensure Python and the required libraries are installed.
3. Open `HSE_Python_Project_Consolidated.ipynb` in Jupyter Notebook or JupyterLab.
4. Keep `oil_gas_hse_raw_data.csv` in the same folder as the notebook.
5. Run the notebook cells from top to bottom.

Required libraries:

```python
pip install pandas numpy matplotlib seaborn jupyter
```

## Limitations

- The dataset is simulated and may not reflect the complexity of real HSE reporting.
- Missing and ambiguous values can affect the interpretation of some results.
- Incident counts alone do not measure risk or establish causation.
- Monthly comparisons require validated dates and consideration of incomplete reporting periods.
- Recommendations would need to be validated against operational context before being applied in a real workplace.

## Conclusion

This project demonstrates a structured Python workflow for cleaning, exploring, and interpreting HSE incident data. It highlights how data quality checks, exploratory analysis, and clear reporting can help identify patterns that warrant further investigation and support evidence-informed safety discussions.

The project forms part of my data analytics portfolio and reflects my interest in applying analytical skills to operational and occupational safety data.

**Author:** Beulah Emefiena

**Project repository:** [Oil & Gas HSE Incident Analysis](https://github.com/Kingchizzy/oil-gas-hse-incident-analysis)
