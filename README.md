# EdTech Startup Analysis Dashboard — Power BI Business Intelligence Report

An end-to-end business intelligence project focused on analyzing startup and EdTech business data using Power BI. The project converts raw data into meaningful insights using data modeling, DAX calculations, and interactive dashboard visualizations.

* * *

## Project Objective

The education technology industry is rapidly growing with startups competing in various domains such as online learning, skill development, certification programs, and digital education platforms.

The objective of this project is to:

• Analyze startup growth trends

• Study funding patterns

• Identify top-performing sectors

• Understand customer and business behavior

• Generate actionable insights through dashboard visualizations

* * *

## Table of Contents

- Business Context
- Business Questions
- Headline Results
- Data Sources
- Data Cleaning and Transformation
- Data Modeling
- Calculated Measures
- Dashboard Outputs
- Insights
- Recommendations
- Repository Structure
- Tools and Technologies

* * *

## Business Context

EdTech startups operate in a highly competitive environment where growth, funding, customer acquisition, and business performance determine long-term success.

Business teams need insights into:

- Funding performance
- Startup growth
- Category analysis
- Customer behavior
- Market trends

* * *

## Business Questions

| Theme | Question |
|---------|----------|
| Startup Analysis | Which startup categories attract maximum users? |
| Funding Analysis | Which startups received the highest funding? |
| Growth Analysis | Which startup shows the highest growth trend? |
| Customer Analysis | Which customer segment contributes the most? |
| Market Analysis | Which sectors dominate the market? |

* * *

## Headline Results

| Metric | Value |
|----------|--------|
| Total Startups | 1000+ |
| Total Funding | $500M |
| Active Users | 250K |
| Growth Rate | 18% |
| Categories | 15 |

* * *

## Data Sources

The dashboard includes:

| Table | Description |
|---------|-------------|
| Startup Data | Startup details |
| Funding Data | Funding records |
| Users Data | Customer information |
| Category Data | Startup category details |
| Date Table | Time intelligence calculations |

* * *

## Data Cleaning and Transformation

The following transformations were performed:

• Removed duplicate records

• Handled null values

• Standardized columns

• Created calculated columns

• Built date hierarchy

• Established relationships

* * *

## Data Modeling

Star schema model used:

- FactStartupData
- Funding Dimension
- User Dimension
- Category Dimension
- Date Dimension

Relationship Type:

One-to-many relationships

* * *

## Calculated Measures

**Total Funding**

```DAX
SUM(Funding[Amount])
```

**Total Users**

```DAX
COUNT(Users[UserID])
```

**Average Funding**

```DAX
DIVIDE(
SUM(Funding[Amount]),
COUNT(Startup[StartupID])
)
```

**Growth Rate**

```DAX
DIVIDE(
[CurrentYearUsers]-[PreviousYearUsers],
[PreviousYearUsers]
)
```

## Dashboard Outputs

Dashboard includes:

1. KPI Cards

2. Startup Growth Analysis

3. Funding Trend Analysis

4. Category Analysis

5. User Segmentation

6. Interactive Filters

7. Business Insights Page

Dashboard Preview:

![EdTech Dashboard](Dashboard.png)

* * *

## Insights

The analysis highlighted the following findings:

• Certain startup categories attracted the largest user base

• Funding increased significantly over recent periods

• Customer growth showed positive trends

• Top startups contributed a major share of revenue

• Market concentration was observed in a few categories

* * *

## Recommendations

• Invest more resources in high-growth categories

• Focus on customer retention strategies

• Improve marketing efforts in underperforming segments

• Monitor startup performance regularly

* * *

## Repository Structure

EdTech-Startup-Analysis/

├── README.md

├── report/

│ └── EdTechDashboard.pbix

├── outputs/

│ └── Dashboard.png

├── documents/

│ └── Dashboard.pdf

* * *

## Tools and Technologies

• Microsoft Power BI

• Power Query

• DAX

• Data Modeling

• Data Visualization

* * *

If you found this project useful, consider starring the repository ⭐
