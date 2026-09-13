# Reproducible Workflows

For every reported result, preserve enough information to reconstruct how it was produced.

## Track the full path, not only the final analysis

Record:

- raw input identity and version,
- preprocessing,
- filtering and exclusions,
- transformations,
- software and package versions,
- parameters and configuration,
- model specification,
- random seeds when relevant,
- output generation,
- manual decisions.

Reproducibility is often lost in small preprocessing steps rather than the headline model.

## Prefer executable workflows

A prose description of steps can drift away from what was actually run. When possible, encode the analysis as scripts, notebooks, pipelines, or workflow definitions that can regenerate outputs.

The goal is not maximal automation for its own sake. It is to reduce hidden state and make the computational history inspectable.

## Avoid manual data manipulation

Manual spreadsheet editing, copy/paste transformations, and undocumented GUI operations are difficult to reproduce and audit.

If a manual step is unavoidable:

- record the input state,
- record the action,
- record who made the decision and why,
- preserve the resulting artifact,
- make the step explicit in the workflow.

## Reproduce from a clean state

Before release, test whether the analysis can be rerun without relying on untracked local files or hidden environment state.

A useful test is whether another competent researcher—or your future self—can regenerate the key outputs from documented inputs.

## Preserve intermediate artifacts selectively

Do not save every temporary file forever, but preserve expensive, irreversible, or interpretation-critical stages so that failures can be localized without recomputing the entire pipeline.

## Source

- Sandve GK, et al. *Ten Simple Rules for Reproducible Computational Research.* https://doi.org/10.1371/journal.pcbi.1003285
