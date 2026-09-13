# Research Skills

A compact family of Agent Skills distilled from high-value PLOS research-methods and scientific-practice guidance.

The package is designed for filesystem-native agents such as Codex and Claude Code. Each skill uses progressive disclosure:

1. The agent discovers a skill from the `name` and `description` in `SKILL.md`.
2. The agent reads the short `SKILL.md` only when the task matches.
3. The agent opens only the relevant files in `references/` for deeper operational guidance.

## Skills

- `scientific-writing` — structure, draft, diagnose, and revise research manuscripts.
- `literature-review` — scope, search, read, synthesize, and write reviews.
- `research-planning` — turn questions into defensible study and analysis plans.
- `peer-review` — review manuscripts and respond to reviewers.
- `research-collaboration` — start, run, and repair scientific collaborations.
- `open-science` — data management, provenance, reproducibility, and sharing.
- `research-software` — build, document, version, automate, and publish research software.

## Installation

Copy any skill directory into the skills directory used by your agent environment.

Typical layouts include:

```text
# Claude Code — project-scoped
.claude/skills/
  scientific-writing/
  literature-review/
  ...

# Claude Code — user-scoped
~/.claude/skills/
  scientific-writing/
  literature-review/
  ...

# Codex — project-scoped
.codex/skills/
  scientific-writing/
  literature-review/
  ...

# Codex — user-scoped
~/.codex/skills/
  scientific-writing/
  literature-review/
  ...
```

You can also install only the skills relevant to a project.

## Design rule

`SKILL.md` is deliberately short. Detailed research knowledge lives in `references/`, and each `SKILL.md` tells the agent which reference to read for a given task.

The material here is synthesized and paraphrased from PLOS sources rather than organized article-by-article. See [SOURCES.md](SOURCES.md) for attribution and provenance.
