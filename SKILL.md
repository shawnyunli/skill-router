---
name: skill-router
description: Choose the smallest relevant set of available Codex skills for the current task when several skills plausibly apply or the user asks which skill to use. Do not invoke for an obvious single-skill task or as a substitute for doing the task.
---

# Skill Router

Decide from the skills actually available in this session, using their descriptions and the user's requested outcome. Do not assume a skill is installed because it existed in another project or conversation.

1. Honor a skill explicitly named by the user. If unavailable, say so and continue with the best in-scope approach.
2. For implicit routing, match the deliverable and work required, not incidental keywords. Choose one skill when it covers the task; choose multiple only when distinct parts genuinely need them. If none fits, proceed without a skill.
3. Read the complete `SKILL.md` of each selected skill before taking task actions. Follow its relevant references and constraints. This router does not replace the selected skill's instructions.
4. Briefly tell the user which skill(s) you are using and why, then complete the underlying task. Do not stop after merely recommending a skill unless selection itself was the user's request.

Do not install, enable, publish, or grant permissions to another skill merely to improve a match. Ask only when the missing choice would materially change the result. Respect the user's scope and existing authorization boundaries.
