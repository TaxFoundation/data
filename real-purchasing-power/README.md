# Real Purchasing Power in US Counties in 2012

Using [Bureau of Economic Analysis data](http://www.bea.gov/newsreleases/regional/rpp/rpp_newsrelease.htm), these compiled data show real purchasing power at the county level. The BEA provides data on both the regional price parity of [individual metropolitan areas](http://en.wikipedia.org/wiki/List_of_Metropolitan_Statistical_Areas), and the RPP averages of metropolitan and non-metropolitan counties in a state. These two sets are included (`bea-data-metro-areas-rpp-2012.csv` and `bea-data-metro-vs-non-metro-rpp-2012.csv`, respectively) and combined. Data for individual metropolitan areas are applied to all counties comprising that metro area. All non-metropolitan counties in a state are assigned the state's non-metropolitan average. The BEA's RPP values are converted to dollar equivalents to express the real value of $100 in each measured location compared to the national average. The goal of combining these datasets is to show not just differences between metropolitan and non-metropolitan areas within states, but also between multiple metropolitan areas within a state.

## Explanation of Data

| Name | Description |
| --- | --- |
| `id` | The [ANSI code](https://www.census.gov/geo/reference/codes/files/national_county.txt) identifying the county in each record. |
| `state` | The [ANSI code](https://www.census.gov/geo/reference/docs/state.txt) identifying the state in each record. |
| `regionalPriceParity` | BEA data describing the price level of goods and services compared to the overall national price level of 100. |
| `purchasingPower` | The real value of $100 in each record adjusted by the regional price parity from the BEA. |
| `metroName` | The name of the metropolitan area this county belongs to, or an indication that the record describes the average of all non-metropolitan areas for that state. |

## Additional Resources

* [Tax Foundation: The Real Value of $100](http://taxfoundation.org/blog/real-value-100-each-state)
* [Bureau of Economic Analysis: Real Personal Income for States and Metropolitan Areas, 2008-2012](http://www.bea.gov/newsreleases/regional/rpp/rpp_newsrelease.htm)