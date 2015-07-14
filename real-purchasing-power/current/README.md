# Real Purchasing Power in US Metropolitan Areas in 2013

Using [Bureau of Economic Analysis data](http://www.bea.gov/newsreleases/regional/rpp/rpp_newsrelease.htm), these compiled data show real purchasing power at the metropolitan level. The BEA provides data on both the regional price parity (RPP) of [individual metropolitan areas](http://en.wikipedia.org/wiki/List_of_Metropolitan_Statistical_Areas), and the RPP averages of metropolitan and non-metropolitan counties in a state. These two sets are included (`bea-data-metro-areas-rpp-2013.csv` and `bea-data-metro-vs-non-metro-rpp-2013.csv`, respectively) and combined. We further break the data down and assign values at the county level depending on which metropolitan or non-metropolitan area a given county belongs to. Data for individual metropolitan areas are applied to all counties comprising that metro area, [as specified by the U.S. Census Bureau](https://www.census.gov/population/metro/files/lists/2009/List1.txt). All non-metropolitan counties in a state are assigned the state's non-metropolitan average. The BEA's RPP values are converted to dollar equivalents to express the real value of $100 in each measured location compared to the national average. The goal of combining these datasets is to show not just differences between metropolitan and non-metropolitan areas within states, but also between multiple metropolitan areas within a state.

![The Real Value of $100 in Metropolitan Areas, 2013](http://taxfoundation.org/sites/taxfoundation.org/files/%24100%20Metro%20Map-03.png)

## Explanation of Data

| Name | Description |
| --- | --- |
| `state` | The [FIPS code](https://www.census.gov/geo/reference/docs/state.txt) identifying the state in each record. |
| `county` | The [FIPS code](https://www.census.gov/geo/reference/codes/files/national_county.txt) identifying the county in each record. |
| `cbsa` | The numerical ID for a given metropolitan statistical area, if available` |
| `rpp-in-100-dollars` | The real value of $100 in each record adjusted by the regional price parity from the BEA. |
| `name` | The name of the metropolitan area this county belongs to, or an indication that the record describes the average of all non-metropolitan areas for that state. |

## Additional Resources

* [Tax Foundation: The Real Value of $100 in Metropolitan Areas 2013](http://interactive.taxfoundation.org/rpp2013/)
* [Bureau of Economic Analysis: Real Personal Income for States and Metropolitan Areas, 2013](http://www.bea.gov/newsreleases/regional/rpp/rpp_newsrelease.htm)
