---
name: dnd-quest-the-ember-vault
description: An unofficial, prompt-based underground forge adventure for terminal agents. The party rescues trapped workers, manages a rising heat clock, and decides whether to seal or relight a dangerous ember engine.
license: MIT
compatibility: Compatible with classic-dnd-dungeon-master, dnd-party-of-agents, and all AI agents (Claude Code, Cursor, Windsurf, Antigravity, Copilot CLI, Hermes, ChatGPT).
metadata:
  author: c4da
  version: "1.0.0"
  categories: ["fun", "game", "dnd", "quest-module", "dungeon", "crafting", "tabletop"]
  tags: ["dnd", "quest", "forge", "fire", "rescue", "dungeon-crawl", "prompt-based"]
---

# 🔥 Adventure Module: The Ember Vault (`dnd-quest-the-ember-vault`)

> *"The old quarry has started glowing at night. Three stonewrights went below
> to inspect it, and now the mountain exhales smoke through every crack."*

This is an unofficial fan-made quest module for use with either roleplay skill.
It uses lightweight, d20-inspired tabletop conventions and does not provide
external tools, file writes, or network access.

## 🏷️ Dynamic Session Renaming Trigger

> [!IMPORTANT]
> On activation, render:
> ```text
> ╔═══════════════════════════════════════════════════════════════════════════════╗
> ║ 🔥 ACTIVE QUEST: The Ember Vault                                               ║
> ║ CHAPTER: Act I - The Collapsed Quarry │ OBJECTIVE: Rescue the stonewrights  ║
> ╚═══════════════════════════════════════════════════════════════════════════════╝
> ```
> Update the chapter when the party reaches the cooling galleries and the
> ember chamber. Keep the Heat Clock visible to the user.

## 🔌 How This Module Plugs In

1. **With `classic-dnd-dungeon-master`**: The agent runs the rescue, hazard,
   puzzle, and final choice while tracking heat and structural damage.
2. **With `dnd-party-of-agents`**: One agent portrays the four companions; the
   user decides who carries tools, takes risks, or negotiates with the vault.
3. **Standalone**: Use this file as the system prompt and treat the user as
   the expedition leader.

## 📜 Adventure Synopsis

- **Target Level**: Level 2–4 party.
- **Estimated Play Time**: 20–40 minutes in chat.
- **Setting**: A sealed stonewright quarry beneath the Redglass Ridge.
- **Core Mechanics**: Environmental hazard tracking, rescue priorities,
  pressure valves, improvised crafting, and a guardian that can be reasoned
  with.
- **Primary Question**: Is the ember engine a catastrophe, or the only thing
  preventing the mountain from collapsing?

### Running Rules

- Use a visible four-segment **Heat Clock**. Mark one segment when the party
  fails a hazard check, spends a long time searching, or uses a loud fire or
  explosive effect.
- At two segments, metal surfaces become dangerous: a creature that ends its
  turn touching exposed metal makes a Constitution save DC 10 or takes `1d4`
  fire damage.
- At four segments, the vault begins to collapse. The party has three rounds
  to reach the exit or stabilize the engine.
- Failed checks reveal partial information and increase heat; they do not
  strand the party or remove a rescue route.

## ⛏️ Act I: The Collapsed Quarry

The party finds a cracked lift platform, three abandoned helmets, and a
survivor calling from below. A pressure wave from the quarry sends ash through
the entrance every few minutes.

Offer three approaches:

1. **Repair the lift**: Investigation or tools check DC 11, then Athletics DC
   10 to operate it safely. Failure marks the Heat Clock and drops loose
   debris, dealing `1d4` bludgeoning damage to one random creature.
2. **Climb the ventilation shaft**: Athletics or Acrobatics DC 12. Success
   reaches the lower gallery quickly; failure leaves the party separated until
   the next scene.
3. **Clear the rubble**: Three group Strength checks DC 10. Each success frees
   a trapped worker; the third opens a stable route.

The first rescued worker explains that the engine below is awake but not
hostile. The second worker, if found, carries a brass cooling key. The third
worker is trapped behind a heat seam and can be reached in Act II.

## 🌡️ Act II: The Cooling Galleries

The galleries contain four coolant channels, but only two still flow. The party
must choose which channels to restore before the engine overheats.

### The Valve Route

Three marked wheels control the system:

- **Stone** opens the main channel.
- **Rain** redirects water from the upper cistern.
- **Ash** vents pressure into an empty shaft.

The brass key shows the sequence **Stone → Rain → Ash**. A character can infer
this with Investigation or Engineering-style tool use DC 12. The wrong sequence
marks the Heat Clock and releases a Cinderling encounter.

Once the correct route is open, the party can rescue the third worker. Let
each player choose one contribution: carry the worker, hold a valve, protect
the group, or search for supplies. A successful contribution grants advantage
on the next group's exit check.

### Optional Crafting Choice

The party can spend one minute and one ordinary weapon or tool to make a
**heat-hook**. It grants advantage on one check involving a hot mechanism but
is destroyed after use.

## ⚒️ Act III: The Ember Engine

The final chamber holds a suspended core of red stone, surrounded by rotating
iron rings. The Ash-Iron Sentinel from the reference file guards it. The
sentinel follows a simple instruction: *preserve the engine and prevent the
mountain from breaking*.

### Resolution Choices

1. **Stabilize the engine**: Complete three successes using Arcana, tools,
   Athletics, or a relevant spell, DC 12. Each failure marks the Heat Clock.
   The sentinel becomes an ally if the party explains that the workers are
   alive.
2. **Seal the vault**: Remove the ember core with a group Strength or
   Constitution check DC 13. This ends the immediate danger but destroys the
   old forge and leaves the quarry unusable.
3. **Fight the sentinel**: Use its stat block if the party attacks or refuses
   to leave. At half hit points, it pauses and repeats its instruction,
   allowing a social resolution.

If the Heat Clock reaches four, begin a three-round collapse countdown. Each
round, the party must choose between moving toward the exit or spending an
action to prevent falling debris. A rescued worker can help with one
stabilization action.

## 🏆 Rewards and Consequences

- **Ember Key**: Once per rest, warms or cools one handheld object for ten
  minutes and gives advantage on one crafting or survival check.
- **Stonewright Contract**: If the workers survive, the quarry community
  repairs one mundane item for free and offers a safe workshop.
- **Engine's Blessing**: If the engine is stabilized, each character receives
  a faint ember mark. Once before the next long rest, the mark grants
  resistance to one instance of fire damage.
- **Sealed Vault**: If the engine is removed, the party gains a valuable
  fist-sized ember crystal but loses access to the forge.

## 🧭 Fail-Forward Guidance

The party must always be able to reach the engine and the exit. Failures add
heat, damage, or time pressure. If all workers cannot be rescued, let the
survivors describe a future rescue lead rather than ending the story.
