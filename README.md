# MechaCar_Statistical_Analysis

## Overview
### Purpose
- To perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes.
- Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots.
- Run t-tests to determine if the manufacturing lots are statistically different from the mean population
- Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. 

### Linear Regression to Predict MPG
![image](https://user-images.githubusercontent.com/96217224/162641591-80564ba6-41e8-4c6e-a053-8d3484ae3e49.png)

- The strongest contributor of non-random variance seems to be the vehicle length with a p-value of 2.60e-12. The other strong contributor of non-random variance is the ground clearance with a p-value of 5.21e-8.
- The slope of the linear model is not zero. We can see that the slope coefficients contain significant non-zero values (vehicle length, ground clearance, and AWD), and the p-values are less than the significance level of p=0.05.
- Our r^2 value is 0.7149, which means the model does have good predictive power for the mpg.

### Summary Statistics on Suspension Coils
![image](https://user-images.githubusercontent.com/96217224/162641712-5a8b8ec4-5af4-47ad-9304-9f50d81c1968.png) ![image](https://user-images.githubusercontent.com/96217224/162641732-c5c60c5e-3fe4-447d-8061-ab7ece8a4cbb.png)

- The overall variance for the entire dataset indicates that the current manufacturing data meets the 100 pounds per square inch variance limitation. Because the lots are chosen randomly, there is a possiblity that a third of the lot does not meet the necessary suspension coils requirement.


### T-Test on Suspension Coils
![image](https://user-images.githubusercontent.com/96217224/162641899-33f16aa1-817e-4e0f-a439-1c4686051f15.png)

 - Whole Lot:  At a significance level of 0.05, we fail to reject the null hypothesis since the p-value equals 0.06.
 - Lot 1: At a significance level of 0.05, we fail to reject the null hypothesis since the p-value equals 1,
 - Lot 2: At a significance level of 0.05, we fail to reject the null hypthesis again since the p-value equals 0.6072.
 - Lot 3: At a significance level of 0.05, we can reject the null hypothesis since the p-value equals 0.04168. 


### Study Design: MechaCar vs Competition
In comparing MechaCar with a competitor we would need to test whether or not the MechaCar has significant differences in these metrics compared to competing models. The null hypothesis will be that these observables don't vary significantly from the competition, and the alternative hypothesis will be that the MechaCar does indeed vary significantly in these variables compared to the competition.
Perform one-tailed t-tests in order to determine if the MechaCar has higher or lower observed values in these variables than the competition according to which direction the consumer would prefer. The consumer would want the cost to be lower, the city and highway fuel efficiency to be higher, the horsepower to be higher, the safety rating to be higher, and the carbon waste output to be lower. Running these statistical tests, we would need the cost, fuel efficiency, horsepower, safety rating, and carbon waste output data from the MechaCar as well as the competitors.

