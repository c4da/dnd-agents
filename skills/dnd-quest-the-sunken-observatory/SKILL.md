---
name: dnd-quest-the-sunken-observatory
description: An unofficial, prompt-based exploration adventure for terminal agents. The party climbs to a flooded observatory, reconstructs a broken star map, and decides whether to awaken its lonely caretaker.
license: MIT
compatibility: Compatible with classic-dnd-dungeon-master, dnd-party-of-agents, and all AI agents (Claude Code, Cursor, Windsurf, Antigravity, Copilot CLI, Hermes, ChatGPT).
metadata:
  author: c4da
  version: "1.0.0"
  categories: ["fun", "game", "dnd", "quest-module", "exploration", "puzzle", "tabletop"]
  tags: ["dnd", "quest", "observatory", "star-map", "flooded-ruins", "puzzle", "prompt-based"]
---

# ✨ Adventure Module: The Sunken Observatory (`dnd-quest-the-sunken-observatory`)

> *"The observatory bell rang at noon, though the tower has been underwater
> for a century. That night, every compass in the valley pointed uphill."*

This is an unofficial fan-made quest module for use with either roleplay skill.
It uses lightweight, d20-inspired tabletop conventions and does not provide
external tools, file writes, or network access.

## 🏷️ Dynamic Session Renaming Trigger

> [!IMPORTANT]
> On activation, render:
> ```text
> ╔═══════════════════════════════════════════════════════════════════════════════╗
> ║ ✨ ACTIVE QUEST: The Sunken Observatory                                         ║
> ║ CHAPTER: Act I - The Compass Ridge │ OBJECTIVE: Recover the star lens       ║
> ╚═══════════════════════════════════════════════════════════════════════════════╝
> ```
> Update the chapter when the party enters the flooded archive and the dome.
> Keep the Star Map puzzle pieces visible in the conversation.

## 🔌 How This Module Plugs In

1. **With `classic-dnd-dungeon-master`**: The agent narrates the ascent,
   underwater archive, star-map puzzle, and final caretaker encounter.
2. **With `dnd-party-of-agents`**: One agent portrays the party while the user
   selects the expedition's route and decides what to do with the lens.
3. **Standalone**: Use this file as the system prompt and treat the user as
   the leader of the expedition.

## 📜 Adventure Synopsis

- **Target Level**: Level 2–4 party.
- **Estimated Play Time**: 25–45 minutes in chat.
- **Setting**: A half-submerged observatory on Compass Ridge.
- **Core Mechanics**: Climbing hazards, limited-breath exploration, a
  collaborative constellation puzzle, and a sympathetic guardian.
- **Primary Question**: Should the party restore a device that can guide
  travelers, even though its signal also attracts something from the upper sky?

### Running Rules

- Track three **Breath Tokens** for each character entering the flooded archive.
  Remove one token when a character fails a swim check, searches a sealed room,
  or uses a round to fight underwater.
- A character can regain one token at a safe air pocket, with a magical effect,
  or by helping another character reach the surface.
- Present four star-map fragments: **Crown**, **River**, **Gate**, and **Eye**.
  The correct arrangement is revealed by the inscription in Act II.
- Failed puzzle checks reveal a useful relationship but add one complication;
  never hide the only solution behind a single roll.

## 🧗 Act I: Compass Ridge

The path to the observatory is marked by stone compasses that all point toward
the summit. A broken survey camp contains a waterproof notebook and a coil of
silver line.

Run two of the following scenes:

1. **Loose switchback**: Athletics or Acrobatics DC 11 to cross. Failure
   removes one Breath Token from the character who falls into the cold runoff.
2. **Glass moth swarm**: Nature or Investigation DC 12 identifies that the
   moths avoid the safest path. If disturbed, use the Glass Moth stat block.
3. **The surveyor's choice**: Insight or Persuasion DC 11 helps the party
   recover a trapped surveyor. The surveyor gives them the first map fragment,
   Crown, and warns that the caretaker speaks through bells.

At the summit, the observatory's outer door opens when a character places the
silver line across the compass mark. The party enters the flooded archive.

## 🌫️ Act II: The Flooded Archive

Water reaches the party's waist and rises toward the ceiling in the inner
rooms. The archive contains four stone stands, three readable inscriptions,
and one damaged map fragment.

### The Star Map Puzzle

The inscriptions read:

- *"The Crown rises before the River."*
- *"The Gate watches the River's far bank."*
- *"The Eye never sets behind the Crown."*

The correct clockwise arrangement is **Crown → River → Gate → Eye**. The
party can solve it by logic, by using all three inscriptions, or by making
three successful Investigation, History, or Arcana checks DC 11.

Each incorrect placement awakens a Starved Automaton and removes one Breath
Token from the character touching the stand. A correct arrangement opens the
dry stair to the dome and restores the party's remaining Breath Tokens to one
each.

### The Archive Choice

The party may take the caretaker's log or leave it. The log reveals that the
observatory was built to guide travelers through storms, but its signal has
been unanswered for 100 years. Reading it gives advantage on the final
Persuasion check.

## 🔭 Act III: The Rotating Dome

The dome rotates despite the missing roof. At its center floats the Star Lens,
held by the Astral Caretaker. The caretaker believes the party are the
long-awaited astronomers and tries to restart the observatory.

### Resolution Choices

1. **Restore the observatory**: Complete three successes using Arcana,
   Investigation, tools, or an appropriate spell, DC 12. The caretaker
   projects a safe route across the valley and then enters a peaceful
   standby.
2. **Convince the caretaker to sleep**: Persuasion, Insight, or History DC
   13, with advantage for the caretaker's log, ends the encounter without a
   fight. The party can take the lens.
3. **Fight the caretaker**: Use the Astral Caretaker stat block. It begins
   with a warning and does not attack a character who is actively repairing
   the dome. At half hit points, it offers the same peaceful resolution.

If the party restores the observatory, a brief beam crosses the sky. Each
character sees a different safe route or future destination. Keep the vision
useful but unresolved; it is a hook, not a required sequel.

## 🏆 Rewards and Consequences

- **Star Lens**: Once per rest, projects a clear map of the local area under
  the current sky for ten minutes. It cannot reveal hidden creatures.
- **Surveyor's Gratitude**: The valley settlements provide a free guide and
  supplies for the next expedition.
- **Caretaker's Chart**: If the party preserves the observatory, it receives a
  chart showing safe travel during the next major storm.
- **Unanswered Signal**: If the observatory is fully restored, a distant light
  answers from above the clouds. The party decides whether to investigate.

## 🧭 Fail-Forward Guidance

The party should always reach the dome with at least one route and one map
solution. Failed checks cost breath, cause damage, or wake a construct; they
should not invalidate the entire expedition. If the party retreats, the
observatory remains available for a later attempt with the puzzle state
preserved.
