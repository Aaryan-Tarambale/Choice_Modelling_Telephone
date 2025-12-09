# Choice_Modelling_Telephone
This project applies discrete choice modelling to understand how consumers choose between two telephone plans: budget and standard. Using a dataset of 196 individuals, five binary logit models were estimated with progressively richer specifications. These models evaluate how cost, household usage, income band, marital status, and residential area influence consumer preferences. All modelling was conducted in R using the Apollo package.
# Project Objectives
The goal of this project is to quantify and interpret the factors that drive the likelihood of a consumer selecting a standard telephone plan over a budget plan. Specifically, the project aims to:

1. Measure the sensitivity of consumers to plan cost

2. Assess whether demographic and usage variables improve model fit
  
3. Compare multiple model specifications using standard choice modelling metrics
  
4. Provide interpretable findings suitable for business decision-making
   
Each model is evaluated using:
i. Log-Likelihood at convergence

ii. Rho-squared and Adjusted Rho-squared

iii. AIC and BIC

iv. Statistical significance of estimated coefficients

All full model outputs are available in data/.
# Results Summary

### Cost as the dominant factor

Across all models, the cost coefficient is negative and statistically significant. This indicates that higher plan prices decrease the probability of selecting the standard option. The finding is robust across linear and log-cost specifications.

Limited influence of additional variables

Variables such as:
1. number of users
2. income band 20–30k
3. marital status
4. area type

show limited statistical significance and do not substantially improve model fit. Their inclusion results in only modest changes to log-likelihood, Rho-squared, AIC, and BIC values.

## Model comparison

Although later models introduce richer behavioural and demographic features, improvements in fit are incremental. Model choice therefore depends more on interpretability needs than on fit metrics alone.

## Overall interpretation

Consumer decision-making in this dataset is primarily driven by price sensitivity, with limited evidence that household or demographic characteristics strongly shift preferences between budget and standard plans.

## Conclusion

The modelling exercise demonstrates that cost is the central driver of telephone plan choice. While demographic and usage variables provide additional context, they do not substantially enhance predictive accuracy in the current dataset. The findings support the view that pricing strategy plays the most crucial role in influencing consumer uptake of standard plans.

## Future extensions may include:
1. Additional demographic variables
2. Expanded datasets to improve variability
3. Mixed logit models to account for random taste heterogeneity
4. Price elasticity estimation for strategic planning
