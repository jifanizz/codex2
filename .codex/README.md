# Project Codex Configuration

`config.toml` holds shared, project-local Codex overrides. It currently inherits
existing settings without selecting a model or changing permissions.

Add documented TOML settings here when the project needs them. Project config
loads only for trusted projects and remains subject to managed requirements.
Keep personal settings in your user configuration and credentials outside this
repository. Do not set `CODEX_HOME` to this directory: it is configuration, not a
replacement for your user-level Codex home.

Repository instructions live in `../AGENTS.md`; reusable skills belong in
`../.agents/skills/`.

[Configuration reference](https://learn.chatgpt.com/docs/config-file/config-basic)
