---
id: w03-hx27-skill-installed-but-invisible
title: "An agent reported a skill installed when the session could not see it"
author: "Haoran Xu (hx27)"
---

I asked my agent to install the `explain-to-me` skill. It wrote
`~/.claude/skills/explain-to-me/SKILL.md` and reported success, but invoking the
skill immediately failed with `Unknown skill: explain-to-me`. The file and its
front matter were valid; the session had loaded its skill registry at startup
and had not rescanned. A fresh session ran the skill on the first try. Writing
the file and installing the skill are different events, and the agent reported
the first as evidence of the second. What should count as verification that an
agent's side effect actually took hold, rather than that it issued the command?
