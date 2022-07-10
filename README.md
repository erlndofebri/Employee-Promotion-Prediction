# Employee Promotion Prediction

A large MNC have 9 broad verticals across the organisation. One of the problem is identifying the right people for promotion (only for manager position and below) and prepare them in time.

The final promotions are only announced after the evaluation and this leads to delay in transition to new roles. Hence, company needs help in identifying the eligible candidates at a particular checkpoint so that they can expedite the entire promotion cycle.

The result of this project is that we managed to increase employees promotion rate by **49.43%** and also decrease  total hiring cost up to **80.89%**. We have also analyzed the most important factors affecting promotion rate with their respective correlations. We also provide rational and achieveable recommendations that can be applied by the relevant team so we can increase employees promotion rate and decrease total hiring cost.

This is also meet the `pareto principle`: We use about `20% effort to get 80% result`, because through this recommendation we only need to improve increment `avg_training_score` 13.5% and improve increment `previous_year_rating` 10% give the result 80.89% total hiring cost reduction

# Project Background

A high number of promotions are an indication that our company was experiencing a lot of change. **Acquiring new business or merging with another organization all require major shifts in labor allocation**. People will take on new tasks and be promoted into various roles based on new needs.

high promotion rate means the company uses internal hiring so that employees can be promoted. Benefit of high promotion rate:
1. Reduced training and socializing time
2. Less external hiring cost
3. Less probability to quit / be fired

Currently company's employee promotion rate is 9%. Our goal is to `increase employee promotion rate by 25%` and `decrease total hiring cost up to 50%`. This can be achieved by knowing the factors that can affect the increment of the employee promotion rates and implementing our recommendations in business processes.

# Dataset Overview

Our data consist of 54808 rows (employees data), which are generated from 1 year historical employees data. There are 12 independent features and 1 target feature. Our target feature explain whether employee will get promotion or not. 

# Data Pre Processing

1. Handling Missing Values
2. Feature Encoding
3. Feature Selection
4. Handling Imbalaced Target 

# Modeling 

We use several algorithm, and those top 3 are:
1. Random Forest
2. Gradient Boost
3. XGBoost

**Scoring:**
we use Precision Score to prevent high number of False Positive (Predicted predicted to be promoted, actually didn't get promotion). Because if have certain number of False Positive, it more costly to get unqualified employees who get promotion.

**Result:**

Random Forest:
1. Train Precision Score : 0.99
2. Test Precision Score : 099

# Recommendation :

1. Improve increment `avg_training_score` 13.5%
2. Improve increment `previous_year_rating` 10%
3. With these two recommendation above, company can **increase 49.43% promotion rate** and **reduce up to 80.89% total hiring cost**



