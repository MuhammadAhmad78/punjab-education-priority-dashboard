# Data Dictionary

**File:** `data/pakistan_district_education_priority_punjab_2019_20.csv`
**Rows:** 36 (one per Punjab district)
**Encoding:** UTF-8, comma-separated

| Column | Type | Description |
|---|---|---|
| `Rank` | Integer | District rank by Primary Education Score, 1 = highest need. Ties share a rank. |
| `Province` | Text | Province name — all rows are `Punjab`. |
| `District` | Text | Name of the district. |
| `Literacy Rate (%)` | Numeric | Overall literacy rate for the district (both genders). |
| `Female Literacy Rate (%)` | Numeric | Literacy rate among females specifically. |
| `Gender Literacy Gap (pp)` | Numeric | Difference in percentage points between overall/male literacy and female literacy. Higher = larger gender disparity. |
| `Out-of-School Rate (%)` | Numeric | Percentage of primary-school-age children not enrolled in school. |
| `Primary Education Score` | Numeric (0–100) | Composite priority score. Higher score = greater need for education investment. |
| `Priority Level` | Categorical | One of `Critical`, `High`, `Medium`, `Lower` — derived from the Primary Education Score. |

## Notes

- Data reflects the 2019–20 reference period.
- "pp" = percentage points (used for the literacy gap, since it's a difference of two percentages).
- Source figures are consistent with province-level education survey data for Punjab; recommended to cross-verify against the original source before use in official reporting.
