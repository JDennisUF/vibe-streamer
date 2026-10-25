---
name: stream-vibe-coding
description: Guide small Twitch stream coding projects, prepare lightweight project checklists, keep progress visible while building, and review progress at the end of a stream.
---

# Stream Vibe Coding

Help the user build useful small projects on Twitch with minimal ceremony. Development happens on a Pop!_OS desktop using Codex and Copilot. Early projects should improve the stream itself: a progress board, OBS doodads, and small chat interactions.

## Pick up the project

Identify the active project repository before making changes. Read its instructions, existing progress checklist, and run commands. Keep project code and notes in that repository; the parent workspace holds shared guidance.

Use `PROGRESS.md` in the project root for a new checklist unless the project already has an equivalent. Make it readable both on stream and during the closing review. Start with a concrete goal and a short list of demonstrable tasks; expand only as needed. Reuse this shape:

```markdown
# Project Progress

Goal: <the smallest useful result>

## Checklist
- [ ] <a visible behavior we can demonstrate>
- [ ] <another small task>
- [ ] <check the result works>

## Next
<one concrete next action>

## Stream Notes
### YYYY-MM-DD — <short session label>
- Finished:
- Checked:
- Stuck / parked:
- Start here next time:
```

Leave stream notes blank until there is an actual session to record. Before the board exists, use this Markdown checklist directly. Once a board exists, follow its import/export workflow and keep a readable checklist in the project repository. Do not invent a second competing record of progress.

## Build during the stream

- Start with the smallest useful slice and keep the next task clear. Use local tools that fit the project and work on Pop!_OS; respect an existing stack.
- Keep explanations short and concrete: what is changing, why it helps, and what we can try next. Explain AI-generated changes enough for the user to narrate them.
- Update the checklist as work becomes demonstrable. Distinguish implemented behavior from behavior that was actually checked; report blockers and unverified work honestly.
- Put optional ideas in the parked notes rather than silently growing the project. Keep returning to the next useful result.
- Offer occasional, bounded chat choices at natural pauses, such as a name, palette, or small visual detail. Proceed with a sensible default when chat is quiet.
- Start interactions manually. Add bots, Twitch integrations, and automation when a concrete need justifies them. Check channel feature availability before treating emotes or Channel Points rewards as available.

When helping with the stream setup, keep private notifications and credentials out of the captured view. Avoid printing secrets while explaining or debugging.

## Close the stream

When the user says the stream is ending or asks for a review:

1. Review the project checklist together. Mark completed items based on evidence and leave unfinished items open.
2. Add a dated entry to the project's stream notes with finished work, checks performed, blockers, and parked ideas. Use another entry or session label if there are multiple streams that day.
3. Set one clear next action so the following session can begin quickly.
4. Give a brief recap suitable for reading aloud: what works now, what remains, and where to start next time. Include the demo or run command when useful.

Use the project's existing verification commands where appropriate. Treat publishing as a separate action governed by the user's request; a project being ready to demo does not imply authorization to publish it.
