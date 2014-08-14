# US Federal Income Tax Rates from 1862 to 2014

These data summarize federal marginal income tax rates for US individuals and households beginning in 1862. Dollar amounts listed in `incomeBracket` are in nominal dollars. These rates combine normal and surtax rates where applicable, and do not factor in exemptions.

## Explanation of Data

| Name | Description |
| --- | --- |
| `year` | The year for which the record's rate and bracket are applicable. |
| `incomeTaxRate` | The marginal rate applied to income equal to or greater than the `incomeBracket`, but not above the `incomeBracket` of the next highest `incomeTaxRate` for that `filingStatus` in that `year`. |
| `incomeGreaterThan` | Income above this amount is taxed at the accompanying `incomeTaxRate`, up to and including `incomeNotGreaterThan` for that `year` and `filingStatus`. Values are in nominal dollars. See note below for an example of usage. |
| `incomeNotGreaterThan` | Income less than or equal to this amount, but not less than or equal to `incomeGreaterThan`, is taxable at this marginal `incomeTaxRate`. Values are in nominal dollars. See note below for an example of usage. |
| `filingStatus` | The type of income tax return filed. See the table below for an explanation of the possible values. |

### Using Income Brackets in the Data

US federal income taxes are marginal taxes. The value in `incomeGreaterThan` is the amount above which that marginal bracket becomes applicable, reaching a maximum of `incomeNotGreaterThan`. For example, if you were a `single` filer in 2013 with taxable income of $40,000, you would owe 10% tax on income from $0 to $8,925, 15% from $8,925.01 to $36,250, and 25% on the remainder.

| `incomeTaxRate` | `incomeGreaterThan` | `incomeNotGreaterThan` | Income Taxed | Tax Owed | Remainder |
| --- | --- | --- | --- | --- | --- |
| 0.1 | 0 | 8925 | $8,925 | $892.50 | $31,075 |
| 0.15 | 8925 | 36250 | $27,325 | $4,098.75 | $3750 |
| 0.25 | 36250 | 87850 | $3750 | $937.50 | $0 |

In this example, total tax owed is $5,928.75. This makes the effective tax rate 14.82%.

### Filing Status Explanation

Note: Not every filing status is present for each year.

| Filing Status | Explanation |
| --- | --- |
| `single` | The most basic filing status for individuals who are not married and do not maintain a household. [Learn more.](http://www.irs.gov/publications/p501/ar02.html#en_US_2013_publink1000220736) |
| `marriedFilingSeparately` | Married individuals who choose to file their tax returns separately from each other. [Learn more.](http://www.irs.gov/publications/p501/ar02.html#en_US_2013_publink1000220762) |
| `marriedFilingJointly` | Married individuals who file a single tax return reporting their combined income. [Learn more.](http://www.irs.gov/publications/p501/ar02.html#en_US_2013_publink1000220742) |
| `headOfHousehold` | Typically individuals who are unmarried and bear over half the cost of keeping up a household with qualifying dependents. [Learn more.](http://www.irs.gov/publications/p501/ar02.html#en_US_2013_publink1000220775) |

## Additional Resources

* [Tax Foundation](http://taxfoundation.org/article/us-federal-individual-income-tax-rates-history-1913-2013-nominal-and-inflation-adjusted-brackets)