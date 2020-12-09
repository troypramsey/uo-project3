# Gentrification And Commercial Decisions: 
### Can We Predict Starbucks/Walmart Location Counts Using Gentrification Markers?

##### Our Gentrification Metrics
We developed three metrics for building our model features: 
- change in median household income
- change in median home values
- change in the percentage of the population possessing a bachelors degree or higher
    
These are the variables used by the Harvard Kennedy School Ash Center, which has been developing metrics for measuring gentrification since 2013. The US Census ACS5 API can call each of these metrics, enabling us to find change over time. However, because we don't have data on when each of these locations opened, we thought looking at longitudinal change over time may show more patterns in our data, rather than a single snapshot in time.
    
##### Why Starbucks? Why Walmart?
Our own assumptions and biases, especially in a nationally recognized zone of significant gentrification (the Portland area), were the basis for choosing our dependent variable locations.
    
##### How did we handle missing data?
The average amount of NaN values in each feature was between 3%-5%, a value which we thought was within the acceptable range to minimize skew.
    
##### What were our findings?
Overall, we see little to no correlation between gentrification markers between 2011-2018 and the number of each dependent store. Walmarts can be predicted a little better than Starbucks, but we don't believe either company heavily utilized these metrics in deciding on opening new locations based on our data. We cannot fully assume this, however, due to the discussed weak areas in our data discussed below.
    
##### What were the weak points in our data?
- We did not possess any data on when new locations were opened for each of these locations, which means that many of them existed prior to the calculation of our gentrification variables. This also illustrates that the inverse hypothesis does not hold true, as gentrification does not appear to occur in any easily predictable measure in areas that already may have Starbucks or Walmart locations from before our data collection.
- Our dataset was limited to 2011 and onwards, as many of these measures were not available in previous estimate datasets.
- Our own biases in the Portland area assumed more mixed-use neighborhood distribution across the country. We assume that zipcodes with the highest gentrification markers are most likely residential-only areas that may not have any commercial operations within their boundaries.