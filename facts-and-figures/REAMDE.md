# Facts and Figures 2014

Published March 19, 2014.

## Notes

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