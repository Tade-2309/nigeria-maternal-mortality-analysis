# Data Quality and Cleaning Notes

## Scope of inspection

These notes are based on comparing the `Nigeria_Maternal_Mortality_Dirt` and `CLEANED DATA` worksheets in the submitted Excel workbook. They describe observable differences and issues; they do not assume undocumented cleaning steps.

## Record and field counts

| Item | Original worksheet | Cleaned worksheet |
|---|---:|---:|
| Data records | 2,600 | 2,563 |
| Fields | 28 | 33 |

The cleaned worksheet therefore contains 37 fewer records and five additional fields. The workbook does not contain a complete row-level exclusion log explaining why each of the 37 records was removed. Add that evidence if it exists in your working notes.

## Observable preparation

The cleaned worksheet has more standardised categorical values and includes additional analytical fields, including geopolitical zone, age group, distance category, maternal-death flag and length of stay. The original and cleaned sheets both remain in the workbook, which makes comparison possible.

## Items requiring review before final publication

1. **ANC visit value of 99:** The cleaned worksheet still contains a value of `99` in `ANC_Visits`. Confirm whether this represents an unknown/missing-value code or an actual value. If it is a code, recode it consistently and document the rule.
2. **Non-numeric facility distance:** At least one cleaned record contains the text value `far` in `Distance_to_Facility_km`, despite the field being intended as a distance in kilometres. Resolve this before numeric analysis.
3. **Missing values:** The cleaned worksheet still contains blank values in fields such as `Parity`, `ANC_Visits`, gestational/clinical measures and other columns. Quantify missingness and decide whether to retain, recode or exclude values for each analysis.
4. **Header consistency:** Some cleaned headers contain whitespace, including `Household_Income_Naira ` and `Length _of _Stay_Days`. Consider renaming these consistently in the next processing stage, while recording the mapping.
5. **Outcome interpretation:** The workbook reports 201 maternal-death outcomes and 2,362 survived outcomes among 2,563 cleaned records. This is a sample outcome split in simulated data, not a national maternal mortality rate.
6. **Power BI page label:** The report includes a page named `Page 2`. Review whether it should be renamed, completed or removed.

## Recommended cleaning log to complete

For reproducibility, record the following for every transformation:

| Step | Required documentation |
|---|---|
| Duplicate handling | Duplicate definition, number detected and number removed. |
| Missing values | Columns affected, counts, treatment and rationale. |
| Invalid values | Validation rule, affected records and treatment. |
| Category standardisation | Original labels, standard labels and mapping rules. |
| Date handling | Accepted formats, invalid dates and date range checks. |
| Derived columns | Formula or rule for each derived field. |
| Row exclusions | Record IDs or reproducible criteria and reason for exclusion. |

Do not describe a transformation as completed unless it is supported by the workbook, a formula, a query or a documented cleaning log.
