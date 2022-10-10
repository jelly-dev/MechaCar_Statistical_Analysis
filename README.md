# MechaCar_Statistical_Analysis

## Overview
- AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has requested a review of the production data for insights that may help the manufacturing team. The analysis includes the following:

    - Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes

    - Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
    - Run t-tests to determine if the manufacturing lots are statistically different from the mean population

    - Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, a summary is included.

## Linear Regression to Predict MPG
- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
    - p-value of coefficients should be compared to alpha = .05 level of significance to verify if statistically significant.
        - mpg: 0 < .05 significant, <b>non-random</b>
        - vehicle length: 0 < .05, significant, <b>non-random</b>
        - vehicle weight: .08 > .05 not significant, random
        - spoiler angle: .31 > .05 not significant, random
        - ground clearance: 0 > .05 significant, <b>non-random</b>
        - AWD: .19>=.05 not statistically significant, random amount of variance

- Is the slope of the linear model considered to be zero? Why or why not?
    - Although some of the slopes of the variables come close to zero, the linear regression formula results in a non-zero slope.

- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
    - The r-squared value is .7149, meaning the dataset is effective and shows a strong correlation. However, there may be other unmeasured variables that play into the mpg that are needed for the most effective prediction.

## Summary Statistics on Suspension Coils

### Total Manufacturing Lot Summary

### Summary per Manufacturing Lot

- The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

## T-Tests on Suspension Coils
- briefly summarize your interpretation and findings for the t-test results. Include screenshots of the t-test to support your summary.

### T-test for All Lots

### T-test for Lot 1

### T-test for Lot 2

### T-test for Lot 3

## Study Design: MechaCar vs Competition
- Write a short description of a statistical study that can quantify how the MechaCar performs against the competition. In your study design, think critically about what metrics would be of interest to a consumer: for a few examples, cost, city or highway fuel efficiency, horse power, maintenance cost, or safety rating.

    - What metric or metrics are you going to test?

    - What is the null hypothesis or alternative hypothesis?

    - What statistical test would you use to test the hypothesis? And why?

    - What data is needed to run the statistical test?
