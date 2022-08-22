# Employee Promotion Prediction

A large MNC have 9 broad verticals across the organisation. One of the problem is identifying the right people for promotion (only for manager position and below) and prepare them in time.

The final promotions are only announced after the evaluation and this leads to delay in transition to new roles. Hence, company needs help in identifying the eligible candidates at a particular checkpoint so that they can expedite the entire promotion cycle.

Result of this model:
- Precision Train Score : 0.919831223628692
- Precision Test Score : 0.9603960396039604

## Project Background

A high number of promotions are an indication that our company was experiencing a lot of change. **Acquiring new business or merging with another organization all require major shifts in labor allocation**. People will take on new tasks and be promoted into various roles based on new needs.

high promotion rate means the company uses internal hiring so that employees can be promoted. Benefit of high promotion rate:
1. Reduced training and socializing time
2. Less external hiring cost
3. Less probability to quit / be fired

Currently company's employee promotion rate is 9%. Our goal is to `increase employee promotion rate by 25%` and `decrease total hiring cost up to 50%`. This can be achieved by knowing the factors that can affect the increment of the employee promotion rates and implementing our recommendations in business processes.

## Dataset Overview

Our data consist of 54808 rows (employees data), which are generated from 1 year historical employees data. There are 12 independent features and 1 target feature. Our target feature explain whether employee will get promotion or not. Data source : [link](https://www.kaggle.com/datasets/arashnic/hr-ana)

## Data Pre Processing

1. Handling Missing Values
2. Feature Encoding
3. Feature Selection
4. Handling Imbalaced Target 

## Modeling 

We use several algorithm, and those top 3 are:
1. Random Forest
2. Gradient Boost
3. XGBoost

**Scoring:**
we use Precision Score to prevent high number of False Positive (Predicted predicted to be promoted, actually didn't get promotion). Because if have certain number of False Positive, it more costly to get unqualified employees who get promotion.

**Result:**

Random Forest:
- Precision Train Score : 0.919831223628692
- Precision Test Score : 0.9603960396039604

## Recommendation :


1. Improve increment `avg_training_score` 30%
2. Improve increment `previous_year_rating` 10%

#### Recommendation result:
===================================================================
#### Training Score Impact After Business Recommendation Implementation
- Current Average avg_training_score = 60.0
- Average avg_training_score after implementing recommendation = 82

===================================================================
#### Promotion Impact After Business Recommendation Implementation
- Current Promotion Rate = 8.52%
- Simulation Promotion Rate After Recommendation = 24.63%
- Promotion Rate Increment =  16.11

===================================================================
#### Hiring Cost Impact After Business Recommendation Implementation
- Current Hiring Cost  = $ 44373900
- Hiring Cost After Implementing Recommendation = $ 36558016
- Percetage Hiring Cost Reduction = 21.38%

===================================================================
#### Talent recruited Impact After Business Recommendation Implementation
- Current Number of Talent Will Be Recruited = 10028
- New Number of Talent Will Be Recruited = 8262

===================================================================

