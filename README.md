# F1 Driver Performance Analysis --- 2025 Season

A data-driven analysis of Formula 1 driver performance beyond
championship points, using **FastF1, Python, Pandas, and Power BI**.

## Project Overview

Formula 1 driver performance cannot be fully understood through
championship points alone. This project analyzes the 2025 season using
race and qualifying data to compare drivers across several dimensions,
including race results, qualifying performance, consistency, and
reliability.

The workflow covers data collection, cleaning, validation, metric
calculation, weighted scoring, and interactive visualization in Power
BI.

## Objectives

-   Analyze driver performance throughout the 2025 season.
-   Compare race and qualifying performance.
-   Measure consistency and reliability.
-   Examine qualifying-to-race position changes.
-   Create a weighted Overall Performance Score.
-   Present the results in an interactive Power BI dashboard.

## Tools and Technologies

-   **FastF1** --- retrieve Formula 1 session data.
-   **Python** --- data extraction and processing.
-   **Pandas** --- cleaning, transformation, aggregation, and analysis.
-   **Matplotlib** --- data visualization where used.
-   **Power BI** --- interactive dashboard and reporting.

## Workflow

`FastF1 → Python → Pandas → Data Cleaning & Validation → Analysis → CSV Files → Power BI`

## Performance Metrics

The project uses eight metrics:

1.  Total Points
2.  Win Rate
3.  Podium Rate
4.  Average Finish Position
5.  Finish Consistency
6.  DNF Rate
7.  Average Qualifying--Race Gap
8.  Average Qualifying Position

## Overall Performance Score

The metrics are converted to comparable scores and combined using a
weighted scoring model.

  Metric                             Weight
  ------------------------------ ----------
  Total Points                          25%
  Win Rate                              15%
  Podium Rate                           15%
  DNF Rate                              15%
  Average Finish Position               10%
  Average Qualifying--Race Gap          10%
  Average Qualifying Position            5%
  Finish Consistency                     5%
  **Total**                        **100%**

The score is intended to compare several aspects of performance rather
than relying on championship points alone. Different weighting choices
may produce different rankings.

## Power BI Dashboard

The dashboard contains five report pages:

-   **Season Rankings** --- championship standings and season summary.
-   **Driver Performance** --- individual performance and positions
    gained.
-   **Reliability Analysis** --- DNF rates and race-completion
    reliability.
-   **Season Trends** --- changes in performance across the season.
-   **Overall Performance** --- comparison of the weighted Overall
    Performance Score and its component metrics.

> **Dashboard screenshots:** Add screenshots of your report pages here
> so visitors can preview the dashboard directly on GitHub.

Example:

``` markdown
![Season Rankings dashboard](screenshots/season-rankings.png)
```

## Data Cleaning and Validation

The data preparation process included:

-   Checking missing values and investigating session-specific cases.
-   Standardizing driver names, abbreviations, and identifiers.
-   Reviewing non-standard race classifications, such as retirements and
    disqualifications.
-   Validating session counts, driver counts, duplicate records, column
    names, data types, and race-by-race record counts.

## Key Findings

The analysis is designed to help explore these questions:

-   How do rankings change when multiple performance metrics are
    considered instead of points alone?
-   How do qualifying results compare with race finishes?
-   Which drivers show stronger consistency or reliability?
-   How do the selected metrics contribute to each driver's Overall
    Performance Score?

Use the dashboard and underlying data to verify and present specific
numerical findings.

## Limitations

-   Results are influenced by car and team competitiveness; the scoring
    model does not fully isolate driver skill.
-   The score depends on the selected metrics and their assigned
    weights.
-   Lap pace, tyre management, pit-stop performance, overtaking, and
    sector performance are not fully represented.
-   Formula 1 session data can include missing values and special
    classifications that require careful handling.

## Future Improvements

-   Lap-time and pace analysis.
-   Tyre compound and degradation analysis.
-   Pit-stop performance analysis.
-   Overtaking and position-change analysis.
-   Circuit-specific comparisons.
-   Team-adjusted driver performance.
-   More advanced statistical analysis.
-   Automated updates for future seasons.

## Repository Contents

Update this list to match the files you actually upload:

``` text
F1-Driver-Performance-Analysis/
├── data/              # Cleaned CSV datasets
├── notebooks/         # Python analysis notebook(s)
├── powerbi/           # Power BI report (.pbix)
├── screenshots/       # Dashboard screenshots
├── presentation/      # Project presentation
└── README.md
```

## How to Explore the Project

1.  Review the dashboard screenshots in `screenshots/`.
2.  Open the Power BI `.pbix` file in Power BI Desktop to explore the
    report.
3.  Review the notebook(s) to understand the data collection, cleaning,
    and analysis workflow.
4.  Check the CSV files to inspect the processed data.

## Author

**Surya Mani Deep**

------------------------------------------------------------------------

*This project is for educational and portfolio purposes. Review the
source data, metric definitions, and scoring assumptions when
interpreting the results.*
