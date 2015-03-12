# Facts and Figures 2015

Published March 10, 2015.

## Notes

These data are in the process of being cleaned and added to Tax Foundation's data repository.

### Tax Freedom Day 2014

Tax Freedom Day is the day when the nation as a whole has earned enough money to pay off its total tax bill for the year. Tax Freedom Day provides Americans with an easy way to gauge the overall tax take-a task that can otherwise be daunting due to the multiplicity of taxes at various levels of government and "hidden" taxes and fees that are often buried in the cost of living. Tax Freedom Day computed by dividing total tax collections by the nation's income, as reported by the Bureau of Economic Analysis. Every dollar that is officially called income by the government is counted, and every payment that is officially considered a tax is counted. The resulting percentage is then converted into days of a 365-day calendar year.

These data include the date of `taxFreedomDay` as [ISO 8601](http://en.wikipedia.org/wiki/ISO_8601) dates and the `rank` from earliest to latest.

### State-Local Tax Burdens

These data accompany the Tax Foundation's report [Annual State-Local Tax Burden Rankings FY 2011](http://taxfoundation.org/article/annual-state-local-tax-burden-ranking-fy-2011) by [Liz Malm](http://taxfoundation.org/staff/liz-malm) and [Gerald Prante](http://www.lynchburg.edu/content/gerald-prante). They are the product of analyzing data from government and public policy sources. This report estimates the combined state and local tax burden shouldered by the residents of each of the fifty states, regardless of the jurisdictions to which those taxes are paid. The burden is calculated as the total taxes paid by state residents to any tax jurisdiction divided by the per capita income of that state. [View full explanation of methodology.](http://taxfoundation.org/article/tax-foundation-state-local-tax-burden-estimates-overview-methodology)

To see more complete data going back to 1977, see [here](https://github.com/TaxFoundation/data/tree/master/state-local-tax-burdens).

### State Indvidual Income Tax Rates

These data summarize state-level marginal income tax rates for US individuals as of January 1, 2015. Dollar amounts listed are in nominal dollars. These rates are not effective rates, i.e. they are not adjusted to account for exemptions.

#### Explanation of Data

| Name | Description |
| --- | --- |
| `id` | The [ANSI code](https://www.census.gov/geo/reference/docs/state.txt) identifying the state in each record. |
| `stateAbbr` | The [ANSI code](https://www.census.gov/geo/reference/docs/state.txt) abbreviation for the state in each record. |
| `stateName` | The full name of the state in each record. |
| `incomeTaxRate` | The marginal rate applied to income equal to or greater than `incomeGreaterThan`, but not above `incomeNotGreaterThan`. |
| `incomeGreaterThan` | Income above this amount is taxed at the accompanying `incomeTaxRate`, up to `incomeNotGreaterThan`. Values are in nominal dollars. |
| `incomeNotGreaterThan` | Upper limit to the amount of income taxed at a particular marginal `incomeTaxRate`. Values are in nominal dollars. |

#### Notes on State Individual Income Tax Rates:

Brackets are for single taxpayers. Some states double bracket widths for joint filers (Ala., Ariz., Calif., Conn., Hawaii, Idaho, Kans., La., Nebr., Ore.). N.Y. doubles all except the 6.85% bracket. Some states increase but do not double brackets for joint filers (Ga., Maine, Minn., N.M., N.D., Okla., R.I., Vt., Wis.). Md. increases some but not all brackets. N.J. adds a 2.45% rate and doubles some bracket widths. Consult TaxFoundation.org for tables for joint filers and married filing separately.


| State | Notes |
| --- | --- |
| Alabama | Allow some or all of federal income tax paid to be deducted from state taxable income. Local income taxes are excluded; the average in each juridiction is 0.5%. Weighted local rates are from the Tax Foundation’s 2015 State Business Tax Climate Index. |
| Alaska | No individual income tax. |
| Arizona | Shows 2015 rates but 2014 brackets, because the state began indexing in the 2015 tax year. |
| Arkansas | Rates apply to regular tax table. A special tax table is available for low income taxpayers which reduces their tax payments. Bracket levels adjusted for inflation each year. |
| California | Shows 2015 rates but 2014 brackets, where laws forbid revenue officials from inflation-indexing brackets until mid-year. Bracket levels adjusted for inflation each year. |
| Colorado | Tax levied on federal taxable income. |
| Delaware | Local income taxes are excluded; the average in each jurisdiction is 0.63%. Weighted local rates are from the Tax Foundation’s 2015 State Business Tax Climate Index. |
| Florida | No individual income tax. |
| Idaho | Shows 2015 rates but 2014 brackets, where laws forbid revenue officials from inflation-indexing brackets until mid-year. Bracket levels adjusted for inflation each year. |
| Illinois | Tax levied on federal adjusted gross income with modifications. |
| Indiana | Tax levied on federal adjusted gross income with modifications. Local income taxes are excluded; the average in each jurisdiction is 1.49%. Weighted local rates are from the Tax Foundation’s 2015 State Business Tax Climate Index. |
| Iowa | Bracket levels adjusted for inflation each year. Allow some or all of federal income tax paid to be deducted from state taxable income. |
| Kansas | Local income taxes are excluded; the average in each jurisdiction is 0.01%. Weighted local rates are from the Tax Foundation’s 2015 State Business Tax Climate Index. |
| Kentucky | Local income taxes are excluded; the average in each jurisdiction is 2.08%. Weighted local rates are from the Tax Foundation’s 2015 State Business Tax Climate Index. |
| Louisiana | Allow some or all of federal income tax paid to be deducted from state taxable income. |
| Maine | Bracket levels adjusted for inflation each year. Has suspended inflation indexing for the years 2014-2015. |
| Maryland | Local income taxes are excluded; the average in each jurisdiction is 2.88%. Weighted local rates are from the Tax Foundation’s 2015 State Business Tax Climate Index. |
| Michigan | Tax levied on federal adjusted gross income with modifications. Local income taxes are excluded; the average in each jurisdiction is 1.7%. Weighted local rates are from the Tax Foundation’s 2015 State Business Tax Climate Index. |
| Minnesota | Bracket levels adjusted for inflation each year. |
| Missouri | Allow some or all of federal income tax paid to be deducted from state taxable income. Local income taxes are excluded; the average in each jurisdiction is 0.5%. Weighted local rates are from the Tax Foundation’s 2015 State Business Tax Climate Index. |
| Montana | Shows 2015 rates but 2014 brackets, where laws forbid revenue officials from inflation-indexing brackets until mid-year. Bracket levels adjusted for inflation each year. Allow some or all of federal income tax paid to be deducted from state taxable income. |
| Nebraska | Has a "tax benefit recapture," by which many high-income taxpayers pay their top tax rate on all income, not just on amounts above the bracket threshold. |
| Nevada | No individual income tax. |
| New Hampshire | Tax applies to interest and dividend income only. |
| New Jersey | Local income taxes are excluded; the average in each jurisdiction is 0.5%. Weighted local rates are from the Tax Foundation’s 2015 State Business Tax Climate Index. |
| New York | Bracket levels adjusted for inflation each year. Local income taxes are excluded; the average in each jurisdiction is 2.11%. Weighted local rates are from the Tax Foundation’s 2015 State Business Tax Climate Index. Has a "tax benefit recapture," by which many high-income taxpayers pay their top tax rate on all income, not just on amounts above the bracket threshold. |
| North Dakota | Bracket levels adjusted for inflation each year. |
| Ohio | Shows 2015 rates but 2014 brackets, where laws forbid revenue officials from inflation-indexing brackets until mid-year. Bracket levels adjusted for inflation each year. Local income taxes are excluded; the average in each jurisdiction is 2.25%. Weighted local rates are from the Tax Foundation’s 2015 State Business Tax Climate Index. Has suspended inflation indexing for the years 2013-2015. |
| Oregon | Bracket levels adjusted for inflation each year. Allow some or all of federal income tax paid to be deducted from state taxable income. Local income taxes are excluded; the average in each jurisdiction is 0.36%. Weighted local rates are from the Tax Foundation’s 2015 State Business Tax Climate Index. |
| Pennsylvania | Local income taxes are excluded; the average in each jurisdiction is 2.96%. Weighted local rates are from the Tax Foundation’s 2015 State Business Tax Climate Index. |
| Rhode Island | Bracket levels adjusted for inflation each year. |
| South Carolina | Bracket levels adjusted for inflation each year. |
| South Dakota | No individual income tax. |
| Tennessee | Tax applies to interest and dividend income only. |
| Texas | No individual income tax. |
| Vermont | Bracket levels adjusted for inflation each year. |
| Washington | No individual income tax. |
| Wisconsin | Bracket levels adjusted for inflation each year. |
| Wyoming | No individual income tax. |

### Inheritance Taxes and Exemptions

Inheritance taxes are taxes on shares bequeathed estates, with rates varying by the named beneficiary of each share. Only Iowa, Kentucky, Maryland, Nebraska, New Jersey and Pennsylvania levy inheritance taxes.

Iowa exempts estates valued at less than $25,000 and annuites purchased through pension/retirement plans, and levies special rates for certain charitable and non-charitable organizations ([source](http://www.iowa.gov/tax/educate/78517.html)).

Kentucky prorates exemptions for non-resident decedents based on the net estate value based in Kentucky. So, if 20% of the net value of an estate is based in Kentucky, the standard exemption at that bracket is multiplied by 20%.

Maryland and New Jersey also have an estate tax. Nebraska's inheritance tax is levied at the county level. New Jersey's inheritance tax only applies to estates over $1,000,000.

In Pennsylvania, parent-child transfers where the child is under 21, transfers of farms and farming equipment, and transfers of some family-owned businesses are exempt.

#### Explanation of Data

These data are formatted as marginal tax rates. If statues allow for exemptions, this is expressed in the data as a marginal bracket where `estateValueAtLeast` equals 0, `estateValueLessThan` equals the exemption amount, and `estateTaxRate` equals 0.

| Name | Description |
| --- | --- |
| `id` | The [ANSI code](https://www.census.gov/geo/reference/docs/state.txt) identifying the state in each record. |
| `stateAbbr` | The [ANSI code](https://www.census.gov/geo/reference/docs/state.txt) abbreviation for the state in each record. |
| `stateName` | The full name of the state in each record. |
| `heirType` | The specific classification of beneficiary. |
| `estateValueAtLeast` | The minimum value of a share of an estate for a given marginal rate to be applicable. |
| `estateValueLessThan` | The maximum value of a share of an estate for a given marginal rate to be applicable. Where blank, there is no maximum. |
| `minimumTax` | Amount of tax paid in a bracket in addition to tax calculated by the marginal rate. |
| `estateTaxRate` | The marginal rate applied to the size of the share of the estate for a given `heirType`. |
| `decedentResidency` | Indicates whether the recently deceased was a `resident` or a `nonresident` of a state, which can affect the tax owed. Where blank, residency status does not matter. |


#### Inheritance Tax Sources

* Iowa: [Iowa Inheritance Tax Rate Schedule](http://www.iowa.gov/tax/forms/60061.pdf)
* Kentucky: [Kentucky Inheritance and Estate Tax Forms and Instructions](http://revenue.ky.gov/NR/rdonlyres/50722C6D-479E-472C-AF55-FF5BEADABE15/0/92A200P714.pdf)
* Nebraska: [Direct family inheritance tax rates](http://nebraskalegislature.gov/laws/statutes.php?statute=77-2004), [remote familiy inheritance tax rates](http://nebraskalegislature.gov/laws/statutes.php?statute=77-2005), [charitable exemptions](http://nebraskalegislature.gov/laws/statutes.php?statute=77-2007.04).

### State Debt Per Capita

Debt at end of fiscal year. See **People Per Household** for average people per household by state. DC is included only in state-local combined data. Source: U.S. Census Bureau, Tax Foundation calculations

## State and Local Debt Per Capita

Total outstanding debt at end of fiscal year.  See **People Per Household** for average people per household by state. Source: U.S. Census Bureau, Tax Foundation calculations

## Income Per Capita by State

Per capita personal income is total personal income divided by total midyear population. All dollar estimates are in current dollars (not adjusted for inflation). Source: Bureau of Economic Analysis

## People Per Household

Does not include persons living institutionalized housing, defined as adult or juvenile correctional institutions, some medical and military facilities, hospital residents, and psychiatric facilities. Source: U.S. Census Bureau, Tax Foundation calculations