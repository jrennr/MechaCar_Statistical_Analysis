# MechaCar Project

## Linear Regression to Predict MPG

Call:
lm(formula = mpg ~ vehicle_length + vehicle_weight + spoiler_angle + 
    ground_clearance, data = mecha_car_data)

Residuals:
     Min       1Q   Median       3Q      Max 
-21.3395  -4.1155  -0.2094   6.8789  17.2672 

Coefficients:
                   Estimate Std. Error t value
(Intercept)      -1.076e+02  1.576e+01  -6.823
vehicle_length    6.240e+00  6.609e-01   9.441
vehicle_weight    1.277e-03  6.948e-04   1.837
spoiler_angle     8.031e-02  6.656e-02   1.207
ground_clearance  3.659e+00  5.394e-01   6.784
                 Pr(>|t|)    
(Intercept)      1.87e-08 ***
vehicle_length   3.05e-12 ***
vehicle_weight     0.0728 .  
spoiler_angle      0.2339    
ground_clearance 2.13e-08 ***
---
Signif. codes:  
0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

Residual standard error: 8.853 on 45 degrees of freedom
Multiple R-squared:  0.7032,	Adjusted R-squared:  0.6768 
F-statistic: 26.65 on 4 and 45 DF,  p-value: 2.277e-11

### Interpretation:

 Variables with p-values less than 0.05 provided a non-random amount of variance to the model. The variables vehicle_length and ground_clearance have p-values much smaller than 0.05. This indicates that they provided a non-random amount of variance to the mpg values.


The slope of the linear model is not considered to be zero.
The coefficients for vehicle_length and ground_clearance are statistically significant because they have p-values that are much smaller than 0.05. The significance of these coefficients means that they are contributing to predicting the mpg values effectively and they are not equal to zero.


This model can account for 70.32% of the variability in mpg using the predictor variables vehicle_length, vehicle_weight, spoiler_angle, and ground_clearance. Also, there could be other factors that weren't included in the model that contribute to the mpg values and are not accounted for.

Additionally, two variables, vehicle_weight and spoiler_angle, have p-values greater than 0.05, indicating they might not be statistically significant predictors. This suggests that they may not even contribute much to the predictive power of the model.

Therefore, the linear model may be somewhat effective in predicting mpg, but there is room for improvement by either identifying more relevant predictors or considering other factors that influence mpg in the MechaCar prototypes.



## Summary Statistics on Suspension Coils

The MechaCar suspension coils were tested across multiple manufacturing lots to ensure consistency in the manufacturing process. The summary statistics for the suspension coil's PSI are:

### Total Summary

![Total Summary](https://github.com/jrennr/MechaCar_Statistical_Analysis/blob/main/Total_Summary.png)

The variance of the suspension coil's PSI across all manufacturing lots is calculated to be 62.29356 pounds per square inch. This value is well below the design specification limit of 100 pounds per square inch. Therefore, the current manufacturing data for all manufacturing lots in total meets the design specification.

### Lot Summary

![Lot Summary](https://github.com/jrennr/MechaCar_Statistical_Analysis/blob/main/Lot_Summary.png)

The lot summary provides mean, median, variance, and standard deviation values for each manufacturing lot.

The current manufacturing data for each individual lot meets the design specification of not exceeding 100 pounds per square inch.

In conclusion, the MechaCar suspension coils meet the design specifications as the variance of the suspension coil's PSI is within the allowable limit for all manufacturing lots in total and each lot individually. The data indicates consistent manufacturing quality across different lots.





## T-Tests on Suspension Coils

Summary:
Based on the t-tests conducted on the suspension coils' PSI data, we found the following results:

- The t-test for all manufacturing lots combined:
  - The p-value was 0.1539, which is greater than the significance level of 0.05.
  - We do not have sufficient evidence to reject the null hypothesis.
  - There is no significant difference between the mean PSI of all manufacturing lots and the population mean of 1,500 psi.

- T-tests for individual manufacturing lots:
  - Lot 1: p-value = 0.5245 (No significant difference)
  - Lot 2: p-value = 0.6389 (No significant difference)
  - Lot 3: p-value = 0.0417 (Significant difference)
  
  For Lot 3, the p-value is less than 0.05, indicating a significant difference between the mean PSI and the population mean.

Screenshots:
![Total Summary T-Test]( "C:\Users\Columbia bootcamp\MenchaCar\test_all_lots.png")

![Lot 1 T-Test]( "C:\Users\Columbia bootcamp\MenchaCar\test_lot1.png")

![Lot 2 T-Test]( "C:\Users\Columbia bootcamp\MenchaCar\test_lot2.png")

![Lot 3 T-Test]( "C:\Users\Columbia bootcamp\MenchaCar\test_lot3")
