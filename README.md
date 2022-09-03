# MechaCar Statistical Analysis

## Linear Regression to Predict MPG
Using our RScript, we gather the following information:

![deliv 1](https://user-images.githubusercontent.com/19378130/188281116-d1422b0a-8600-4793-b5ea-045dc549c52d.PNG)

- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
  - Vehicle_length and ground_clearance, as well as Intercept (marked with ***)

- Is the slope of the linear model considered to be zero? Why or why not?
  - No, because our Pvalues do not equal 0
 
- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
  - According to our Multiple R-squared outcome of 0.7149, our model predicts 71% accuracy


## Summary Statistics on Suspension Coils
Here we can see the tables created with our total_summary and lot_summary dataframes

![total summary](https://user-images.githubusercontent.com/19378130/188282937-5ecd6281-eab4-4191-8bac-6d95a2d19e98.PNG)

![lot summary](https://user-images.githubusercontent.com/19378130/188282940-90a8c141-928a-4d1e-ba2f-f387ca0828f8.PNG)

- The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
  - Looking at our total summary, the variance looks great, but once broken down by the lot, we can see that Lot3 is over the threshold of 100 PSI.



## T-Tests on Suspension Coils
Here is our lot-wide test:

![t test](https://user-images.githubusercontent.com/19378130/188283330-68ea1706-9d05-4312-b859-817e59eff0da.PNG)

A P-value of 0.05 or less is significant enough to reject the hypothesis. We can see that our P-Value is 0.06, so we fail to reject the null hypothesis.

--------
Our individual lot tests:

![t test each lot](https://user-images.githubusercontent.com/19378130/188283344-ccd9fe2b-243d-4432-940c-c91eaaa31360.PNG)

Lot 1 shows that they are not statistically different from the population mean, our P-Value is 1, meaning we fail to reject the null hypothesis.

Lot 2 has a P-value of 0.6072, so we again fail to reject the null hypothesis.

Lot 3 shows that they are slightly statistically different from the rest of the population, they also have a P-Value of 0.0417. That is low enought for us to reject the null hypothesis. This proves that this lot should be discarded


## Study Design: MechaCar VS Competition
I would suggest comparing MechaCar to it's competitors in the POV of a family by looking at the cost of the vehicle, fuel efficiency, and safety ratings.

H0: MechaCar is equal to the competition

Ha: MechaCar is statistically above/below the ratings of our competition

We would need to use ANOVA testing. this would help to answer if there is a statistical difference of the means in multiple samples. It will help us to look at categorical data about multiple competitors. The data needed for this test is the cost, mpg, and safety ratings from MechaCar and its competition.

