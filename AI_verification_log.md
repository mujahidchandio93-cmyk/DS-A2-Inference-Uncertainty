# DS-A2 AI Use and Verification Log

## AI tool and tasks
**Tool:** ChatGPT.

AI assistance was used to clarify statistical concepts, develop and troubleshoot Python simulation code, interpret simulation outputs, organize project files, and prepare reproducibility documentation. The final analysis and interpretation remain the author's responsibility.

## Verification and execution
The notebook was executed in Google Colab using the **Run all** command, and the execution completed without reported errors. The power-analysis results and counterexample summary were exported as CSV files. Simulation figures were inspected in the notebook.

These checks support successful execution but do not, by themselves, establish that every statistical formula, assumption, or exported result is correct.

## Corrections and decisions
A DataFrame export initially failed because its columns had unequal lengths. The export code was corrected by providing two repetition-count entries, one for each statistical method.

The resulting counterexample table reported Type I error rates of 0.0478 for Welch's test and 0.0049 for the pooled-variance test.

## Interpretation and limitations
Under the specified simulated configuration, Welch's test had a rejection rate close to the nominal 0.05 level, whereas the pooled-variance test was substantially more conservative. This finding is specific to the simulation settings and should not be generalized to all sample sizes, variance patterns, or data-generating processes.

AI-generated code and interpretations are not independent validation. Statistical assumptions, formulas, confidence intervals, and consistency between the notebook and exported files should be checked separately.

## Reproducibility and final checks

To reproduce the analysis, open `DS_A2_Inference_Uncertainty_final.ipynb` in Google Colab or Jupyter and execute the cells in order. The notebook uses a documented random seed and records software version information. The expected exported result files are `DS-A2_power_simulation_results.csv` and `DS-A2_counterexample_results.csv`.

Before submission, the notebook outputs, exported CSV files, method note, figures, and final PDF should be checked for consistency and completeness. The GitHub repository should contain the intended final files.
