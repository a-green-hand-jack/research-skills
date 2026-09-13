# Research Skills

A compact family of Agent Skills distilled from high-value PLOS research-methods and scientific-practice guidance.

## Attribution

Much of the guidance in this project is derived from material published by [PLOS](https://plos.org/), especially the PLOS Computational Biology *Ten Simple Rules* series. The source material has been distilled, paraphrased, reorganized, and adapted into agent-oriented skills; it is not reproduced article-by-article. See [SOURCES.md](SOURCES.md) for the detailed attribution and source list. This project is independent and is not affiliated with or endorsed by PLOS.

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

The recommended installation method is the standard [`skills`](https://github.com/vercel-labs/skills) CLI, which runs through `npx` and supports Codex, Claude Code, OpenCode, Cursor, and other compatible agents.

Install all skills globally for your user account:

```bash
npx skills add a-green-hand-jack/research-skills -g -y
```

Install all skills for the current project instead:

```bash
npx skills add a-green-hand-jack/research-skills -y
```

Install only selected skills:

```bash
npx skills add a-green-hand-jack/research-skills \\
  --skill scientific-writing \\
  --skill literature-review \\
  -g -y
```

To target a specific agent, add its name with `-a`, for example `-a codex` or `-a claude-code`.

### Manual installation

You can also copy any skill directory into the skills directory used by your agent environment.

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
