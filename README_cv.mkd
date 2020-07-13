# Problem Statement

<em>There are a seemingly innumerable amount of features that can be factored into the ultimate determination of a listing price for a home. Those features influence both the price that a property is listed at along with the price that is agreed upon to sell. In an effort to minimize the input costs on a property before sale for an optimal return I have measured the effect of a few different features on the variability of a property's sale price. Along with modifications to the home that an owner can choose to make as an investment we will also analyze some of the built-in attributes and the weight that they impress upon the sale. Our objective as real estate investors is to find the proper combination of features that will allow us to optimize for net return on a property.</em>

## Executive Summary

Through thorough analysis of the 'Ames Housing' dataset as well as independent research, I have isolated 12 features that will aid an appraiser in determining ~85% of the variability in 'Sale Price' for a property.

### Contents:
- [Link Test](#this-is-a-link-test)
- [2018 Data Import and Cleaning](#2018-Data-Import-and-Cleaning)
- [Exploratory Data Analysis](#Exploratory-Data-Analysis)
- [Data Visualization](#Visualize-the-data)
- [Descriptive and Inferential Statistics](#Descriptive-and-Inferential-Statistics)
- [Outside Research](#Outside-Research)
- [Conclusions and Recommendations](#Conclusions-and-Recommendations)

### Data Dictionary

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**SalePrice**|*float*|train|The USD that a listing sold for.|
|**Overall Qual**|*int*|train|Numerical score of total porperty on ten point scale.|
|**Neighborhood**|*string*|train|1 of 28 different neighborhoods that the structure is located in.|
|**House Style**|*string*|train|One of 8 different structure styles influencing the style of the structure.|
|**Bldg Type**|*string*|train|One of 5 different structure types usually determined by the structure's capacity.|
|**Gr Liv Area**|*int*|train|Ground floor living room area of the structure measured in ft <sup>2</sup>.|
|**Garage Area**|*int*|train|Space within garage measured in ft <sup>2</sup>.|
|**Garage Cars**|*int*|train|The number of cars that can be kept in the garage.|
|**Total Bsmt SF**|*int*|train|Space within the structure's basement measured in ft <sup>2</sup>.|
|**1st Floor SF**|*int*|train|Space on the first floor of the structure measured in ft <sup>2</sup>.|
|**age_weight**|*int*|train|The current year (2020) * the 'Year Built'.|
|**sell_age_weight**|*int*|train|'Year Sold' * 'Year Built'.|
|**remodel_age_weight**|*int*|train|The current year (2020) * the 'Year Remod/Add'.|



# Conclusion

### Recommendations
Instead of spending time recording and measuring as many attributes as possible surrounding a real estate listing, first focus on recording the 12 features listed in the data dictionary. Those features have been shown test results of explaining ~85% of the variability in 'Sale Price' of a listing historically.

### Next Steps
* Attempt to achieve lower levels of granularity with neighborhood, city, house style, crime rates of zip, school system grade etc.
    * Parsing out street information with regex functions/methods could let us look at blocks/ranges of blocks within a neighborhood
* Dig into seemingly subjective measures such as 'Overall Qual', 'Functional', etc.
* Continue to record new housing data as it actualizes. We can strengthen our model through higher record counts as well as refine the weights of the features that we have previously pinpointed.