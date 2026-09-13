# Skill Synthesis

Use this reference after the evidence has been collected and the capability needs to become an installable skill.

## Output contract

Every generated skill needs a folder with a `SKILL.md` containing concise YAML frontmatter:

```yaml
---
name: lowercase-and-hyphenated-name
description: What the skill does and when it should be used.
---
```

The body should contain only the decisions and actions that improve the target workflow:

1. Purpose and scope.
2. Trigger conditions and meaningful exclusions.
3. Core workflow or decision points.
4. Links to focused references, with instructions for when to read them.
5. Validation and completion criteria.

Move long source summaries, schemas, venue-specific procedures, examples, and troubleshooting into `references/`. Keep each reference focused. Do not load every reference by default when only one operating mode is relevant.

## Gap-to-skill transformation

Translate the research record into observable behavior:

| Research record | Skill instruction |
| --- | --- |
| User needs the current submission deadline | Find and cite the current official cycle page before stating a date |
| Several official pages govern the workflow | Check each page relevant to the decision and record conflicts |
| Template changes by venue or year | Retrieve the current official template instead of baking a stale copy into prose |
| Source material is copyrighted or access-restricted | Link and summarize with attribution; do not redistribute the full text |
| The agent cannot verify a required rule | Stop short of a confident claim and report the unresolved question |

For a conference-writing example, the resulting skill should help an agent discover the current ICML or ICLR requirements, obtain the correct template, explain the workflow, and draft or validate against those requirements. It should not hardcode a particular year's deadline or claim that one conference's rules apply to another.

## Quality gate

Before publishing a generated skill, check:

- the name and description are specific enough for discovery;
- the workflow produces files, decisions, or checks that can be inspected;
- every conditional reference is linked and routed from `SKILL.md`;
- source facts, inferences, and local conventions are distinguishable;
- time-sensitive claims require a fresh official-source check;
- no secrets, private session state, or unauthorized source copies are included;
- the skill validator passes and a realistic dry run reaches the intended output;
- the skill reports its sources, assumptions, and unresolved questions.

The goal is not to create the longest instruction file. The goal is to leave the next agent with a reliable, maintainable capability that can be updated when its sources change.
