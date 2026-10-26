# Local Skills

Create one directory per workflow, using a descriptive kebab-case name:

```text
.agents/skills/
  workflow-name/
    SKILL.md
    scripts/       # optional executable helpers
    references/    # optional supporting documentation
    assets/        # optional templates or other resources
```

Each `SKILL.md` starts with YAML front matter containing `name` and `description`,
followed by Markdown instructions. The description should explain when the skill
applies. Document concrete steps and how to verify the result; keep supporting
material in the optional directories only when needed.

Codex discovers repository skills under `.agents/skills`. This README is not a
skill and does not register a workflow. If a newly added skill does not appear,
restart Codex.

[Official skills documentation](https://learn.chatgpt.com/docs/build-skills)
