# Skill Router

A lightweight Codex skill for choosing the smallest relevant set of available skills when a task could match more than one. It honors skills named by the user, reads the selected skill instructions, and then completes the actual task.

## Install

```bash
npx skills add https://github.com/shawnyunli/skill-router --skill skill-router
```

For personal use across repositories, add `-g` to the command. The repository also contains `agents/openai.yaml` for the Codex display name and description.

## Scope

Skill Router is intended for ambiguous or overlapping skill matches. It does not force itself into every request, install other skills, or grant permissions. Obvious single-skill tasks should go straight to that skill.
