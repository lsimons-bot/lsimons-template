# Agent Instructions for lsimons-$project

<!-- Replace $project with your project name and update this description -->
Brief project description.

## Quick Reference

<!-- Update these commands for your project -->
- **Setup**: `uv venv && uv pip install -e .`
- **Test**: `uv run pytest`
- **Lint**: `uv run ruff check . && uv run pyright`
- **Format**: `uv run ruff format .`

## Structure

<!-- Document your project structure here -->

## Guidelines

**Code quality:**
- Full type annotations (pyright: 0 errors)
- Tests for all functionality
- ruff for linting and formatting

## Commit Message Convention

Follow [Conventional Commits](https://conventionalcommits.org/):

**Format:** `type(scope): description`

**Types:** `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `build`, `ci`, `perf`, `revert`, `improvement`, `chore`

## Session Completion

Work is NOT complete until `git push` succeeds.

1. **Quality gates** (if code changed):
   ```bash
   uv run pytest
   uv run ruff check . && uv run pyright
   ```

2. **Push**:
   ```bash
   git pull --rebase && git push
   git status  # must show "up to date with origin"
   ```

Never stop before pushing. If push fails, resolve and retry.
