# 🏍️ Motorbike Sales Dashboard: Excel Data Analysis

An Excel data-analysis project: clean a raw customer dataset, summarise it with **PivotTables**, and present the results in an interactive **dashboard with slicers** to find out **which customers buy a motorbike**.

![Motorbike Sales Dashboard](images/dashboard.jpg)

## Key insights
- **48.1 %** of customers bought a bike (481 of 1,000).
- **Middle-aged customers (31-54) make up 80 % of buyers** and buy at 54.6 %, versus 31.2 % for Old (55+) and 35.5 % for Young (under 31).
- **Short commutes buy more:** 54.6 % at 0-1 miles and 58.6 % at 2-5 miles, falling to 29.7 % beyond 10 miles.
- **Buyers earn more on average** in both genders (male 60,124 vs 56,208; female 55,774 vs 53,440), and men earn more than women in both groups.

➡️ Full tables, recommendations and limitations: [`docs/insights.md`](docs/insights.md)

## Business question
Which customer characteristics are associated with buying a bike, so marketing can target the right customers?

## Dataset
| | |
|---|---|
| Raw records | 1,026 |
| Cleaned records | 1,000 (26 duplicates removed) |
| Columns | 13 original + 1 derived (`Age Range`) |
| Outcome | `Purchased Bike` (Yes / No) |

Field definitions: [`docs/data_dictionary.md`](docs/data_dictionary.md)

## What I did in Excel
1. **Cleaned the data** - removed 26 duplicates, replaced the M/S and M/F codes with Married/Single and Male/Female, renamed "10+ Miles", and created an `Age Range` column with an `IF` formula. → [`docs/data_cleaning.md`](docs/data_cleaning.md)
2. **Built three PivotTables** - average income by gender, purchases by age range, and purchases by commute distance, each split by purchase status.
3. **Created three charts** - one column chart and two line charts linked to the PivotTables.
4. **Added four slicers** - Gender, Marital Status, Region and Education - which filter all charts at once.
5. **Designed the dashboard** - a title banner, slicer panel and chart layout. → [`docs/dashboard_guide.md`](docs/dashboard_guide.md)

## Recommendations
1. Focus on customers aged **31-54**.
2. Target customers who **live within 5 miles**.
3. **Pilot offers** for Young and Old customers, who buy less often.
4. De-prioritise customers living **more than 10 miles** away.

## Repository structure
```
motorbike-sales-dashboard/
├── README.md
├── LICENSE
├── excel/
│   └── Motorbike_Sales_Project.xlsx    # raw data, cleaned data, PivotTables, dashboard
├── data/
│   ├── bike_buyers_raw.csv             # export of the raw sheet (1,026 rows)
│   └── bike_buyers_cleaned.csv         # export of the cleaned sheet (1,000 rows)
├── images/
│   └── dashboard.jpg
└── docs/
    ├── data_dictionary.md
    ├── data_cleaning.md
    ├── dashboard_guide.md
    └── insights.md
```

## How to use
1. Download `excel/Motorbike_Sales_Project.xlsx` and open it in **desktop Excel**.
2. Go to the **Dashboard** sheet and click the slicers to filter.
3. Inspect `Working Sheet (Cleaned)` and `Pivot Table` to see how the numbers are built. (Use *Data → Refresh All* if values look stale.)

The CSV files are plain exports of the two data sheets for quick viewing on GitHub; they contain no PivotTables or slicers.

## Limitations
The analysis is descriptive, so it shows association rather than cause. The data has no dates, prices or revenue. The dataset's source and income currency are not documented.

## Skills demonstrated
Data cleaning · Excel formulas · PivotTables & PivotCharts · Slicers · Dashboard design · Descriptive analysis · Business recommendations

## Author
**<Your Name>** · [LinkedIn](https://linkedin.com/in/your-profile)
