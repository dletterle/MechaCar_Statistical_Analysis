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



