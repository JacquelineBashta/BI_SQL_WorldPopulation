# BI_SQL_WorldPopulation_2022
Analysis regarding the growth rate for the world population using SQL

## Source
The data is collected from the original CIA source for year 2022 [Here](https://www.cia.gov/the-world-factbook/about/archives/2022/references/guide-to-country-comparisons/)

---------------------
## Data Structure
The columns collected are:
- area : total area of the country (area_water + area_land).
 - population : population of the country
 - population_growth : ratio of the population growth in 2015
 - birth_rate
 - death_rate
 - net_migration_rate : ratio of people that left the country to another.

Additionally following columns added extra
 - id : id number attribuated to a country.
 - code : country code, made from the two first letters of the country.

--------------------
## Procedure
### a. From Site to 1 db
first each column is downloaded from website as separate .csv file
then pandas is used to merge all of them to on table

### b. Store and explore db
then the created table is saved in Rational db.
The created db is then explored via SQL language.