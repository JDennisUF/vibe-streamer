# Vibe Streamer

A lightweight home for shared stream guidance and independent project repos. See [PLAN.md](PLAN.md) for the starter projects.

```text
vibe-streamer/
  .agents/skills/stream-vibe-coding/SKILL.md
  AGENTS.md
  PLAN.md
  projects/
    stream-board/       # independent Git repo, ignored here
    stream-overlay/     # independent Git repo, ignored here
```

## Project repos

Clone or initialize each project under `projects/`. The parent `.gitignore` already ignores everything there except the directory placeholder, so there is no per-project ignore list to maintain.

Run Git commands from the repo you intend to change. Each project owns its source, dependencies, checklist, commits, and remote. The parent repo stores shared guidance. Cloning this parent later does not restore the ignored projects; clone each project's remote separately. This layout does not use Git submodules.

## Shared guidance for Codex and Copilot

The shared workflow lives in [.agents/skills/stream-vibe-coding/SKILL.md](.agents/skills/stream-vibe-coding/SKILL.md). It covers small tasks, visible progress, minimal chat interaction, and end-of-stream checklist reviews.

The root agent instructions point to it for work in this workspace. Independent nested Git repositories can have their own discovery boundaries, so do not rely on them automatically inheriting parent instructions. See the official [Codex skill discovery](https://learn.chatgpt.com/docs/build-skills) and [AGENTS.md discovery](https://learn.chatgpt.com/docs/agent-configuration/agents-md) guidance.

When setting up a project directly under `projects/`, add this small pointer to its `AGENTS.md` and `.github/copilot-instructions.md`, preserving any existing instructions:

```markdown
For Twitch stream planning, coding, and closing reviews, read
`../../.agents/skills/stream-vibe-coding/SKILL.md`, resolved from this
project's repository root. Follow that shared workflow alongside this
project's own instructions. If the shared file is unavailable, report
that and continue using the project's own guidance.
```

Those pointers keep one maintained workflow instead of copies of it. They depend on this local directory layout; a standalone clone remains usable with its own project guidance. If an assistant does not load the pointer, explicitly ask it to read the shared file at the start of the session. Copilot behavior depends on the client and enabled instruction support.

Example opening prompt:

> Read the shared stream-vibe-coding skill and this project's progress checklist. Help me work on the next small task for today's stream.

Example closing prompt:

> We're ending the stream. Review the project checklist with me, record what we finished and checked, and set the next starting task.

Each project keeps its own `PROGRESS.md` or existing equivalent. The future progress board can display and exchange that information; until then, the Markdown checklist is enough.
