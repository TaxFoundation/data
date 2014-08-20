# World Corporate Tax Rates 1993-2014

This dataset compiled by the Tax Foundation lists known top marginal general corporate income tax rate for countries and equivalent taxing authories and GDP for the years 1993 to 2014. As of publication, these data are incomplete. Corporate tax rate and GDP totals have not been found by the Tax Foundation for all countries. We are continuing to build this dataset and welcome any new sources of information.

GDP numbers are from the [Department of Agriculture’s International Macroeconomic Dataset](http://www.ers.usda.gov/data-products/international-macroeconomic-data-set.aspx#.U_SlPfldVMc). All values in 2005 U.S. dollars.

## Explanation of Data

Note: These data are UTF-8 encoded. Country names with special characters (e.g., the Åland Islands) may not be read correctly in Excel. To get around this, open the file in Excel by going to Data -> Get External Data -> From Text. Select the downloaded CSV, and set `File origin:` to `65001 : Unicode (UTF-8)`.

| Name | Description |
| --- | --- |
| `id` | [ISO 3166-1 numeric](http://en.wikipedia.org/wiki/ISO_3166-1_numeric) codes used to identify countries. |
| `year` | The year in which a given country had rates/GDP of the stated level. |
| `country` | The name of the country in the record. |
| `corporateTaxRate` | The corporate tax rate for a given country in a given year. These data are incomplete. |
| `region` | The geographic region of a given country. |
| `oecd` | `Boolean` representing whether or not the country is an OECD member as of 2014. |
| `gseven` | `Boolean` representing whether or not the country is a G7 member as of 2014. |
| `gtwenty` | `Boolean` representing whether or not the country is a G20 member as of 2014. |
| `brics` | `Boolean` representing whether or not the country is a BRICS nation (Brazil, Russia, India, China, and South Africa). |
| `eu` | `Boolean` representing whether or not the country is member of the European Union as of 2014. |
| `gdp` | The Gross Domestic Product of the nation in the year of the record. |


## Additional Resources

* [OECD](http://www.oecd.org/tax/tax-policy/tax-database.htm)
* [PwC](http://www.pwc.com/gx/en/tax/corporate-tax/worldwide-tax-summaries/downloads.jhtml)
* [Deloitte](https://dits.deloitte.com/#TaxGuides)
* [Ernst and Young Worldwide Corporate Tax Guide](http://www.ey.com/GL/en/Services/Tax/Global-tax-guide-archive)