# Task 12: Missing Value Identification

## Objective
Identify missing values in a dataset and summarize where they occur.

## Tools Used
- Python
- Pandas
- Excel

## Dataset
Titanic-style passenger dataset containing 30 records and 8 columns.

## Work Done
- Identified missing values using `isnull()` and `isna()`.
- Counted missing values column-wise.
- Calculated missing-value percentages.
- Summarized missing and non-missing values.
- Suggested suitable methods for handling missing data.

## Key Findings
- Age: 3 missing values.
- Fare: 2 missing values.
- Embarked: 2 missing values.
- Other columns have no missing values.
- No rows or values were deleted.

## Python Code
```python
import pandas as pd

df = pd.read_csv("titanic_practice.csv")

missing = df.isnull().sum()
percentage = (missing / len(df)) * 100

summary = pd.DataFrame({
    "Missing Values": missing,
    "Missing Percentage": percentage
})

print(summary)
```

## Deliverables
1. Excel workbook with raw data and missing-value summary.
2. Missing-value identification report.
3. Key findings and recommendations.

## Conclusion
Successfully identified and summarized missing values using Python and Pandas. This task helped understand basic missing-data inspection and the importance of handling missing values carefully without blindly deleting data.

**Internship:** Veda Technology – Data Analytics Track
