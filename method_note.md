# DS-A2 Method Note: Inference and Uncertainty

## Objective
This project uses simulation to investigate how sample size, population variability, and effect size influence statistical power and uncertainty in a two-group comparison.

## Estimand and hypotheses
The estimand is the difference between two population means. The null hypothesis is that the population mean difference equals zero; the alternative hypothesis is that it is nonzero. The significance level is 0.05. The simulated effect sizes are 0, 0.2, 0.5, and 0.8 standardized units. The minimum meaningful effect should be justified in the notebook according to the project context.

## Methods
Repeated simulation estimates rejection rates across combinations of sample size, population standard deviation, and true effect size. The estimated rejection rate under a nonzero effect represents statistical power; under a zero effect, it estimates the Type I error rate. Monte Carlo standard errors quantify simulation uncertainty. The counterexample compares Welch's two-sample t-test with the pooled-variance Student's t-test under unequal sample sizes and unequal population variances.

## Limitations
The results depend on the simulated distributions, parameter choices, and random seeds. They are not clinical findings or estimates from actual patients. Monte Carlo error can cause small deviations from the nominal significance level. The counterexample demonstrates behavior under one specified configuration and does not establish that either test always performs better.
