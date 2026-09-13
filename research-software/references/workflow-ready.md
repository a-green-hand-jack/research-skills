# Workflow-Ready Research Software

Software becomes easier for agents, pipelines, and workflow engines to use when inputs, outputs, configuration, and side effects are explicit.

## Expose a machine-usable interface

Prefer an interface that accepts explicit inputs and configuration and produces explicit outputs. Command-line interfaces, APIs, or library functions are usually easier to automate than GUI-only tools.

Avoid requiring users to edit source code or hidden config files for normal runtime choices.

## Make all consequential configuration visible

Parameters that can change scientific output should be externally configurable and recordable.

Do not rely on:

- hard-coded local paths,
- hidden environment variables without documentation,
- interactive prompts that cannot be logged,
- untracked defaults that change between runs.

## Separate human judgment from mechanical work

Automate calculation, file movement, and deterministic transformations.

When human judgment is scientifically necessary, create an explicit checkpoint:

1. workflow produces an interpretable report plus structured state,
2. human makes a decision,
3. decision is recorded as structured provenance,
4. workflow continues from that record.

Do not hide judgment inside an undocumented manual step.

## Prefer composable tools

A tool that performs one coherent responsibility is easier to test and combine. If software performs several independent operations, consider exposing them as separate subcommands or endpoints while sharing one codebase.

## Produce both human- and machine-readable outputs when useful

For agentic workflows, a useful pattern is:

- structured JSON/TSV/etc. for downstream computation,
- HTML/Markdown/report output for inspection.

## Source

- Brack P, et al. *Ten simple rules for making a software tool workflow-ready.* https://doi.org/10.1371/journal.pcbi.1009823
