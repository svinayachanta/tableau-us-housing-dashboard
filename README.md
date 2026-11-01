# Homequest

A Tableau dashboard for choosing a US state or city to buy a house. The question is which place has the more favorable mix of price, crime, and unemployment.

Open `tableau-us-housing.twbx` in Tableau Desktop or Tableau Public. The workbook already contains the data. The three CSVs are the same tables, kept here so the sources are readable.

## Who it is for

A buyer or a small investor who wants one place to compare states before picking one. The dashboard is exploratory: maps and charts to compare, not a single recommended city.

## Data

| File | What it is | Source |
| --- | --- | --- |
| `datasets/houses.csv` | Average house price by state and city, 2000–2023 | [Zillow Research](https://www.zillow.com/research/data/) |
| `datasets/crime.csv` | State crime rates, 1960–2019 | [CORGIS state crime](https://corgis-edu.github.io/corgis/csv/state_crime/) |
| `datasets/unemployment.csv` | State unemployment, 1980–2023 | [Iowa State ICIP](https://www.icip.iastate.edu/tables/employment/unemployment-states) and the [Bureau of Labor Statistics](https://www.bls.gov/lau/lastrk18.htm) |

Cleaning was mostly state names and state codes so the three tables can share a map, plus date columns that Tableau had read as numbers.

## What the dashboard shows

- A map of average house price. Orange marks the high-price cities.
- A line of price over time for the state or city you select.
- Bars for unemployment by state.
- Several lines for crime types over time.

The written read of those views, from August 2023: California's average price rises from about $234k in 2000 to $1,000k or more in 2023, unemployment there is about 4.5%, and crime rates are lower than in the 1990s. High population and a price-to-rent ratio are the reasons that write-up treats California as the standout market.

Lifestyle, school quality, and healthcare are not in the data. Those were left as a later addition.
