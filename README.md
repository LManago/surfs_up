# surfs_up

##### Overview of the statistical analysis

This analysis was done to analyze the ability to sustain a surf shop in Hawaii year round. The analysis gives the trends of the months mid-year as well as end of year.

##### Results
![Image of December Tobs](https://github.com/LManago/surfs_up/blob/main/Resources/December%20Tobs.PNG)
![Image of June Statistics](https://github.com/LManago/surfs_up/blob/main/Resources/June%20Statistics.PNG)

* The average tempature in December would be 71 degrees with a max tempature of 83.
* The average tempature in June would be 74 with a max of 85. Both months shows of relatively close average tempature.
* The minimun tempature in December was 56 while teh minimum tempature in June was 64.

##### Summary
The tempature in December are only slightly lower than June, which means that opening a surf shop for year round wouldn't be affected by the weather.
Additional analysis to gather which would be good to look at would be the precipation in these two months.
Following code:

* Track the total precipation levels through June & December

session.query(Measurement.date, Measurement.prcp).filter(extract('month', Measurement.date) == 6).all()

session.query(Measurement.date, Measurement.prcp).filter(extract('month', Measurement.date) == 12).all()
