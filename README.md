# NYC Airbnb Price Analysis

This project analyzes NYC Airbnb listings to understand how price varies by borough, room type, ZIP code, review activity, and listing quality.

## Interactive Dashboard

[View the Tableau Public dashboard](https://public.tableau.com/views/AirbnbProject_17798582505110/Dashboard1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Project Objective

The goal was to clean and analyze Airbnb listing data, then build a dashboard that answers practical pricing questions:

- Which boroughs have the highest Airbnb prices?
- How does room type affect price?
- Do luxury listings raise the overall average?
- Do review patterns relate to pricing?
- Which ZIP codes appear most expensive?
- How much of the data is missing or questionable?

## Tools Used

- Excel
- Power Query
- PivotTables
- Tableau Public

## Data Cleaning Summary

The original dataset was cleaned in Excel before being loaded into Tableau. Cleaning steps included:

- Standardized column names
- Converted ZIP code to text
- Converted price, beds, review count, and review score fields to numeric values
- Created `Rating_Status` to identify missing ratings
- Created `Review_Status` and `Review_Bucket` fields
- Created `Price_Bucket` for Budget, Mid, Premium, and Luxury listings
- Flagged high-price outliers
- Removed or reviewed invalid records
- Documented cleaning steps in a cleaning log

## Key Findings

- Manhattan had the highest average price among major boroughs.
- Entire homes/apartments were far more expensive than private or shared rooms.
- Luxury listings raised the overall average price, making median price an important comparison point.
- A meaningful share of listings had missing ratings, so rating-based conclusions should be treated carefully.
- ZIP-code-level pricing showed clear geographic variation across NYC.

## Repository Structure

```text
data/
  airbnb_clean_tableau.csv

docs/
  data_dictionary.md

README.md
```

## Notes

This repo documents the cleaned dataset and analysis workflow. The final interactive visualization is hosted on Tableau Public.
