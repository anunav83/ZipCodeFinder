## Finding Zip Codes based on latitude and longitude

As part of another project I had geocodes of over 100,000 location beloging to same neighborhood, the data is useless unless we had the ZIP codes the location belonged to. Using google APIs / other Thrid Party APIs had a cap on how many zipcodes we could find in a day for free.

In this project we will determine the zip codes based on the geocode( latitude and longitude) with upto 97.7% accuracy using clustering techniques ( KNearest Neighbors)

### Training Data 

Below table contains few records we have in our training data (TrainingData.csv). THe training data has geocodes and the corresponding ZIP Code

| latitude | longitude | address | zipcode |
| :---         |     :---:      |          ---: |          ---: |
| 37.783970 |-122.390156 | 180 Brannan St, San Francisco, CA 94105, USA	|94105|
|	37.771100 |-122.424606 | Market St & Laguna St, San Francisco, CA 94102 |94102|
|	37.755795	|-122.432384 | 822 Noe St, San Francisco, CA 94114, USA	|94114|

Create the traing data using google geocode api to get info on zipcodes.

### Zip Codes in Training Data

![Test Image 4](https://github.com/anunav83/ZipCodeFinder/blob/master/ZipCode-Distribution.png)

### Distribution of datapoints grouped by their Zipcode.

![Test Image 5](https://github.com/anunav83/ZipCodeFinder/blob/master/ZipCode-OnAMap.png)
