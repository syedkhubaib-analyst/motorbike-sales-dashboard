# Data Cleaning

Cleaning was done in Excel: `bike_buyers (Raw Data)` (untouched, kept as an audit trail) → `Working Sheet (Cleaned)`.

| # | Step | Result |
|---|---|---|
| 1 | Removed duplicate records | 1,026 → **1,000** rows (26 duplicates removed; every ID now unique) |
| 2 | Replaced Marital Status codes `M` / `S` | `Married` / `Single` |
| 3 | Replaced Gender codes `M` / `F` | `Male` / `Female` |
| 4 | Renamed commute label `10+ Miles` | `More than 10 Miles` |
| 5 | Created `Age Range` with a formula | `Young` / `Middle Age` / `Old` |

**Age Range formula** (cell M2, filled down):

```excel
=IF(L2>54,"Old",IF(L2>=31,"Middle Age",IF(L2<31,"Young","Invalid")))
```

## Checks on the cleaned sheet
| Check | Result |
|---|---|
| Rows | 1,000 |
| Duplicate rows | 0 |
| Blank cells | 0 |
| Records with `Purchased Bike = Yes` / `No` | 481 / 519 |
