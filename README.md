# MechaCar_Statistical_Analysis

## Part 1 - Linear Regression to Predict MPG

### Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

Vehicle length and ground clearance (as well as intercept) provided a non-random amount of variance to the mpg values.

![linear_summary_table](https://user-images.githubusercontent.com/110419577/210616884-3d31a688-66fe-4b2e-9729-4627bf03d33d.png)

### Is the slope of the linear model considered to be zero? Why or why not?
The slope of the linear model is not considered to be zero as r is measured at 0.7149. This is strong evidence of a positive linear relationship.

### Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

This linear model does predict mpg ofof MechaCar prototypes effectively. The multiple R-squared is at 0.7149, which is considered strong. However, the P-value is under .05, which means data not normally distributed and similar results may not be found if tested again. It may be a good next step to complete simple linear regression models to fully understand the data. 

## Part 2 - Summary Statistics on Suspension Coils

### Total Summary Dataframe
![total_summary_df](https://user-images.githubusercontent.com/110419577/210623715-175ce265-d333-4630-a572-60491e4fa7cd.png)

### Lot Summary Dataframe
![lot_summary_df](https://user-images.githubusercontent.com/110419577/210623744-5f34e407-d1fc-4b30-ab3c-177807d60983.png)

### The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

The current manufacturing data meets the design specification for all manufacturing lots in total and for Lot 1 and Lot 2 individually. The design specifications dictate that the variation of the suspension coils must not exceed 100 pounds per square inch. The total summary meets this with a variance of 62.3. The individual variances for Lot 1 and Lot 2 meet this as well at 0.98 and 7.47 respectively. However, Lot 3 reflects of variance of 170.29, well over the 100 pound requirement.

## Part 3 - T-Tests on Suspension Coils

Assuming our significance level is at the standard 0.05 percent, our p-value is above our significance level for the total t-test as well as t-tests for Lot 1 and Lot 2. Therefore, we do not have sufficient evidence to reject the null hypothesis, and we would state that the means for the total, Lot 1 and Lot 2 are statistically similar. However the p-value for Lot 3 is under 0.05 percent at 0.42. Therefore, we do have sufficient evidence to reject the null hypothesis and would state the two means for Lot 3 are not statistically similar.

![t-test_total](https://user-images.githubusercontent.com/110419577/210627517-fed36a16-bb00-48d3-9669-4f82b4a4f358.png)

![t-test_lot1](https://user-images.githubusercontent.com/110419577/210627511-ba0161c3-112e-4c0d-a987-b6623083de27.png)
![t-test_lot2](https://user-images.githubusercontent.com/110419577/210627513-dc81651f-79b3-49bc-a26c-303f4cfd1742.png)
![t-test_lot3](https://user-images.githubusercontent.com/110419577/210627514-b35c5cfc-8617-4bde-a235-daaa4e9ba2a5.png)



## Part 4 - Study Design: MechaCar vs Competition

### Write a short description of a statistical study that can quantify how the MechaCar performs against the competition. In your study design, think critically about what metrics would be of interest to a consumer: for a few examples, cost, city or highway fuel efficiency, horse power, maintenance cost, or safety rating.

### What metric or metrics are you going to test?

I am going to test for cost and safety rating to establish the safest vehicles and how this compares to their value. This will be compared against MechaCar vehicles as well as competitor's vehicles to understand how desireable MechaCar vehicles are to a customer interested in safety.

### What is the null hypothesis or alternative hypothesis?

Null Hypothesis - If ratings are not higher in MechaCar vehicles than in the competition, then we can conclude MechaCar vehicles do not rate higher than the competition.

Alternative Hypothesis - If ratings are higher in MechaCar vehicles compared to the competition, we can conclude MechaCar vehicles rate higher than the competition.

### What statistical test would you use to test the hypothesis? And why?
I would utilize two-way ANOVA to test the means of a two different independent variables (cost and safety rating) with multiple groups (MechaCar vehicles and competitor vehicles). This will establish average safety rating and cost under all MechaCar vehicles to compare with competitors.


### What data is needed to run the statistical test?
I would need data for both MechaCar vehicles and competitor vehicles. This data would include make, model, price and safety rating. 
