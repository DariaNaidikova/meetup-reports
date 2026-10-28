# Boring Task, Hard Lessons: Building an AI Agent That Works

The talk is a case study of building an AI agent that migrates legacy HTML email templates to React + MJML. The task is niche, but the design traps apply to any agent.

## What the report covers

- **The task:** why email templates hurt, and why React + MJML is the fix.
- **Mistake 1, weak context:** a few examples covered about 20% of real cases and the agent hallucinated on the rest. Purpose-built reference docs (validation rules, variable binding, component docs) fixed it.
- **Mistake 2, one agent for everything:** variable extraction, component mapping, dependency check and validation in one agent became an unmaintainable monolith. Splitting it into independently testable skills with a thin orchestrator fixed it.
- **Skill vs. agent:** if you write "how-to" steps inside the orchestrator, that logic should be its own skill.
- **Sharing it:** shipping the result as a plugin through a team plugin marketplace.
- **What I'd do differently:** plan first, write the spec, decide the skill breakdown upfront (spec-driven development).

## Files

- [`index.html`](index.html): slide viewer. Open it in a browser. Navigate with the arrow keys, Space, Home/End, swipe or the progress bar. Press `F` for fullscreen.

## Useful links

- [GitHub Spec Kit](https://github.com/github/spec-kit#spec-driven-development)
- [mattpocock skills](https://github.com/mattpocock/skills/tree/main/skills/engineering) (`grilling`, `to-spec`, `to-tickets`)
- [awesome-claude-code-subagents](https://github.com/VoltAgent/awesome-claude-code-subagents/tree/main/categories)
