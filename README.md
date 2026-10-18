# Marketing-Campaign-Performance-Data-Analysis

## Project Overview

This project explores marketing campaign performance using Python and
Power BI. The goal is to analyze revenue, conversions, leads,
acquisition cost, channel performance, customer segments, engagement,
and trends over time.

## Objectives

-   Compare revenue across marketing channels.
-   Evaluate conversions by campaign type.
-   Understand the conversion funnel from impressions to clicks, leads,
    and conversions.
-   Explore monthly revenue trends.
-   Compare acquisition cost and cost per conversion.
-   Examine customer segments and engagement patterns.
-   Build an interactive Power BI dashboard to communicate findings.

## Tools & Technologies

-   **Python** --- data analysis
-   **Pandas** --- data manipulation and aggregation
-   **Matplotlib** --- visualizations in Python
-   **Power BI Desktop** --- interactive dashboard and KPI reporting
-   **Jupyter Notebook** --- analysis workflow

## Dataset

The dataset includes fields such as: `Campaign_ID`, `Campaign_Type`,
`Target_Audience`, `Duration`, `Channel_Used`, `Impressions`, `Clicks`,
`Leads`, `Conversions`, `Revenue`, `Acquisition_Cost`, `ROI`,
`Language`, `Engagement_Score`, `Customer_Segment`, and `Date`.

> Note: Confirm the meaning and units of Revenue, Acquisition_Cost, and
> ROI before interpreting or publishing financial conclusions.
> `Campaign_ID` should not automatically be assumed to represent a
> unique campaign without checking the dataset's definition.

## Analysis Workflow

1.  Load and inspect the dataset in Python.
2.  Clean data types and prepare the date field.
3.  Explore overall metrics such as revenue, leads, conversions, and
    acquisition cost.
4.  Analyze performance by channel and campaign type.
5.  Calculate funnel rates:
    -   Click-through rate (CTR) = Clicks / Impressions × 100
    -   Click-to-lead rate = Leads / Clicks × 100
    -   Lead-to-conversion rate = Conversions / Leads × 100
6.  Explore monthly revenue trends, customer segments, and engagement.
7.  Compare cost per conversion where the cost definition supports the
    calculation.
8.  Build a Power BI dashboard with KPI cards, charts, filters, and a
    key-insights section.

## Power BI Dashboard

The dashboard is designed to include: - Total Revenue - Total
Conversions - Total Leads - Total Acquisition Cost - Average ROI
(subject to validation of the metric definition) - Revenue by Channel -
Conversions by Campaign Type - Revenue by Engagement Score - Monthly
Revenue by Channel - Conversion Funnel - Cost per Conversion by
Channel - Customer Segment analysis - Key Insights and a detailed table

## Key Metrics

-   **CTR (%)** = Clicks ÷ Impressions × 100
-   **Click-to-Lead (%)** = Leads ÷ Clicks × 100
-   **Lead-to-Conversion (%)** = Conversions ÷ Leads × 100
-   **Cost per Conversion** = Total Acquisition Cost ÷ Total
    Conversions, only if Acquisition_Cost is an additive cost measure
    aligned with the conversions.

## Important Validation Notes

Before sharing the dashboard publicly: - Ensure Python and Power BI use
the same cleaned dataset and filters. - Compare revenue totals by
channel between Python and Power BI. - Check monthly totals for
incomplete months, missing dates, or unexpected drops. - Avoid summing
ROI values. Confirm the correct definition before displaying an average
or overall ROI. - Validate all Key Insights against the final charts and
calculations. - Format large values consistently (for example, K or M)
and ensure funnel labels are readable.

## Repository Structure

``` text
marketing-campaign-performance-analysis/
├── data/
│   └── marketing_campaign_cleaned.csv
├── notebooks/
│   └── marketing_campaign_analysis.ipynb
├── powerbi/
│   └── Marketing_Campaign_Performance.pbix
├── images/
│   └── dashboard.png
└── README.md
```

*The filenames above are suggested. Update them to match the files
included in your repository.*

## Results

Add validated findings here after checking the final calculations.
Examples of useful findings include: - Highest-revenue marketing
channel - Campaign type with the most conversions - Lowest cost per
conversion - Customer segment with the highest revenue - Months with
notable increases or decreases

Do not publish example values as final results until they have been
verified against the dataset.

## How to Run

1.  Clone or download this repository.

2.  Open the Jupyter Notebook in `notebooks/`.

3.  Install the required Python libraries if needed:

    ``` bash
    pip install pandas matplotlib jupyter
    ```

4.  Update the data path in the notebook to point to the CSV file in
    `data/`.

5.  Open the `.pbix` file in Power BI Desktop to explore the dashboard.

## Author

Nada Mohamed Rashid
https://www.linkedin.com/in/nada-mohammed-95bb05263
