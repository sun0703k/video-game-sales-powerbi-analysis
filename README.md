# Video Game Sales Portfolio Analysis

End-to-end business analysis of historical video game sales using Python, Power BI and GenAI. The project evaluates genre and platform performance to support portfolio investment decisions.

## Business Question

Which genres and platforms should a video game publisher prioritize based on historical sales, hit rate, regional demand and portfolio risk?

## Dataset Scope

* Source: `vgsales.csv`
* Analysis period: 2012–2015
* Grain: One game-platform release record per row
* Analysis-ready records: 2,399
* Hit definition: Global Sales ≥ 1 million copies
* Sales values are reported in millions of copies

## Data Preparation

* Reviewed dataset grain and candidate keys
* Checked exact and business-level duplicates
* Removed one exact duplicate
* Kept the same game on different platforms as separate business records
* Did not impute missing release years because an estimated year could distort time-based analysis
* Validated Global Sales against the sum of regional sales
* Created an analysis-ready dataset for the 2012–2015 period

## Key Performance Indicators

| Metric             |    Result |
| ------------------ | --------: |
| Total Global Sales | 1,333.14M |
| Release Records    |     2,399 |
| Median Sales       |     0.15M |
| Successful Records |       317 |
| Hit Rate           |    13.21% |

## Key Insights

* Shooter had the highest historical hit rate at 32.45%, followed by Platform at 26.03% and Sports at 19.20%.
* Action generated the highest total global sales, but its hit rate was lower than Shooter.
* Shooter performance was strongest on PS4 and Xbox One within the reviewed sample.
* Action contributed the largest regional sales share in North America, Europe and Other markets.
* Role-Playing games were particularly important in Japan, contributing approximately 34% of regional sales.
* Genre performance was concentrated among top-selling releases, creating blockbuster-dependence risk.

## Business Recommendation

Prioritize Shooter titles for North America and Europe, especially on PS4 and Xbox One, while maintaining Action titles for portfolio scale. For Japan, evaluate a separate Role-Playing strategy because regional preferences differ significantly.

Investment decisions should not rely only on historical hit rate. Sample size, sales concentration, platform lifecycle, development cost and profitability should also be considered.

## Risks and Limitations

* The dataset represents historical records and may not reflect the complete market.
* Recent-year record counts drop sharply, suggesting incomplete coverage after 2016.
* Sales figures do not include development cost, marketing cost or profit.
* Platform-level Shooter estimates have relatively small samples and wide confidence intervals.
* Historical performance does not guarantee future success.

## Dashboard Features

* Executive KPI cards
* Year, Genre and Platform slicers
* Global Sales by Genre
* Hit Rate by Genre
* Global Sales by Year
* Shooter Hit Rate by Platform
* Sample-size filter for platform comparisons
* Executive summary with findings, recommendations and limitations

## Project Files

* [Python Analysis Notebook](./video-game-sales-analysis.ipynb)
* [Power BI Dashboard](./Video_Game_Portfolio_Dashboard.pbix)
* [Exported Dashboard Report](./video-game-sales-dashboard.pdf)

## Tools Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Google Colab
* Power BI
* DAX
* GenAI for code and communication review

## Author

Sunny Kumar
Aspiring Business Analyst / Data Analyst

