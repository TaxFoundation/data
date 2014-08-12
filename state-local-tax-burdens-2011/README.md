# State and Local Tax Burdens in Nominal Dollars from 1977 to 2011

These data accompany the Tax Foundation's report [Annual State-Local Tax Burden Rankings FY 2011](http://taxfoundation.org/article/annual-state-local-tax-burden-ranking-fy-2011) by [Liz Malm](http://taxfoundation.org/staff/liz-malm) and [Gerald Prante](http://www.lynchburg.edu/content/gerald-prante). They are the product of analyzing data from government and public policy sources. This report estimates the combined state and local tax burden shouldered by the residents of each of the fifty states, regardless of the jurisdictions to which those taxes are paid. The burden is calculated as the total taxes paid by state residents to any tax jurisdiction divided by the per capita income of that state. [View full Explanation of methodology.](http://taxfoundation.org/article/tax-foundation-state-local-tax-burden-estimates-overview-methodology)

## Explanation of Data

Dollars in this data are nominal. Inflation-adjusted data is available [here](http://taxfoundation.org/article/state-and-local-tax-burdens-all-years-one-state-1977-2011), calculated with the Consumer Price Index - All Urban Consumers, annual measure (1977-2011). The data begin with summary records for the United States as a whole, with averages weighted by population.

| Name | Explanation |
| --- | ---: |
| `id` | The [ANSI code](https://www.census.gov/geo/reference/docs/state.txt) identifying the state in each record. Summary data for the United States as a whole uses the id `0`. |
| `location` | The name of the state described in the record. |
| `burden` | The estimated tax burden on residents of a state in a given year, equal to `taxesPaidTotal` divided by `incomePerCapita`. |
| `rank` | Ranking of a state's tax burden relative to other states in a given year. United States summary data has no `rank` value. The District of Columbia is not technically ranked in this report as it is not a state; however, rankings are provided for DC to show where it would fall if it were a state. |
| `taxesPaidToOwnState` | Per capita taxes paid by residents of a state to their own state and local governments. |
| `taxesPaidToOtherStates` | Per capita taxes paid by residents of a state to other state and local governments. |
| `taxesPaidTotal` | Sum of `taxesPaidToOwnState` and `taxesPaidToOtherStates`. |
| `incomePerCapita` | Per capita income for residents of a state. |

## Additional Information

* [Latest release of Annual State-Local Tax Burden Rankings](http://taxfoundation.org/burdens)
* [Methodology for Burdens Report](http://taxfoundation.org/burdensmethodology)
* [Tool for extracting specific parts of dataset](http://taxfoundation.org/article/state-and-local-tax-burdens-all-years-one-state-1977-2011)