# zimmertr

TJ's GitHub profile repo. Its [`README.md`](README.md) is what the profile page shows. It is TJ's: don't edit it, and never restructure it.

This repo took a trimmed set of the files a new project starts with (zimmertr/yggdrasil record 0038). When a change here makes a decision, write its record under `docs/architectural-decision-records/`; when it needs `CONTRIBUTING.md` or a `docs/` page, add it in the same PR.

## Rules

- **Actions are pinned to commit SHAs** with the version in a comment. Dependabot bumps them.

## Issues

File issues with the `create-issue` skill from zimmertr/ai-config: the two-sentence summary, the six sections, the hemingway and humanizer passes, one priority, one type, the area labels and the session label. The skill reads the four things below from this section.

- **The reader**: TJ, who owns the profile.
- **The gates**: `PR Title / PR Title` and the three `Lint /` checks pass; the README changes only when TJ asks.
- **The constraints**: no secrets in the repo; the PR title is `type(scope): summary`.
- **The areas**: `profile` (the README), `ci` (the workflows and Dependabot), `security`.

## Working in this repo

- Work in a fresh clone in the session's scratchpad, never in TJ's checkout. Branch from the latest `origin/main`.
- Everything reaches main through a squash-merged PR. Never push to main.
- CI runs on zimmertr/yggdrasil's `pr-title` and `lint` modules, pinned by commit SHA with the version beside it. Dependabot bumps the pin, and a patch or minor merges itself after three days.
