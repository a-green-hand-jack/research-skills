# Study Design and Bias

Study design should make the intended inference hard to explain away by bias, confounding, measurement error, or dependence.

## Start from the inference

Write the intended conclusion first, then ask what observations would justify it.

For a causal claim, identify plausible alternative causes. For a predictive claim, identify what information will be available at deployment time. For a descriptive claim, define the target population and measurement process.

## Map sources of bias by stage

Bias can enter through:

- who or what is selected,
- allocation or exposure assignment,
- measurement,
- missingness,
- data processing,
- analytic flexibility,
- selective reporting.

Do not use "bias" as a generic criticism. State the mechanism by which a design feature could systematically change the estimate or conclusion.

## Use controls that attack alternatives

A control is useful when it distinguishes the preferred explanation from a plausible alternative.

For each important control, write:

> Without this control, the result could also be explained by ______.

If the blank is unclear, the control may be ritual rather than inference-driven.

## Respect the unit of independence

Do not treat repeated measurements, technical replicates, clustered observations, or samples from the same experimental unit as independent simply because they create more rows in a dataset.

Identify:

- experimental unit,
- observational unit,
- repeated/clustered structure,
- level at which treatment or exposure varies.

Pseudoreplication can create false precision.

## Reduce avoidable measurement bias

Prefer objective and standardized measurements when feasible. Use clear operating procedures, consistent definitions, and documented data handling.

If measurement is subjective, consider blinding, multiple raters, reliability checks, or explicit adjudication rules where appropriate.

## Make design limitations explicit before data collection

Ask before starting:

- What conclusion will this design *not* support?
- What confounders cannot be controlled?
- Which population will the result not generalize to?
- Which outcome definitions are proxies rather than direct measurements?

A known limitation can often be mitigated; an unrecognized one becomes a post hoc surprise.

## Source

- Schwab S, et al. *Ten simple rules for good research practice.* https://doi.org/10.1371/journal.pcbi.1010139
