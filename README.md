## 1. Assigment 1
### Project Overview

The aim of this projects is to introduce you to data visualiazation with Python as concrete and as consistent as possibe. Using what you've learned; download the London Crime Dataset from Kaggle. This dataset is a record of crime in major metropolitan areas, such as London, occurs in distinct patterns. This data covers the number of criminal reports by month, LSOA borough, and major/minor category from Jan 2008-Dec 2016.

This dataset contains:
* `lsoa_code`: this represents a policing area
* `borough`: the london borough for which the statistic is related
* `major_category`: the major crime category
* `minor_category`: the minor crime category
* `value`: the count of the crime for that particular borough, in that particular month
* `year`: the year of the summary statistic
* `month`: the month of the summary statistic

link dataset : https://www.kaggle.com/jboysen/london-crime


## 2. Assigment 2
### Project Overview

Using what you've learned; download the NYC Property Sales Dataset from Kaggle. This dataset is a record of every building unit (apartment, etc) solid in the New York City property market over a 12-month period.

This dataset contains the location, address, type, sale price, and sale date of building units solid. A reference on the trickier fields.

* `BOROUGH`: A digit code for the borough the property is located in; in order these are Manhattan(1),Bronx(2),Brooklyn(3), Queens(4), and Staten Island(5).
* `BLOCK; LOT`: The combination of borough, block, and lot forms a unique key for property in New York City. Commonly called a BBL.
* `BUILDING CLASS AT PRESENT and BUILDING CLASS AT TIME OF SALE`: The type of building at various points in time.

Note that because this is a financial transaction dataset, there are some points that need to be kept in mind:

* Many sales occur with a nonsensically small dollar amount: $0 most commonly. These sales are actually transfers of deeds between parties: for example, parents transferring ownership to their home to a child after moving out for retirement.
* This dataset uses the financial definition of a building/building unit, for tax purposes. In case a single entity owns the building in question, a sale covers the value of the entire building. In case a building is owned piecemeal by its resident (a condominium), a sale refers to a single apartment or group of apartments) owned by some individual.

link dataset: https://www.kaggle.com/new-york-city/nyc-property-sales


## 3. Assigment 3
### Project Overview

The data is related with direct marketing campaigns of a Portuguese banking instituation. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) wouls be ('yes') or not ('no') subscribed.

`bank-additional-full.csv` with all examples (41188) and 20 inputs, ordered by date (from May 2008 to November 2010), very close to the data analyzed in [Moro et al.,2014]
  
The smallest datasets are provided to test more computatioally demanding machine learning algorithms (e.g., SVM).

The classification goal is to predict if the client will subscribe (yes/no) a term deposit (variable y).

User Details:
   1. `age` (numeric)

   2. `job` : type of job (categorical: 'admin.','blue-collar','entrepreneur','housemaid','management','retired','self-employed','services','student','technician','unemployed','unknown')

   3. `marital` : marital status (categorical: 'divorced','married','single','unknown'; note: 'divorced' means divorced or widowed)

   4. `education` (categorical: 'basic.4y','basic.6y','basic.9y','high.school','illiterate','professional.course','university.degree','unknown')

   5. `default`: has credit in default? (categorical: 'no','yes','unknown')

   6.  `housing`: has housing loan? (categorical: 'no','yes','unknown')

   7. `loan`: has personal loan? (categorical: 'no','yes','unknown')

Related with the last contact of the current campaign:
   8. `contact`: contact communication type (categorical: 'cellular','telephone')

   9. `month`: last contact month of year (categorical: 'jan', 'feb', 'mar', ..., 'nov', 'dec')

   10. `day_of_week`: last contact day of the week (categorical: 'mon','tue','wed','thu','fri')

   11. `duration`: last contact duration, in seconds (numeric). Important note: this attribute highly affects the output target (e.g., if duration=0 then y='no'). Yet, the duration is not known before a call is performed. Also, after the end of the call y is obviously known. Thus, this input should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model.

Other attributes:

   12. `campaign`: number of contacts performed during this campaign and for this client (numeric, includes last contact)

   13. `pdays`: number of days that passed by after the client was last contacted from a previous campaign (numeric; 999 means client was not previously contacted)

   14. `previous`: number of contacts performed before this campaign and for this client (numeric)

   15. `poutcome`: outcome of the previous marketing campaign (categorical: 'failure','nonexistent','success')

Social and economic context attributes
   16. `emp.var.rate`: employment variation rate - quarterly indicator (numeric)

   17. `cons.price.idx`: consumer price index - monthly indicator (numeric)

   18. `cons.conf.idx`: consumer confidence index - monthly indicator (numeric)

   19. `euribor3m`: euribor 3 month rate - daily indicator (numeric)

   20. `nr.employed`: number of employees - quarterly indicator (numeric)

Output variable (desired target):

   21. `y` - has the client subscribed a term deposit? (binary: 'yes','no')
   
   link dataset: https://archive.ics.uci.edu/ml/datasets/Bank+Marketing