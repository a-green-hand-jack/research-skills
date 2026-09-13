# Source Discovery

Use this reference when a missing capability depends on external rules, changing procedures, or a large body of material.

## Source priority

Use the highest-ranked source that directly answers the decision:

1. First-party operational sources: the current conference or journal site, call for papers, author instructions, official template repository, submission-system help, policy page, or maintainer documentation.
2. Primary sources: the original paper, standard, specification, dataset card, or official release notes.
3. Trusted secondary sources: institutional guidance or a careful technical overview, used to clarify rather than replace a primary source.
4. Search snippets, forums, and personal posts: discovery hints only. Do not use them as the final authority for deadlines, policy, required formats, or compliance.

## Search recipe

Start with the capability and decision, not a broad topic. Useful query parts include:

- the exact venue, tool, standard, or organization name;
- the current cycle, version, or release;
- the artifact needed, such as `author guidelines`, `template`, `submission`, `FAQ`, or `policy`;
- `site:` restricted to the first-party domain when appropriate.

For an agent writing an ICML or ICLR paper, search separately for the current call for papers, author instructions, LaTeX or Word template, submission-system instructions, supplementary-material rules, review or anonymity policy, and post-submission updates. These may live on different official pages and may change independently.

## Capture and conflict handling

For every candidate, record what decision it supports and its freshness. Prefer a current page over an undated copy. If two official sources disagree, preserve both in the research notes, identify the newer or more specific rule, and do not silently resolve the conflict. If a required fact cannot be confirmed from an authoritative source, mark it as unresolved and make the generated skill ask for verification rather than inventing an answer.

Distinguish these statements in notes and in the generated skill:

- **Source fact:** directly supported by a cited source.
- **Inference:** a conclusion drawn from one or more source facts.
- **Local convention:** a repository or team preference that is not a universal rule.
- **Open question:** a missing or conflicting fact that needs fresh confirmation.

## Minimum evidence set

Do not stop at the first useful page when the task is operational. Collect enough evidence to cover the decisions the skill will make. For a submission workflow, that normally includes eligibility and dates, manuscript format, submission mechanics, review and anonymity requirements, supplementary material, and any post-submission constraints. Store links and retrieval metadata even when the source file itself cannot be redistributed.
