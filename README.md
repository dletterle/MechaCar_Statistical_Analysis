# MechaCar_Statistical_Analysis
# Background

A few weeks after starting his new role, Jeremy is approached by upper management about a special project. AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

In this challenge, you’ll help Jeremy and the data analytics team do the following:
  * Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
  * Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
  * Run t-tests to determine if the manufacturing lots are statistically different from the mean population
  * Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.

In order to complete the above challenge the following deliverables will be met: 
  * Deliverable 1: Linear Regression to Predict MPG
  * Deliverable 2: Summary Statistics on Suspension Coils
  * Deliverable 3: T-Test on Suspension Coils
  * Deliverable 4: Design a Study Comparing the MechaCar to the Competition


# Deliverable 1: Linear Regression to Predict MPG

<img width="389" alt="Linear Regression to Predict MPG" src="https://user-images.githubusercontent.com/99268646/171061713-4d66971f-e8d2-47c0-b535-3eb4e5de064a.png">

**Statistical Summary**
 
 mpg = (6.267)vehicle_length + (0.0012)vehicle_weight + (0.0688)spoiler_angle + (3.546)ground_clearance + (-3.411)AWD + (-104.0)
 
  * The variables/coefficients that provide a non-random amount of variance to the mpg values in the dataset are: vehicle length and vehicle ground clearance. This means the vehicle length and vehicle ground clearance have a significant impact on mpg for MechaCar prototype 
  * Because the p-value is 5.35e-11 (and smaller than the assumed level of 0.05%) there is sufficient evidence to reject the null hypothesis meaning the slope of the linear model is not 0
  * Because the r-square value is 0.7140 it means that approximately 71% of all mpg predictions will correctly determined by this regression analysis and so it is an effective model to predict prototypes

# Deliverable 2: Summary Statistics on Suspension Coils

<img width="335" alt="total_summary" src="https://user-images.githubusercontent.com/99268646/171063227-6f9ec13e-ec23-48b8-8ac5-39189614ba94.png">

<img width="451" alt="lot_summary" src="https://user-images.githubusercontent.com/99268646/171063231-34a40890-9dd2-4238-8b61-56cb59b8d0d4.png">

**Statistical Summary**

Because the variance of the coils is 62.29 PSI and withing the 100 PSI variance requirement, the design specifications for the MechaCar suspension coils meet the design specifications in total.

At each lot individually, Lot 1 and Lot 2 are well within the 100 PSI variance requirement at 0.98 PSI and 7.47 PSI. But Lot 3 has a variance of 170.29 PSI and does not meet the design specification. So the total variance would be much closer if Lot 3 did meet the correct specifications, and therefore should be reviewed further for better compliance. 

# Deliverale 3: t-Tests on Suspension Coils

<img width="664" alt="T-Tests on Suspension Coils" src="https://user-images.githubusercontent.com/99268646/171064125-1aac5753-ac5d-40a5-8ea2-7669122caf20.png">

The true mean of the sample is 1498.78 with a p-value of 0.06 which is higher than the standard significant level of acceptance of 0.05 so therefore we must accept the null hypothesis because there is not enough evidence to reject it. The mean of all three manufacturing lots is statistically similar to the population mean (1,500 pounds per square inch). 

<img width="293" alt="T-Tests on Suspension Coils_lot" src="https://user-images.githubusercontent.com/99268646/171064976-fbb955c6-462a-489c-85b1-ae0a70b1cce0.png">

Looking at the individual lots: 
 * Lot 1: the sample mean is 1500 and the p-value is 1 which is more than the significance level 0.05 so we must accept the null hypothesis
 * Lot 2: the sample mean is 1500.02 and the p-value is 0.61 which is more than the significance level 0.05 so again we must accept the null hypothesis 
 * Lot 3: the sample mean is 14.96.14 and the p-value is 0.04 which is less than the significan level 0.05 so we can reject the null hypothesis 

# Deliverable 4: Study Design: MechaCar vs Competition

To conduct a statistical study that can quantify how the MechaCar performs against the competition, certain metrics need to be considered:  
 * Fuel efficiency: MPG, horsepower, gasoline vs hybrid vs electric 
 * Monetary values: price of the vehicle, re-sale opportunities, maintenance/upkeep 
Hypothesis:
 * Null Hypothesis - MechaCar is priced correctly based on its performance of key metrics and factors
 * Alternate Hypothesis - MechaCar is not priced correctly based on its performance of key metrics and factors 
I would use linear regression as statistical method to test the hypothesis because there are multiple metrics and factors to review and would also aid in reviewing the correlation between each variable and the greatest determinant of price  
The data needed to run the statistical test would be divided into two categories and then ran in each separate category. So there would need to be a category for fuel efficiency and the following variables would need to be reviewed: MPG, horespower, gasoline vs hybrid vs electric; and a category regarding monetary variables including: price of the vehicle, re-sale price, and maintenance/upkeep on the vehicle on a yearly basis. 
