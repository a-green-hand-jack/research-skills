# Statistical Reasoning

Statistics should connect data to a scientific question. Do not begin with "Which test should I use?" before deciding what quantity or hypothesis the data need to inform.

## Start with the scientific target

Identify:

- the estimand or target quantity,
- the comparison or prediction of interest,
- the unit of inference,
- relevant sources of variability,
- what uncertainty must be represented.

Only then choose a model or test.

## Make assumptions part of the analysis

Every model encodes assumptions about the data-generating process. Check those that materially affect the conclusion.

Possible concerns include:

- independence,
- distributional form,
- linearity,
- measurement error,
- missingness,
- exchangeability,
- model specification,
- selection effects.

Use diagnostics, sensitivity analyses, and alternative specifications when they illuminate robustness.

## Do not let software define the question

Statistical software provides procedures, not scientific intent. A method should be explainable in terms of how it answers the substantive question.

The Methods section should make that connection explicit rather than naming a package or function as if the tool were the rationale.

## Treat significance as graded evidence, not a switch

A p-value below an arbitrary threshold is not the same as a scientifically important effect, and a value above the threshold is not proof of no effect.

Report effect sizes and uncertainty. Interpret statistical evidence alongside study design, prior knowledge, multiplicity, model assumptions, and practical relevance.

Avoid language that turns a threshold crossing into discovery by itself.

## Separate exploration from confirmation

Extensive data exploration can reveal important patterns, but inferential quantities computed after many unrecorded choices may no longer have their nominal interpretation.

When possible:

- validate discoveries in independent data,
- separate exploratory and confirmatory phases,
- report analytic flexibility,
- preregister primary analyses for confirmatory work.

## Reproducibility is part of statistical quality

Keep analyses scripted and traceable. Record transformations, model formulas, software versions, random seeds where relevant, and the path from raw data to reported numbers.

## Sources

- Kass RE, et al. *Ten Simple Rules for Effective Statistical Practice.* https://doi.org/10.1371/journal.pcbi.1004961
- Schwab S, et al. *Ten simple rules for good research practice.* https://doi.org/10.1371/journal.pcbi.1010139
