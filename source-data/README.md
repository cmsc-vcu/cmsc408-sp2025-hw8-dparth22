# CMSC 408 - Homework 8: World Bank Data Analysis

## Overview

This assignment involved exploring and analyzing data from the World Bank’s World Development Indicators. Using SQL and Python (via Quarto), I created a data pipeline and queried data to uncover patterns in global economic indicators.

We worked with three main tables:

- `wdi_country`: Information about countries and regions.
- `wdi_series`: Metadata about available indicators.
- `wdi_data`: Actual indicator values across years and countries.

## Tasks Completed

- Wrote and executed SQL queries using aggregation, filtering, grouping, ordering, subqueries, case statements, and joins.
- Identified unique regions, country counts per region, income classifications, and explored edge cases like missing income data.
- Created a copy of the `wdi_country` table in my own schema.
- Fixed an income classification issue (Qatar).
- Built summary tables and percent-based breakdowns.
- Answered challenge tasks like generating all missing region-income group pairs.

## Skills Practiced

- SQL: `SELECT`, `GROUP BY`, `ORDER BY`, `CASE`, `WITH`, `JOIN`, subqueries
- Python + Pandas: Loading and cleaning CSVs, database connections
- Quarto: Reporting and documentation

## Setup

1. Data loaded from the [World Bank WDI ZIP](https://databank.worldbank.org/data/download/WDI_CSV.zip).
2. `loader.qmd` used to unzip, process, and populate MySQL tables.
3. `.env` file used for secure database credentials.
4. Queries run against both `world_bank_data` (read-only) and a local copy of `wdi_country` in my schema.

## Notes

- All queries were run using Python’s `sqlalchemy` and helper functions.
- Tables and results were rendered within a Quarto HTML report.
- Reflections on challenges, learnings, and strategies are included in the final section of the report.
