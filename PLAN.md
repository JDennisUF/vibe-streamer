# PLAN.md: Start Streaming, Build the Tools We Need

## Summary

Start with a few small projects that make streaming easier. Keep the setup light: a short show checklist, project checklists we review at the end of each stream, and a visible board showing what we’re doing and what’s next.

Develop on Pop!_OS with Codex and Copilot. Keep the tools simple to run locally and easy to change during a stream.

## Starter Projects

1. **Stream Progress Board** — Build a small local web app that shows the current project, its checklist, completed items, and the next task. Save progress in the browser and support exporting and importing checklist files in the repo, so it’s convenient to use live and straightforward to review with Codex or Copilot after a stream.
2. **Stream Overlay Doodads** — Add a simple OBS browser-source page for the project name, current task, and a short break or “back soon” message. Reuse the board’s project information where practical.
3. **Chat Interaction Kit** — Collect a handful of emote ideas, chat commands, and optional Channel Point rewards. Start with simple text interactions and rewards that are available on the channel; try editor theme-color picks as a manually handled reward.

Keep the first board focused on showing progress. Add features only when a real stream reveals a need.

## Stream Routine

- **Before:** Pick a small task, open the board, and check audio, screen readability, and OBS scenes.
- **During:** Work through the checklist. Pause at a few natural points to read chat or ask for a bounded choice.
- **After:** Review what shipped, mark checklist progress, note what got stuck, and choose the next task.

Every project checklist should make the goal and next task obvious. End each stream by reviewing it together, recording the outcome, and setting a clear starting point for next time.

## First Milestones

- Build and use the progress board on a real stream.
- Add the OBS overlay when the board helps establish a useful stream status.
- Add chat commands and rewards as the channel and stream routine are ready.
- Keep setup and operation comfortable on Pop!_OS; avoid requiring accounts, hosted services, or custom Twitch integrations to get started.

## Assumptions and Checks

Assume a small local web app is the right first project. It saves progress in the browser and exchanges checklist files with the repo. Before relying on it, test a refresh, export and import, and recovery from an incomplete session. Check Twitch’s current channel feature availability before listing rewards as ready to redeem.
