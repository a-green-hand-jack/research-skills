# Provenance and Automation

Provenance is the record of where an artifact came from and which operations and decisions produced it.

## Capture machine actions

For computational steps, capture:

- input identity,
- command or executable action,
- parameters/configuration,
- software version/environment,
- output identity,
- timestamps when relevant.

Prefer machine-generated logs when possible because manually maintained process notes can diverge from actual execution.

## Capture human decisions too

Automation does not eliminate scientific judgment. If a person chooses a threshold, excludes a sample, labels a case, resolves an ambiguous match, or changes a parameter after inspection, preserve that decision as part of provenance.

A useful pattern is:

- machine-readable input/output,
- human-readable report for judgment,
- explicit structured record of the human decision,
- next computational stage consumes that structured decision.

## Avoid hidden GUI-only workflows

A workflow that requires an unrecorded sequence of clicks is difficult to reproduce. Where practical, expose computation through scripts, APIs, command-line interfaces, or exported configuration.

## Make checkpoints inspectable

Long pipelines should expose intermediate states or logs sufficient to identify where a result changed. This helps both debugging and scientific audit.

## Keep provenance proportional

Do not generate enormous logs nobody can interpret. Preserve the information needed to explain and reproduce consequential decisions.

## Sources

- Sandve GK, et al. *Ten Simple Rules for Reproducible Computational Research.* https://doi.org/10.1371/journal.pcbi.1003285
- Brack P, et al. *Ten simple rules for making a software tool workflow-ready.* https://doi.org/10.1371/journal.pcbi.1009823
