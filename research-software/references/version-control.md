# Version Control and Releases

Version control is the scientific history of code and related project artifacts.

## Track meaningful project changes

Use Git or equivalent version control for:

- source code,
- analysis scripts,
- configuration,
- documentation,
- small text-based metadata,
- manuscripts when appropriate.

Avoid committing credentials, secrets, or restricted data.

## Make commits interpretable

Prefer commits that represent coherent changes. A useful history helps answer:

- when behavior changed,
- why it changed,
- which version produced a result,
- who made the change.

## Use branches or pull requests for nontrivial changes

Separate experimental development from the stable line of work. Review changes that alter scientific behavior, data processing, or key outputs with particular care.

## Mark publication states

Tag or release the exact software state associated with a paper, dataset, or major analysis. Where possible, archive that release in a repository that provides a persistent identifier.

A paper should not point only to a moving default branch.

## Use issues for durable project memory

Track bugs, planned improvements, known limitations, and unresolved scientific implementation questions rather than relying only on private messages.

## Source

- Perez-Riverol Y, et al. *Ten Simple Rules for Taking Advantage of Git and GitHub.* https://doi.org/10.1371/journal.pcbi.1004947
