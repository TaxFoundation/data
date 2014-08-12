# IRS Interstate Migration Data, Inflows from 1992 to 2011

This dataset is a compilation of [IRS data](http://www.irs.gov/uac/SOI-Tax-Stats-Migration-Data) about where taxpayer claim to live from one tax year to another. By using income tax filing data, the IRS can estimate interstate migration of households and individuals within the United State and how much taxable income a state gains or loses year-to-year.

Original IRS data also includes figures for foreign migration, but these data are not included in this compiled dataset. The [Tax Foundation](http://taxfoundation.org)'s goal in compiling these data was to measure interstate, rather than international, migration.

The IRS provides both inflow and outflows. We have only compiled inflows. Outflows are easily obtained from inflow data. The inflow to `targetState` from `sourceState` is equal to the outflow from `sourceState` to `targetState`.

The Tax Foundation has used these data to create an [interactive tool](http://interactive.taxfoundation.org/migrationsTableGenerator/) for examining interstate migrations. The code for this tool is also [available on GitHub](https://github.com/TaxFoundation/MigrationTables).

| Name | Description |
| --- | --- |
| `year` | The ending tax year during which a migration occurred. |
| `targetState` | The ANSI code for the state receiving migration inflows. |
| `sourceState` | The ANSI code for the state from which the `targetState` is receiving inflows. |
| `taxReturnInflows` | The number of new tax returns filed in a `targetState` by people who filed the previous year in the `sourceState` This number could reprent individual single filers or entire joint-filing households. |
| `taxExemptionsInflows` | The number of new tax exemptions claimed in a `targetState` by people who filed the previous year in the `sourceState` This number more closely approximates individuals, whether single or as part of a household. |
| `adjustedGrossIncomeInflows` | The sum of income being reported in the `targetState` by filers in that record. Where `targetState` and `sourceState` are equal, this figure represents the claimed income of non-migrants. Where different, it represents inflows of income to `targetState` from `sourceState`.