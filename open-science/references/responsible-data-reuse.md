# Responsible Data Reuse

Public availability does not automatically mean that a dataset is appropriate for every scientific question or free of legal, ethical, technical, and attribution constraints.

## Start from purpose, not availability

Use a dataset because it is scientifically suitable for the research question, not merely because it is easy to download.

Before analysis, ask:

- What population or process generated the data?
- What was the original collection purpose?
- Which variables are direct measurements versus derived fields?
- What selection mechanisms shaped the dataset?
- Does the dataset represent the target population or environment?

## Read the reuse conditions

Check licenses, data-use agreements, embargoes, consent limitations, privacy constraints, and repository-specific terms.

Do not infer that "public" means "unrestricted."

## Inspect provenance and semantics

Before modeling, understand:

- dataset version and release date,
- schema and units,
- missing-value conventions,
- preprocessing already performed,
- sample identifiers and possible duplicates,
- known batch effects or collection artifacts,
- links to source publications and documentation.

## Verify integrity programmatically when possible

For large or important datasets, prefer scripted downloads and preserve checksums, file manifests, query parameters, accession identifiers, or other stable provenance so the acquisition itself can be reproduced.

## Avoid ethical laundering through public data

A dataset can be technically accessible while still raising ethical concerns about consent, vulnerable populations, re-identification, or harmful downstream use. Consider the context in which the data were created and the consequences of the proposed reuse.

## Give data producers credit

Cite datasets and repositories according to their requested citation practice. Preserve identifiers so downstream artifacts can trace back to the exact source.

## Share derived artifacts responsibly

When publishing cleaned data, features, embeddings, models, or reprocessed outputs, preserve links to upstream provenance and apply appropriate licenses/access controls. Do not accidentally make restricted information more accessible through derived products.

## Sources

- Oza VH, et al. *Ten simple rules for using public biological data for your research.* https://doi.org/10.1371/journal.pcbi.1010749
- Zook M, et al. *Ten simple rules for responsible big data research.* https://doi.org/10.1371/journal.pcbi.1005399
