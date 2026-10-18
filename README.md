# COVID-19 Global Impact Dashboard

## Project Overview
An interactive Microsoft Power BI dashboard for exploring country-level COVID-19 cases, deaths, vaccination data, and trends over time. The report uses a green-and-white visual theme.

## Dashboard Features
- KPI cards for total cases, highest country deaths, countries covered, and people vaccinated.
- Daily reported COVID-19 cases trend.
- Top 10 countries by cases.
- Country comparison by deaths.
- Cases by continent donut chart.
- Date-range and continent slicers.

## Tools
Microsoft Power BI Desktop, DAX, CSV dataset.

## Dataset
The cleaned dataset is included under `data/processed/` and `data/raw/` when available. The source data is country-level and contains daily COVID-19 indicators. Vaccination fields may have missing values.

## Build / Open
1. Open `dashboard/COVID_19_Global_Impact_Dashboard.pbix` in Power BI Desktop.
2. If the PBIX file is not there yet, open your existing report in Power BI Desktop and use **File → Save As** to save it at that path.
3. If Power BI asks to locate the dataset, select `data/processed/covid_cleaned.csv`.
4. Check that the date and continent slicers filter the visuals as expected.

## Data interpretation notes
- Use daily `new_cases` for daily trend visuals, not the sum of cumulative `total_cases` over every date.
- For country rankings and continent comparisons based on cumulative cases, use a latest-available-per-country snapshot to avoid repeatedly summing cumulative totals across dates.
- The donut total is the sum of latest available country-level records represented in the visual; it is not automatically an official global total.
- Vaccination data may be incomplete. Validate its definition and coverage before presenting it as a complete global count.

## Suggested submission contents
- Power BI `.pbix` report (save it into `dashboard/`)
- Dashboard screenshot (save it into `reports/`)
- This README
- Dataset, if allowed by the internship submission rules

## Author
Add your name, internship/program name, and submission date before publishing.
