# Part I - Income and Health. What does the data say?
## by (Olubunmi Adejimi)


## Dataset


> This is a dataset of the Population growth, fertility, life expectancy and mortality for countries all over the world collected from https://data.un.org/. This data contains the following information:
* `Infant mortality for both sexes (per 1,000 live births)`,
* ` Life expectancy at birth for both sexes (years)`,
* `Life expectancy at birth for females (years)`,
* `Life expectancy at birth for males (years)`,
* `Maternal mortality ratio (deaths per 100,000 population)`,
* `Population annual rate of increase (percent)`,
* `Total fertility rate (children per women)`

> A second dataset from https://databank.worldbank.org/source/world-development-indicators containing the Gross National Income (GNI) per capita for the years 2010, 2015 and 2020, is combined with the previous dataset.

> These data are
 combined with a `GeoJSON` file collected from https://geojson-maps.ash.ms/, to have a more detailed dataset for a robust analyses.

> The following data wrangling steps were performed:
* Columns that were not necessary were dropped.
* The header names for the columns weere renamed.
* The GeoJSON file was imported and the required data were extracted from the file and passed as a dataframe.
* The un dataset and the geo data were merged into one.
* The `economy` column was cleaned to retain only the correct strings.
* the thousand separator were removed from specific column.
* The data types of a few columns were changed.
* Null values were replaced.
* Some inconsistent rows were dropped based on the `Year` column.
* A new column `Income level` was created using the GNI per capita column.



## Summary of Findings

> Sequel to exploring this dataset, we can conclude the following;
* More countries are categorized as `High income `and the least number of countries as `low income`.
* More countries have lower infant and maternal mortality rate, population increase rate and higher life expectancy.
* Developed countries have the lowest rate of population growth, which appears to be related to the low fertility rate in developed countries. Africa has the highest fertility rate and annual population increase rate and is predominantly a `low income` economy.
* There has been a drop in the annual rate of population increase between 2010 and 2020, with Asia experiencing the most reduction in rate of population increase and South America has seen an uptrend in the rate of population increase.
* There is a strong correlation between maternal mortality and infant mortality, indicating that a child whose mother dies is likely to survive, especially in least developed economies like Africa.
* While the African continent and `low income` economies show poor data in terms of mortalities and life expectancies, they also have the highest improvements in these aspects. This is an indication of improved health and healthcare.
* The high fertility rate in the African continent and 'least developed economies, indicates that the population is younger which can be beneficial towards improvement the economy and overall livelihood and health of its citizens.


## Key Insights for Presentation


> Maternal health and infant health suffers in the least developed countries. This highlights the need for improved healthcare and economic development to help improve this the health of infant and mothers.
> Being a wealthy individual or country increases life expectancy. This may be due to better access to healthcare and better quality of life due to higher income levels.