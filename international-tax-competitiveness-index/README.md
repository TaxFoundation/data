# International Tax Competitiveness Index

The Tax Foundation’s [International Tax Competitiveness Index](http://taxfoundation.org/article/international-tax-competitiveness-index) (ITCI) measures the degree to which the 34 OECD countries’ tax systems promote competitiveness through low tax burdens on business investment and neutrality through a well-structured tax code. The ITCI considers more than forty variables across five categories: Corporate Taxes, Consumption Taxes, Property Taxes, Individual Taxes, and International Tax Rules.

The ITCI attempts to display not only which countries provide the best tax environment for investment but also the best tax environment to start and grow a business.

## Methodology

The ITCI is a relative ranking of the competitiveness and neutrality of the tax code in each of the 34 OECD countries. It utilizes over 40 variables across five categories: corporate tax, consumption taxes, property taxes, individual taxes, and international tax rules. Each category has multiple subcategories, and each subcategory holds a number of the 40 variables. For example, the consumption tax category contains three subcategories: rate, base, and complexity. The consumption tax base subcategory then has three variables: consumption tax as a percentage of total consumption, deduction limitations, and VAT threshold.

The ITCI is designed to measure a country’s tax code on its relative competitiveness rather than on an absolute measurement. This means that a score of 100 does not signify the absolute best possible tax code but the best tax code among the 34 OECD countries. Each country’s score on the ITCI represents its relative distance from the best country’s score.

### The Calculation of the Variable, Subcategory, and Category Scores

First, the standard deviation and average of each variable is calculated. The standard deviation measures the average distance of a country’s tax variables from the mean among all 34 countries. For example, the average corporate income tax rate across the 34 OECD countries is 25.3 percent with a standard deviation of 6 percentage points. This means that on average, an OECD country’s corporate tax rate is 6 percentage points away from the mean rate of 25.3 percent.

In order to compare each variable, it is necessary to standardize them, because each variable has a different mean and standard deviation. To standardize the variables, each observation is given a normalized score. This sets every variable’s mean to 0 with a standard deviation of 1. Each country’s score for each variable is a measure of its distance from the mean across all countries for that variable. A score of 0 means a country’s score is equal to the average, a score of -1 means it is one standard deviation below average, and a score of 1 is one standard deviation above average.

The score for the corporate tax rate demonstrates this process. Of the 34 OECD countries, the average corporate income tax rate is 25.3 percent, and the standard deviation is 6 percentage points. The United States’ corporate tax rate normalized score is -2.32,64 or 2.32 standard deviations less competitive than the average OECD country. In contrast, Ireland’s tax rate of 12.5 percent is 2.20 standard deviations more competitive than the average OECD country.

The next step is to combine variable scores in order to calculate subcategory scores. Within subcategories, each individual variable’s score is equally weighted and added together. For instance, the subcategory of cost recovery includes six variables: loss carryback, loss carryforward, the present discounted value of depreciation schedules for machines, industrial buildings, and intangibles, and inventory accounting method. The scores for each of these six variables are multiplied by 1/6, or 16.6 percent, to give them equal weight and then added together. The result is the cost recovery subcategory score.

From here, each category’s score is constructed by combining the scores of each contained subcategory. This is computed by multiplying each subcategory by a weight (all weights are equal) and adding the result together. For example, the score for the corporate rate category is calculated by multiplying the scores of the rate, cost recovery, incentives/complexity subcategories by 33.3 percent and adding them together. This is done for all five categories.

The overall normalized score for each country is calculated by taking each category’s normalized score, multiplying each by 20 percent (equal weight for the five categories), and adding them together.

### Calculating the Final Score

From here, two transformations occur on the category scores and the overall score. First, in order to eliminate any negative values, each category’s score and the overall score is converted to its cumulative distribution value, or p-value. These p-values represent the likelihood that a random country’s score is worse than a given country. For example, the United States’ normalized overall score is -0.423. After converting it, the United States receives a p-value of 33.5 percent. This means that there is a 33.5 percent percent chance that the United States has a better tax system than a random OECD country.

Second, the p-value of the overall and category scores for each country is scaled to 100, relative to the country with the highest p-value overall and in each category. This is done by taking each country’s p-value and dividing it by the highest p-value in each category. For example, Estonia, which has the highest overall p-value of 77.9 percent, receives a final overall score of 100. The United States, which has an overall p-value of 33.5 percent, receives a final overall score of 43.1.

## Explanation of Data

| Name | Description |
| --- | --- |
| `country` | Name of each OECD nation in the Index, in English. |
| `maxCorprateRate` | The top marginal corporate tax rate in a given nation. |
| `lossCarryback` | Number of years a corporation may apply current losses against previous tax bills, allowing for tax rebates. |
| `lossCarryforward` | Number of years a corporation may apply current losses against future tax bills, lowering those years' taxable income. |
| `pdvMachines` | Percentage of the present value cost of machinery that corporations can write off over the depreciable life of the asset. |
| `pdvBuildings` | Percentage of the present value cost of buildings that corporations can write off over the depreciable life of the asset. |
| `pdvIntangibles` | Percentage of the present value cost of intangibles that corporations can write off over the depreciable life of the asset. |
| `inventory` | Score given based on a country's allowable inventory cost accounting methods. Countries that allow Last In, First Out (LIFO) score `1`; countries that allow Average Cost of Inventory score `0.5`; countries that only allow First In, First Out (FIFO) score `0`. |
| `patentBox` | Indicates which countries have patent boxes, which create lower tax rates for income generated through patented products. Countries without patent boxes are marked with `0`, countries with patent boxes are marked as `1`. |
| `rndCredit` | Indicates which countries offer research and development tax credits. Countries without such credits are marked `0`; those with R&D credits are marked `1`. |
| `complianceTime` | Complexity of tax system measured by average time in hours needed to comply with a country's corporate tax requirements. |
| `profitPayments` | Complexity of tax system measured by number of yearly profit payments. |
| `otherPayments` | Complexity of tax system measured by number of other yearly tax payments. |
| `vatRate` | The national (or average) consumption tax rate (either sales tax or VAT) for a country. |
| `threshold` | The upper sales limit in US dollars for which a corporation does not need to pay consumption taxes. |
| `base` | The ratio of consumption taxes collected to potential collections if consumption tax rates were applied equally across all goods/services. This ratio measures exemptions to the taxes and/or noncompliance. |
| `deductionLimitations` | Indicates whether or not there are limits to deducting consumption taxes paid on business inputs. Countries with limits to deducations are marked `1`; counties with no limits are marked `0`. |
| `consumptionTime` | Complexity of consumption taxes measured by average time in hours needed for corporations to comply with a country's consumption tax requirements. |
| `propertyTaxes` | Indicates whether capital additions to land are taxed. Fully taxing land and improvements is marked `1`; allowing deductions of taxes on improvements from corporate income taxes is marked `0.5`; taxing only land or not having a property tax is marked `0`. |
| `propertyTaxesCollections` | Property taxes collected in a country as a percentage of GDP. |
| `netWealth` | Indicates the existence of taxes on net wealth. Countries with wealth taxes are marked `1`; those without are marked `0`. |
| `estateOrInheritanceTax` | Indicates the existence of taxes on estates or inheritances. Countries with such taxes are marked `1`; those without are marked `0`. |
| `transferTaxes` | Indicates the existence of taxes on the transfer (buying and selling) of real property. Countries with property transfer taxes are marked `1`; those without are marked `0`. |
| `assetTaxes` | Indicates the existence of a tax on net corporate assets. Countries with an asset tax are marked `1`; those without are marked `0`. |
| `capitalDuties` | Indicates the existence of a tax on the issuance of shares of stock. Countries with a capital duties tax are marked `1`; those without are marked `0`. |
| `financialTrans` | Indicates the existence of a tax on the transfer of financial assets. Countries with financial transfer taxes are marked `1`; those without are marked `0`. |
| `capGainsRate` | Tax rate for capital gains. |
| `capGainsIndex` | Indicates whether a country indexes capital gains against inflation, ensuring that only real returns are taxed. Countries with capital gains indexing are marked `1`; countries without indexing are marked `0`. |
| `divRate` |  The total top marginal dividend tax rate after any imputation or credit system. |
| `incRate` | The top marginal income tax rate. |
| `progressivity` | Measure of progressivity of individual income tax rates as a ratio of minimum income level at which the top rate applies to the average income. |
| `taxWedge` | Total tax cost of labor in a country (includes individual income tax and payroll tax). |
| `laborPayments` | Complexity of tax system measured by number of yearly labor tax payments. |
| `laborTime` | Complexity of tax system measured by average time in hours needed to comply with a country's labor tax requirements. |
| `dividendExempt` | Percentage of dividends paid from foreign subsidiaries which are exempt from local taxes. |
| `capGainsExemption` | Indicates whether capital gains from foreign investments are exempted from local taxes. Fully exempt is marked as `1`; non-exempt is marked as `0`. |
| `divWithhold` | Required withholding for tax payments on dividends to be paid to foreign investors or businesses. |
| `intWithhold` | Required withholding for tax payments on interest to be paid to foreign investors or businesses. |
| `royWithhold` | Required withholding for tax payments on royalties to be paid to foreign investors or businesses. |
| `taxTreaties` | Number of foreign nations with which a country has tax treaties. |
| `cfcRules` | Indicates existence of controlled foreign corporation rules. Countries with CFC rules are marked `1`; those without are marked `0`. |
| `countryLimitations` | Indicates whether country has certain exemptions to a territorial tax system based on the source of the foreign income. Existence of exemptions are marked as `1`; no exemptions are marked `0`.  |
| `thinCap` | Indicates whether a country puts thin capitalization resitrictions on companies' debt-to-asset ratios. Countries with restrictions are marked as `1`; those without are marked `0`. |

## Data Sources

* PricewaterhouseCoopers Worldwide Tax Summaries
* Ernst & Young International Tax Guide
* Deloitte International Tax Source
* The Organization for Economic Cooperation and Development
* The Oxford University Said School of Business Corporate Tax Database
* The Tax Foundation

The ITCI uses the most up-to-date data available as of July 2014.