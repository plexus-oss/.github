# Contributing to Plexus

Thanks for your interest in contributing! This guide covers the basics for all repos in the `plexus-oss` organization.

## Reporting Bugs

- Search [existing issues](https://github.com/plexus-oss) first to avoid duplicates
- Use the **Bug Report** issue template
- Include reproduction steps, expected vs actual behavior, and your environment

## Requesting Features

- Use the **Feature Request** issue template
- Describe the problem or use case, not just the solution
- Keep requests focused on a single idea

## Submitting Pull Requests

1. Fork the repo and create a branch from `main`
2. Make your changes, keeping the scope small and focused
3. Follow the existing code style and patterns in that repo
4. Fill out the PR template completely
5. Link the related issue

### PR Expectations

- **Describe what changed** and why
- **Link an issue** when one exists
- **Keep scope small** — one concern per PR
- **Tests pass** before requesting review
- **No breaking changes** without discussion first

## Development Setup

Each repo has its own setup instructions:

- **[agent](https://github.com/plexus-oss/agent)** — Python SDK (`pip install -e ".[dev]"`)
- **[c-sdk](https://github.com/plexus-oss/c-sdk)** — C library (see repo README for build instructions)
- **[ui](https://github.com/plexus-oss/ui)** — React components (`pnpm install`)

## Code Style

- Follow existing patterns in whichever repo you're contributing to
- No style wars — consistency with the file you're editing wins
- If the repo has a linter or formatter configured, use it

## Questions?

Join our [Discord](https://discord.gg/plexus) for help and discussion.
