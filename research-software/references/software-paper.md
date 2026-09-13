# Writing a Scientific Software Paper

A software paper must demonstrate both scientific value and software usability. A novel algorithm that nobody can run is difficult to evaluate; polished software without a meaningful scientific purpose may not justify a research paper.

## Decide what kind of paper it is

Common cases include:

- a paper whose main contribution is the software itself,
- a research paper in which new software is a critical enabling component.

The structure and evaluation should match the contribution.

## State the problem the software solves

Explain:

- who has the problem,
- why existing tools are insufficient,
- what capability the software adds,
- what assumptions or scope limits apply.

Do not substitute a feature list for a scientific contribution.

## Evaluate against meaningful alternatives

Choose benchmarks, datasets, and competing tools that answer the scientific question rather than merely making the new software look favorable.

Report tradeoffs such as:

- accuracy,
- runtime,
- memory,
- robustness,
- usability,
- scalability,
- interpretability,
- domain limitations.

## Make the software inspectable

A strong software paper should point to:

- accessible source or distribution when possible,
- documentation,
- version used in the paper,
- license,
- reproducible examples,
- test or benchmark data,
- citation information.

## Plan for longevity

Websites disappear and dependencies evolve. Use redundant durable references: repository, archived release, DOI, documentation, and explicit version information in the paper.

## Sources

- Romano JD, Moore JH. *Ten simple rules for writing a paper about scientific software.* https://doi.org/10.1371/journal.pcbi.1008390
- Lee BD. *Ten simple rules for documenting scientific software.* https://doi.org/10.1371/journal.pcbi.1006561
