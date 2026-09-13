# Scientific Software Documentation

Documentation should let a new user answer: what does this software do, who is it for, how do I run it, what do inputs/outputs mean, and how do I cite it?

## Document while developing

Do not defer all documentation until the end. Capture intent and non-obvious reasoning when it is fresh.

Use meaningful names and comments to explain why code exists or why a non-obvious decision was made. Avoid comments that simply restate syntax.

## Provide layered documentation

### Project-level

Include:

- purpose,
- intended audience,
- problem solved,
- installation,
- minimal example,
- license,
- citation.

### Interface-level

For functions, commands, APIs, and file formats document:

- purpose,
- inputs and types,
- units where relevant,
- outputs,
- defaults,
- error behavior,
- side effects.

### Task-level

Provide worked examples that map real scientific tasks to commands or code.

## Keep documentation executable where possible

Examples that are automatically tested are less likely to become stale.

If a tutorial depends on a specific release, say so.

## Document failure modes

Explain common mistakes and make error messages actionable. A user who reaches an error should not need intimate knowledge of the source code to understand the next step.

## Tell users how to cite the software

Provide a stable citation path, such as a DOI and machine-readable citation metadata where appropriate. Make the citation visible in the repository rather than expecting users to reverse-engineer it from a paper.

## Source

- Lee BD. *Ten simple rules for documenting scientific software.* https://doi.org/10.1371/journal.pcbi.1006561
