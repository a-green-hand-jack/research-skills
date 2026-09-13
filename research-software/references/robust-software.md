# Robust Research Software

Research software is robust when someone other than the original author can run it, understand failures, and obtain scientifically consistent outputs in the intended environments.

## Make execution repeatable

Avoid dependence on undocumented local state. Specify:

- dependencies and versions,
- configuration,
- required data/resources,
- runtime assumptions,
- deterministic settings or random seeds where relevant.

## Test scientific behavior

Tests should protect the properties that matter scientifically, not only whether the program runs.

Consider tests for:

- known input/output cases,
- numerical tolerances,
- edge cases,
- parsing and schema validation,
- invariants that should always hold,
- regression against previously validated results.

## Fail loudly and informatively

Validate inputs early. Error messages should help the user identify:

- what failed,
- the relevant state or parameter,
- likely corrective action.

Silent coercion or partial output can be more dangerous than a crash in scientific workflows.

## Separate algorithm from interface

Keep core computation separable from notebooks, GUIs, command-line wrappers, or web services when feasible. This supports testing and reuse across environments.

## Treat portability as a scientific property

If a result depends on one unrecorded machine configuration, it is fragile. Use environment specifications, containers, package locks, or equivalent mechanisms when they improve reproducibility.

## Source

- Taschuk M, Wilson G. *Ten simple rules for making research software more robust.* https://doi.org/10.1371/journal.pcbi.1005412
