# Reducing Maternal Mortality in Nigeria: An End-to-End Data Analytics Project

This project explores patterns in a simulated maternal health dataset using Excel and Power BI, with SQL and Python analysis planned as the next stages.

> **Data notice:** The dataset used in this project is simulated for learning and portfolio demonstration. It is not official Nigerian maternal mortality data, hospital records, or clinical evidence. Findings should not be interpreted as population estimates or causal conclusions.

## Project question

What patterns in antenatal care attendance, delivery conditions, facility access, and patient demographics are associated with maternal outcomes in this dataset, and what data-informed interventions could be explored?

## Project workflow and status

| Stage | Status | Work |
|---|---|---|
| Excel | Completed draft | Data cleaning, exploratory summaries, PivotTables, KPIs and dashboard |
| SQL | Planned | Database design, data preparation and analytical queries |
| Power BI | Completed draft | Interactive report with maternal-death and patient-analysis pages, plus a third page requiring review |
| Python | Planned | Exploratory analysis, statistical analysis and predictive modelling |

## Dataset overview

The supplied workbook contains an original dataset sheet and a cleaned dataset sheet. The project notes record 2,600 original rows and 2,563 cleaned rows. The cleaned table includes demographic, antenatal, delivery, referral, clinical measurement, outcome and socioeconomic fields. See [`documentation/data_dictionary.md`](documentation/data_dictionary.md) and [`documentation/data_quality_and_cleaning_notes.md`](documentation/data_quality_and_cleaning_notes.md).

## Repository structure

```text
.
├── README.md
├── excel/
│   └── maternal_mortality_analysis.xlsx
├── power-bi/
│   └── maternal_mortality_dashboard.pbix
├── sql/                 # Planned SQL work
├── python/              # Planned Python work
├── reports/             # Final report and supporting outputs
└── documentation/
    ├── data_dictionary.md
    └── data_quality_and_cleaning_notes.md
```

## Tools

- Microsoft Excel: cleaning, summaries, PivotTables and dashboarding
- Power BI: interactive visual analysis
- SQL: planned database querying stage
- Python: planned statistical and predictive analysis stage

## Important interpretation limits

- The dataset is simulated; it cannot establish the real burden or geographic distribution of maternal mortality in Nigeria.
- Associations observed in this dataset do not establish causation.
- Predictive performance, if developed later, would apply only to this simulated dataset unless validated against suitable real-world data under appropriate governance.
- Clinical decisions must not be based on this portfolio analysis.

## Collaboration and learning context

Prepared as a portfolio project in the context of the 2026 NECA/ITF-TSDP Data Analytics Training Programme, in collaboration with Shamzbridge Consult.

## Current next steps

1. Review unusual or invalid values in the cleaned workbook, including the recorded ANC visit value of 99 and the non-numeric distance value `far`.
2. Review and rename the generic third Power BI report page if appropriate.
3. Complete the SQL stage and document the queries and outputs.
4. Complete the Python stage and document the methods, limitations and results.

## Author

Samson Bukola Oguntade  
GitHub: [@Tade-2309](https://github.com/Tade-2309)
