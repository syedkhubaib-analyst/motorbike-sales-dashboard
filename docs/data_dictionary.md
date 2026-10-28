# Data Dictionary

Raw sheet `bike_buyers (Raw Data)`: 1,026 rows × 13 columns.
Cleaned sheet `Working Sheet (Cleaned)`: 1,000 rows × 14 columns (adds `Age Range`).

| Column | Type | Description / values |
|---|---|---|
| ID | Number | Customer ID (unique in the cleaned sheet) |
| Marital Status | Text | Married / Single (raw data: M / S) |
| Gender | Text | Male / Female (raw data: M / F) |
| Income | Number | Annual income, 10,000 to 170,000 (currency not stated in the data) |
| Children | Number | Number of children, 0 to 5 |
| Education | Text | Partial High School, High School, Partial College, Bachelors, Graduate Degree |
| Occupation | Text | Manual, Skilled Manual, Clerical, Professional, Management |
| Home Owner | Text | Yes / No |
| Cars | Number | Number of cars owned, 0 to 4 |
| Commute Distance | Text | 0-1 Miles, 1-2 Miles, 2-5 Miles, 5-10 Miles, More than 10 Miles (raw data: "10+ Miles") |
| Region | Text | Europe, North America, Pacific |
| Age | Number | Customer age, 25 to 89 |
| **Age Range** | Text (formula) | **Derived column.** Young: under 31 · Middle Age: 31 to 54 · Old: 55 and over |
| Purchased Bike | Text | **Outcome.** Yes / No |
