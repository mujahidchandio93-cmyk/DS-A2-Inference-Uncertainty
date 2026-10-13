# DS-A2 Method Note: Inference and Uncertainty

## Objective
This project uses simulation to investigate how sample size, population variability, and effect size influence statistical power and uncertainty in a two-group comparison.

## Estimand and hypotheses
The estimand is the difference between two population means. The null hypothesis is that the population mean difference equals zero; the two-sided alternative is that it is nonzero. The significance level is 0.05.

The simulated standardized effect sizes are 0, 0.2, 0.5, and 0.8. A standardized effect of 0.5 is used as a prespecified benchmark for a potentially meaningful effect in this simulation; it is not a clinically validated threshold for male infertility.

## Methods
Repeated simulations estimate rejection rates across combinations of sample size, population variability, and true effect size. Under the null hypothesis, the rejection rate estimates the Type I error rate. Under a nonzero effect, it estimates statistical power.

Monte Carlo standard errors quantify the simulation uncertainty arising from a finite number of repetitions. The counterexample compares Welch's two-sample t-test with the pooled-variance Student's t-test under unequal sample sizes and unequal population variances.

## Limitations
The results depend on the simulated distributions, parameter choices, number of repetitions, and random seed. They are not clinical findings or estimates from actual patients. Monte Carlo variability can cause estimated rejection rates to differ from their theoretical values.

The counterexample illustrates the behavior of the two tests under one specified configuration and does not establish that either test always performs better. Conclusions should therefore be limited to the simulated conditions rather than generalized to all data-generating processes.
