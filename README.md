# Cars-Statistical-Analysis

## Linear Regression to Predict MPG
1.Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
Based on the summary of our multiple linear regression, car ground clearance and vehicle length provided a non-random amount of variance to our mpg data. This is evidenced by their extremely low 'Pr(>|t|)' values. This value is a measure of the likelihood that the variance that the variable in question provides is random. So, the fact that the p-values for these variables is much smaller than 0.05(95% confidence) indicates that the variables are good predictors of fuel efficiency.  

2. Is the slope of the linear model considered to be zero? Why or why not?
No, the slope of the linear model is not zero. If it were, that would indicate no relationship between the variables in our model and fuel efficiency. As mentioned in question 1, this is not the case.

3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
Yes, this model is a decent predictor of fuel efficiency. This is because in the summary of our linear model, we can see our model has a relatively high adjusted R-squared value of 0.6825. This can be interpreted as saying that our model succesfully predicts around 70% of the non-random variation in the relationship between our variables. While we may desire an R-squared around 0.9, our current R-squared is acceptable. It would be worth mentioning in our report that our model only explains around 70% of the data however.

## Summary Statistics on Suspension Coils
Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
- In total, the manufacturing datra meets the design specifications for MechaCar. However, when examined individually we can see that Lot 3 does not meet the design specifications. Below are the figures used to make this conclusion:

![Total_mechacar](https://user-images.githubusercontent.com/93050931/154864974-eaf64d83-b989-4c6f-9500-7c7035931482.png)
(Figure 1: Summary of all lots: We can see that the variance of the PSI of the suspension coils is ~62.3 across all manufacturing lots. So, we can assume manufacturing is up to spec.)

![indiv_manufacturing](https://user-images.githubusercontent.com/93050931/154865057-185aa6af-d18c-4af3-b301-8a987c8721e8.png)
(Figure 2: Summary for individual lots: In this figure it is clear that Lot 1 and 2 have extremely low variances which are masking the deficiencies of lot 3 when all lots are looked at together. We can therefore, conclude that Lot 3 is not manufacturing suspension coils up to the design specifications.)


## T-Tests on Suspension Coils
By conducting one-sample t-tests on the mean coil PSI of each lot to the population mean of 1500 PSI, we can see that the only lot with a statistically different mean than 1500 is Lot 3.

The figure below is the results of the t-test for the hypothesis that the mean PSI of Lot 1 is statistically different from the population mean of 1500 PSI. As we can see, the resulting p-value is above 0.05. This means that we cannot reject the null hypothesis and that the two means are statistically similar.
![Lot_1_t_test](https://user-images.githubusercontent.com/93050931/154866056-a37e693e-c0ff-4908-a3d9-664c2df39b2a.png)

The t-test for Lot 2 has the same result. A p-value of greater than 0.05 means we cannot reject the null hypothesis and that the means are statistically similar.
![ttest_lot2](https://user-images.githubusercontent.com/93050931/154866182-60584207-6645-4638-81a3-2a5d7c4b16e0.png)

Lastly, the t-test for Lot 3 shows that the resulting p-value of 0.04168. This number is below 0.05 and means that we can accept the alternative hypothesis that the two means are statistically different.
![lot_3_ttest](https://user-images.githubusercontent.com/93050931/154866235-422c41a1-dd4b-4634-bcbf-aed8f76f1e9d.png)




## Study Design: MechCar vs Competition
