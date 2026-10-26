# Repository Guidelines

## Project Structure & Module Organization

This workspace currently contains no application code, tests, assets, or build configuration. Establish the layout when adding the first implementation, and update this guide to match. Prefer `src/` for application code, `tests/` for tests, `assets/` for static resources, and `docs/` for supporting documentation unless the chosen framework requires another layout. Group related functionality together and avoid creating empty directories speculatively.

## Build, Test, and Development Commands

No build, test, or local development commands are configured yet. When introducing a toolchain, document its prerequisites and exact commands in `README.md`, and expose routine tasks through the project's package manager or task runner. Include commands for installing dependencies, starting local development, building, testing, and linting. Do not document commands as supported until they work from a clean checkout.

## Coding Style & Naming Conventions

Follow the idiomatic style of the language and framework selected for the project. Add formatter and linter configuration alongside the first source files; use those tools to enforce indentation and formatting consistently. Use descriptive names, follow language conventions for identifiers, and keep filename casing consistent within each module. Prefer small, focused modules over unrelated functionality collected in generic utility files.

## Testing Guidelines

No testing framework or coverage threshold is established. Introduce tests with new behavior and select a framework appropriate to the implementation language. Use descriptive test names that identify the scenario and expected result. Add regression tests for bug fixes, cover meaningful failure cases, and keep tests deterministic. Document how to run individual tests and the full suite.

## Commit & Pull Request Guidelines

There is no Git history available here from which to infer commit conventions. Use short, imperative commit subjects, such as `Add configuration loader`, and keep commits focused. Pull requests should explain the problem, summarize the change, link relevant issues, and record validation performed. Include screenshots for visible UI changes. Clearly identify any checks that could not be run.

## Security & Configuration

Keep credentials and local secrets out of version control. Provide placeholder configuration examples when needed, and ignore generated output and machine-specific files when introducing the toolchain.

## Agent Configuration

Use `.codex/config.toml` for shared project overrides; it currently inherits existing settings. Store reusable workflows in `.agents/skills/<skill-name>/SKILL.md`, following `.agents/skills/README.md`. Keep general repository instructions in this file. Update configuration and workflow documentation when project tooling changes.
