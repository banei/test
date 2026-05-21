# AGENTS.md

Instructions for AI coding agents working in this repository.

## Project overview

This is a minimal repository (`README.md` currently contains only a placeholder title). There is no application code, package manager, or CI configuration yet. Treat changes as greenfield unless the user specifies an existing stack.

## Repository layout

```
.
├── AGENTS.md    # Agent instructions (this file)
└── README.md    # Human-facing project description
```

When you add source code, tests, or tooling, update this file with real paths and commands.

## Development workflow

1. **Read context first** — Check `README.md`, the nearest `AGENTS.md` (if nested later), and existing files before editing.
2. **Minimize scope** — Change only what the task requires. Avoid drive-by refactors or unrelated formatting.
3. **Match conventions** — Follow naming, structure, and style already present in the repo. If none exist, use clear defaults and document them here.
4. **Verify when possible** — Run build, lint, and test commands once they exist. Do not claim success without command output.

## Build and test commands

No build or test toolchain is configured yet. When one is added, document exact commands here, for example:

```bash
# Example — replace with real commands after setup
# npm install
# npm run build
# npm test
```

Agents should run the documented commands before finishing tasks that touch buildable code.

## Code style

- Prefer small, focused diffs.
- Add comments only for non-obvious logic.
- Do not add tests unless requested or they meaningfully cover changed behavior.

## Git and pull requests

- Use descriptive branch names (e.g. `cursor/<short-description>` when working from automation).
- Write commit messages in complete sentences that explain *why*, not only *what*.
- Open or update a PR with a clear summary of changes and how they were verified.

## Security

- Do not commit secrets, API keys, or credentials.
- Do not disable security checks without explicit user approval.

## Updating this file

Keep `AGENTS.md` in sync with the repo. When you introduce a language, framework, or CI pipeline, add:

- Install and dependency commands
- Build, lint, and test commands
- Directory structure and important entry points
- Project-specific gotchas agents should know
