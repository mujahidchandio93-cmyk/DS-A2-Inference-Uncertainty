# DS-A2 AI Use and Verification Log

## AI tool and tasks

**Tool:** ChatGPT.

AI assistance was used to clarify statistical concepts, develop and troubleshoot Python simulation code, interpret simulation outputs, organize project files, and prepare reproducibility documentation. The author is responsible for the final analysis, verification, and interpretation.

## Verification and execution

The notebook was executed in Google Colab using the **Run all** command and completed without reported errors. The power-analysis results and counterexample summary were exported as CSV files, and the simulation figures were inspected.

Successful execution confirms that the notebook ran, but it does not establish that every formula, statistical assumption, or result is correct. Before submission, the simulation formulas, rejection-rate calculations, and consistency between notebook outputs and exported CSV files should be checked.

## Corrections and decisions

A DataFrame export initially failed because its columns had unequal lengths. The export code was corrected by providing two repetition-count entries, one for each statistical method.

The resulting counterexample table reported Type I error rates of 0.0478 for Welch's test and 0.0049 for the pooled-variance test. These values should be interpreted in the context of the specified simulation configuration.

## Interpretation and limitations

Under the simulated conditions, Welch's test had a rejection rate close to the nominal 0.05 level, whereas the pooled-variance test was substantially more conservative. This result is configuration-specific and should not be generalized to all sample sizes, variance patterns, or data-generating processes.

The comparison illustrates why the assumptions underlying a statistical test matter. It also demonstrates that a method can produce misleading inferential results when its assumptions are poorly matched to the data. Simulation results provide evidence about the conditions tested, not a universal guarantee of performance.

## Reproducibility and final checks

To reproduce the analysis, open `DS_A2_Inference_Uncertainty_final.ipynb` in Google Colab or Jupyter and execute the cells in order. The notebook documents the random seed and software version information. The expected exported result files are `DS-A2_power_simulation_results.csv` and `DS-A2_counterexample_results.csv`.

Before submission, check the notebook outputs against the exported CSV files and confirm that the method note, figures, and final PDF report consistent results. Any verification claims should reflect checks actually performed by the author. The GitHub repository should contain the intended final files.
