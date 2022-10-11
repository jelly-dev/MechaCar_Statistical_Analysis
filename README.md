# MechaCar_Statistical_Analysis

## Overview

- AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has requested a review of the production data for insights that may help the manufacturing team. The analysis includes the following:

    - Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes

    - Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
    - Run t-tests to determine if the manufacturing lots are statistically different from the mean population

    - Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, a summary is included.

## Linear Regression to Predict MPG

![Linear regression model](/images/linearRegression.png "Linear regression model")

- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

    - p-value of coefficients should be compared to alpha = .05 level of significance to verify if statistically significant.

        - mpg: 0 < .05 significant, <b><em>non-random</em></b>
        - vehicle length: 0 < .05, significant, <b><em>non-random</em></b>
        - vehicle weight: .08 > .05 not significant, random
        - spoiler angle: .31 > .05 not significant, random
        - ground clearance: 0 > .05 significant, <b><em>non-random</em></b>
        - AWD: .19>=.05 not statistically significant, random amount of variance

    - The three variables that provided non-random variance are mpg, vehicle length, and ground clearance. 

- Is the slope of the linear model considered to be zero? Why or why not?

    - Although some of the slopes of the variables come close to zero, the linear regression formula results in a non-zero slope.

- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

    - The r-squared value is .7149, meaning the dataset is effective and shows a strong correlation. However, there may be other unmeasured variables that play into the mpg that are needed for the most effective prediction.

## Summary Statistics on Suspension Coils

### Total Manufacturing Lot Summary

![Total lot summary](/images/summary_all_lots.png "Total lot summary")

### Summary per Manufacturing Lot

![Each lot summary](/images/summary_each_lot.png "Each lot summary")

- The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

    - Total manufacturing lot variance is 62, which is within the design specification of staying under 100 PSI. However, when reviewing the data by each lot, Lot 3 is found to be a large contributing factor to high variance. Lot 3 shows a variance of 170 which is too high to meet design specifications.

## T-Tests on Suspension Coils
    - The majority of lots show a normal distribution. There is not sufficient evidence to reject the null hypothesis, showing that the two means are statistically similar.

### T-test for All Lots
![T-test all lots](/images/t_test_all.png "T-test all lots")

    - p-value = .6028, alpha = .05

    - The total manufacturing lot is not statistically significant from the normal distribution and normality can be assumed. The mean falls within the 95% confidence interval.

### T-test for Lot 1

![T-test lot 1](/images/t_test_1.png "T-test lot 1")

- p-value = 1, alpha = .05

- Lot 1 is not statistically significant from the normal distribution and normality can be assumed. The mean falls within the 95% confidence interval.

### T-test for Lot 2

![T-test lot 2](/images/t_test_2.png "T-test lot 2")

- p-value = .6072, alpha = .05

- Lot 2 is not statistically significant from the normal distribution  and normality can be assumed. The mean falls within the 95% confidence interval.

### T-test for Lot 3

![T-test lot 3](/images/t_test_3.png "T-test lot 3")

- p-value = .04168, alpha = .05

- Lot 3 is statistically significant from the normal distribution and normality cannot be assumed. However, the mean falls within the 95% confidence interval.
