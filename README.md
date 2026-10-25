# Vibe Streamer

Shared guidance for coding on Twitch with Codex and Copilot on Pop!_OS.

- [Plan](PLAN.md): what to build next.
- [Shared skill](.agents/skills/stream-vibe-coding/SKILL.md): how we work. Keep words brief and simple.
- `projects/`: separate project repos, ignored by this repo.

## Add a project

1. Clone or create its repo inside `projects/`.
2. Run its Git commands from that folder. Save and push each project separately.
3. Keep its checklist in `PROGRESS.md` or its existing progress file.

Cloning this workspace does not restore the project repos. Clone them separately.

## Share the skill

Separate repos may not load the parent instructions. For each repo directly under `projects/`, add this to its `AGENTS.md` and `.github/copilot-instructions.md`. Keep existing instructions:

```markdown
For stream work, read `../../.agents/skills/stream-vibe-coding/SKILL.md`
relative to this project's root. Follow it with this project's instructions.
If unavailable, mention it and use the project's own guidance.
```

This path needs the same folder layout. If the AI misses it, ask it to read the shared skill.

**Start:** “Read the skill and checklist. Help with the next small task.”

**Finish:** “Review progress, record what we checked, and set the next task.”
