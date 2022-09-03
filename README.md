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
