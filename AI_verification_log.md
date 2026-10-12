# DS-A2 AI Use and Verification Log

## AI tool and tasks
Tool: ChatGPT.

AI assistance was used to clarify statistical concepts, develop and troubleshoot Python simulation code, interpret simulation outputs, organize project files, and plan reproducibility documentation.

## Verification and execution
The notebook was executed in Google Colab using the Run all command. The execution completed without reported errors. The power-analysis results and counterexample summary were exported as CSV files. The simulation figures were inspected in the notebook.

## Corrections and decisions
A DataFrame export initially failed because its columns had unequal lengths. The export code was corrected by providing two repetition-count entries, one for each statistical method. The resulting counterexample table reported a Type I error rate of 0.0478 for Welch's test and 0.0049 for the pooled-variance test.

## Interpretation and limitations
Under the simulated configuration, Welch's test produced a rejection rate close to 0.05, whereas the pooled-variance test was more conservative. This finding applies to the specified simulation and should not be generalized to all settings.

AI-generated code and interpretations are not independent validation. Further checks of statistical assumptions, formulas, confidence intervals, and agreement between the notebook and exported files are required before submission.

## Remaining checks
- Confirm that the notebook runs from top to bottom in a fresh runtime.
- Verify the exported CSV files against the notebook outputs.
- Check that all required figures and analyses are included.
- Confirm that the method note accurately describes the implemented methods.
- Create and verify the final PDF and versioned GitHub repository.
