# Provenance and Licensing

Use this reference when downloading web pages, PDFs, templates, repositories, or other source artifacts into a local research workspace.

## Suggested workspace

Keep source collection separate from the final skill until synthesis is complete:

```text
work/skill-research/<skill-slug>/
├── manifest.yaml
├── notes.md
└── sources/
    ├── source-001.html
    └── source-002.pdf
```

The exact scratch directory may vary by environment. It should be easy to delete, excluded from the generated skill unless needed, and distinct from any user data or production directory.

## Manifest fields

Use one record per source. YAML or JSON is acceptable; keep the fields stable enough for another agent to audit.

```yaml
sources:
  - id: source-001
    title: Current author instructions
    publisher: Official organization
    url: https://example.org/author-instructions
    accessed_at: 2026-09-13T00:00:00Z
    published_or_updated: unknown
    version_or_commit: null
    source_type: first-party
    local_path: sources/source-001.html
    sha256: record-if-saved
    license_or_access: link-only; redistribution not confirmed
    supports:
      - manuscript format
      - submission requirements
```

Use the actual retrieval time and checksum. Do not fill unknown values with guesses. For a Git repository, record the commit or tag used; for a web page, record the access date and any visible update date.

## Retention rules

- Retain downloaded artifacts in the scratch workspace only when they are useful for reproducibility and permitted by their license or access terms.
- For material whose redistribution is unclear, retain the URL, metadata, checksum, and original notes; do not copy the full text into the public skill repository.
- For permissively licensed templates or reference data, preserve the license and attribution alongside the retained file.
- Use short excerpts only when needed to explain a transformation, and link to the original source. Do not turn the generated skill into a mirror of the source material.
- Scrub credentials, cookies, private URLs, session data, and personal information before a source record leaves the local workspace.

## Final provenance

The generated skill should link to a curated source list or provenance note. It should say whether the content is copied, paraphrased, summarized, or independently inferred, and it should state that source organizations do not endorse the generated skill unless explicit endorsement exists.
