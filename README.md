# excel-reporting-improvement
Anonymised Case Study: Transforming messy monthly reports into analytics-ready dataset for easier insights.

# From Data Chaos to Reporting Clarity

![Infographic](data-chaos-to-clarity.png)

## Case Study: Optimizing Demographic Reporting for Analytics & Decision-Making

### Context
Monthly reports were submitted in a flat, operational format across branches. While functional for records, they required heavy manual processing for insights on youth/non-youth participation, gender distribution, transaction volumes, and performance trends.

### The Problem
- Key metrics were hidden and required repetitive manual calculations.
- Inconsistent structure made it incompatible with BI tools or automated dashboards.
- High risk of errors from manual cleaning.

### The Solution
Redesigned the master dataset to be analytics-ready:
- Added explicit **Youth (≤35)** and **Non-Youth (>35)** columns using Excel formulas:
  - Youth: `=IF(AND(ISNUMBER(Age), Age <= 35), 1, 0)`
  - Non-Youth: `=IF(AND(ISNUMBER(Age), Age > 35), 1, 0)`
- Standardized fields (time intelligence: calendar year, fiscal year, month).
- Enforced consistency with data validation (dropdowns for Gender, Sector).
- Split multi-owner entries into separate rows for accurate individual counts.

### Outcome
- Drastically reduced manual effort.
- Enabled instant insights via pivot tables and dashboards.
- Fully compatible with BI tools—no extra transformation needed.

### Skills Demonstrated
- Data structuring & cleaning
- Reporting optimization
- Analytics enablement
- BI-ready dataset design
- Excel formulas, validation, and pivot tables

### Sample Files
- [Sample Before and After Dataset] (https://github.com/adatashift/excel-reporting-improvement/blob/main/sample_dataset_before_and%20after.xlsx)

### Before vs. After Table
| Before (Messy)                  | After (Analytics-Ready)                  |
|---------------------------------|------------------------------------------|
| Multi-owners in one cell        | Separate rows per individual             |
| Manual youth calculation        | Auto-computed columns                    |
| No unique IDs                   | BusinessID for tracking                  |
| Inconsistent fields             | Standardized + validation                |

Next: Building a lightweight Excel dashboard with pivots for at-a-glance metrics (within resource constraints).
