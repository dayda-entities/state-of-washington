---
title: >-
  Broadband Adoption and Computer Use by year, state, demographic
  characteristics
created: '2020-11-10T17:20:06.424563'
modified: '2020-11-10T17:20:06.424573'
state: active
type: dataset
tags:
  - Adoption
  - Broadband
  - Census
  - Ntia
groups:
  - Local Government
csv_url: 'https://data.wa.gov/api/views/8sap-vzbp/rows.csv?accessType=DOWNLOAD'
json_url: 'https://data.wa.gov/api/views/8sap-vzbp/rows.json?accessType=DOWNLOAD'
layout: post

---
This dataset is imported from the US Department of Commerce, National Telecommunications and Information Administration (NTIA) and its "Data Explorer" site.  The underlying data comes from the US Census

1. dataset: Specifies the month and year of the survey as a string, in "Mon YYYY" format. The CPS is a monthly survey, and NTIA periodically sponsors Supplements to that survey.

2. variable: Contains the standardized name of the variable being measured. NTIA identified the availability of similar data across Supplements, and assigned variable names to ease time-series comparisons.

3. description: Provides a concise description of the variable.

4. universe: Specifies the variable representing the universe of persons or households included in the variable's statistics. The specified variable is always included in the file. The only variables lacking universes are isPerson and isHouseholder, as they are themselves the broadest universes measured in the CPS.

5. A large number of *Prop, *PropSE, *Count, and *CountSE columns comprise the remainder of the columns. For each demographic being measured (see below), four statistics are produced, including the estimated proportion of the group for which the variable is true (*Prop), the standard error of that proportion (*PropSE), the estimated number of persons or households in that group for which the variable is true (*Count), and the standard error of that count (*CountSE).

DEMOGRAPHIC CATEGORIES

1. us: The usProp, usPropSE, usCount, and usCountSE columns contain statistics about all persons and households in the universe (which represents the population of the fifty states and the District and Columbia). For example, to see how the prevelance of Internet use by Americans has changed over time, look at the usProp column for each survey's internetUser variable.

2. age: The age category is divided into five ranges: ages 3-14, 15-24, 25-44, 45-64, and 65+. The CPS only includes data on Americans ages 3 and older. Also note that household reference persons must be at least 15 years old, so the age314* columns are blank for household-based variables. Those columns are also blank for person-based variables where the universe is "isAdult" (or a sub-universe of "isAdult"), as the CPS defines adults as persons ages 15 or older. Finally, note that some variables where children are technically in the univese will show zero values for the age314* columns. This occurs in cases where a variable simply cannot be true of a child (e.g. the workInternetUser variable, as the CPS presumes children under 15 are not eligible to work), but the topic of interest is relevant to children (e.g. locations of Internet use).

3. work: Employment status is divided into "Employed," "Unemployed," and "NILF" (Not in the Labor Force). These three categories reflect the official BLS definitions used in official labor force statistics. Note that employment status is only recorded in the CPS for individuals ages 15 and older. As a result, children are excluded from the universe when calculating statistics by work status, even if they are otherwise considered part of the universe for the variable of interest.

4. income: The income category represents annual family income, rather than just an individual person's income. It is divided into five ranges: below $25K, $25K-49,999, $50K-74,999, $75K-99,999, and $100K or more. Statistics by income group are only available in this file for Supplements beginning in 2010; prior to 2010, family income range is available in public use datasets, but is not directly comparable to newer datasets due to the 2010 introduction of the practice of allocating "don't know," "refused," and other responses that result in missing data. Prior to 2010, family income is unkown for approximately 20 percent of persons, while in 2010 the Census Bureau began imputing likely income ranges to replace missing data.

5. education: Educational attainment is divided into "No Diploma," "High School Grad,
