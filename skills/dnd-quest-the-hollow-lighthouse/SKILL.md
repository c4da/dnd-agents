---
name: dnd-quest-the-hollow-lighthouse
description: An unofficial, prompt-based coastal mystery adventure for terminal agents. The party investigates a silent lighthouse, navigates rising water, and chooses whether to redeem or defeat its bound keeper.
license: MIT
compatibility: Compatible with classic-dnd-dungeon-master, dnd-party-of-agents, and all AI agents (Claude Code, Cursor, Windsurf, Antigravity, Copilot CLI, Hermes, ChatGPT).
metadata:
  author: c4da
  version: "1.0.0"
  categories: ["fun", "game", "dnd", "quest-module", "mystery", "coastal", "tabletop"]
  tags: ["dnd", "quest", "mystery", "lighthouse", "coastal", "exploration", "prompt-based"]
---

# 🌊 Adventure Module: The Hollow Lighthouse (`dnd-quest-the-hollow-lighthouse`)

> *"The lighthouse has been dark for nine nights. Every evening, three pale
> flashes answer from the sea, and every morning another fishing boat is found
> drifting empty."*

This is an unofficial fan-made quest module for use with either roleplay skill.
It uses lightweight, d20-inspired tabletop conventions and does not provide
external tools, file writes, or network access.

## 🏷️ Dynamic Session Renaming Trigger

> [!IMPORTANT]
> On activation, render:
> ```text
> ╔═══════════════════════════════════════════════════════════════════════════════╗
> ║ ⚓ ACTIVE QUEST: The Hollow Lighthouse                                         ║
> ║ CHAPTER: Act I - The Silent Beacon │ OBJECTIVE: Find the missing crews       ║
> ╚═══════════════════════════════════════════════════════════════════════════════╝
> ```
> Update the chapter when the party reaches the flooded tunnels or lantern
> chamber. Do not skip the party's opportunity to investigate or negotiate.

## 🔌 How This Module Plugs In

1. **With `classic-dnd-dungeon-master`**: The agent runs the investigation,
   presents clues, and manages the lighthouse hazards.
2. **With `dnd-party-of-agents`**: One agent portrays the four companions while
   the user chooses the party's route and makes final decisions.
3. **Standalone**: Use this file as the system prompt and treat the user as
   the adventuring party's leader.

## 📜 Adventure Synopsis

- **Target Level**: Level 1–3 party.
- **Estimated Play Time**: 20–40 minutes in chat.
- **Setting**: The storm-battered village of Greyhook and its abandoned
  lighthouse on a sea stack.
- **Core Mechanics**: Investigation, social deduction, a rising-tide clock,
  spatial navigation, and a nonviolent boss resolution.
- **Primary Question**: Is the lighthouse keeper murdering sailors, or is the
  beacon warning them away from something worse?

### Running Rules

- Ask for a check only when the result changes the situation. Use DC 10 for
  routine clues, DC 12 for risky actions, and DC 14 for hidden or time-critical
  details.
- A failed check gives a partial clue and advances the tide clock; it never
  erases the central mystery.
- Keep a visible four-segment **Tide Clock**. Mark one segment for a failed
  navigation check, a loud fight in the tunnels, or a deliberate delay.
- At four segments, the lower tunnels flood. The party can still finish the
  quest, but movement becomes harder and the final confrontation gains one
  environmental hazard.

## 🗺️ Act I: Three Flashes at Greyhook

The party arrives while the village council argues over whether to burn the
lighthouse. The last surviving deckhand remembers seeing a lantern shutter
open from inside the sealed tower, followed by three flashes toward the
western reef.

Give the party three leads:

1. **The empty boat**: Investigation DC 11 finds salt crystals inside the
   cabin, but no blood or signs of a struggle.
2. **The keeper's ledger**: Persuasion or Insight DC 12 convinces the harbormaster
   to show it. The final entry reads, *"The light is not calling them. It is
   keeping the deep gate asleep."*
3. **The cliff path**: Survival DC 10 finds fresh boot prints and a broken
   brass lens fragment. A failure costs one Tide Clock segment.

If the party talks to the villagers, they learn that Keeper Maelin vanished
three months ago after refusing to extinguish the beacon during a storm. The
party may approach by the cliff path or row directly to the sea-stack. Both
routes reach Act II.

## 🕳️ Act II: The Flooded Service Tunnels

The lighthouse door is locked from the inside. A maintenance hatch beneath the
cliff opens into tunnels that fill and drain with the sea.

### Navigation Challenge

Run three checks before the party reaches the lantern stairs:

- **Investigation DC 12**: Identify the dry route by following old drainage
  arrows.
- **Athletics or Acrobatics DC 11**: Cross a collapsed walkway.
- **Arcana or Nature DC 12**: Recognize the pale algae that marks a safe air
  pocket.

The party needs two successes. Each failure marks the Tide Clock and creates
one encounter with a Brine Mote from the reference file. Creative solutions
can grant an automatic success.

### The Three Valve Puzzle

At a junction, three corroded valves are marked **Bell**, **Wave**, and
**Moon**. A brass plate reads:

> *"Ring before the wave, wait beneath the moon, and never wake the bell twice."*

The safe sequence is **Bell → Wave → Moon**. Turning a valve twice releases a
burst of pressurized water: Dexterity save DC 12 or `1d6` bludgeoning damage
and one Tide Clock segment. The correct sequence drains the final stairwell
and reveals a hidden compartment containing Maelin's journal.

## 🔦 Act III: The Lantern Chamber

The lantern burns with cold blue fire. Keeper Maelin stands inside the
mechanism, bound to the lens by strands of seawater and glass. The keeper is
the Hollow Lighthouse Warden described in the reference file.

The party learns that Maelin bound themself to the beacon to hold shut a
nearby sea cave. The missing crews were not killed; they were pulled into the
cave after following false lights emitted by a damaged lens. The binding is
now failing.

### Resolution Choices

1. **Repair the beacon**: Three successful checks (Arcana, Religion, or
   appropriate tool use, DC 12) free Maelin and restore the warning light.
   Each failure marks the Tide Clock.
2. **Break the lens**: The party can destroy the lens after defeating or
   persuading Maelin. This ends the immediate threat but leaves the sea cave
   sealed only temporarily.
3. **Fight the Warden**: If the party attacks or ignores the warnings, use the
   Warden stat block. At half hit points, Maelin asks for help and the party
   can switch to the repair resolution.

If the Tide Clock reached four, every round in the chamber begins with a
surging wave. Each creature chooses a Strength save DC 11 or moves 10 feet
toward the stairwell.

## 🏆 Rewards and Consequences

- **Tideglass Lens**: Once per rest, reveals hidden writing or invisible
  markings within 30 feet for one minute.
- **Greyhook's Trust**: The village provides shelter, food, and a safe boat.
- **Keeper's Favor**: If Maelin is freed, the lighthouse becomes a reliable
  navigation point and the party receives a sealed chart to a future coastal
  adventure.
- **Hard Choice**: If the lens is broken, the village is safe for now but the
  final journal page warns that something beneath the reef has begun to wake.

## 🧭 Fail-Forward Guidance

The party should always learn that the beacon is a warning, not a lure. Failed
checks increase danger, reduce available time, or cause damage; they do not
remove the central clue. If the party retreats, Greyhook can provide a short
rest and the Tide Clock keeps its current value.
