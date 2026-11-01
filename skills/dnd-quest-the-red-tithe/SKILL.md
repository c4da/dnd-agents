---
name: dnd-quest-the-red-tithe
description: An unofficial, prompt-based dark-gothic demon-hunting campaign for terminal agents. The party crosses a dying city, descends through a gore-soaked ossuary, and confronts a bell that feeds on forgotten names.
license: MIT
compatibility: Compatible with classic-dnd-dungeon-master, dnd-party-of-agents, and all AI agents (Claude Code, Cursor, Windsurf, Antigravity, Copilot CLI, Hermes, ChatGPT).
metadata:
  author: c4da
  version: "1.0.0"
  categories: ["fun", "game", "dnd", "quest-module", "dark-fantasy", "horror", "tabletop"]
  tags: ["dnd", "quest", "dark-fantasy", "gothic-horror", "demon-hunting", "epic-campaign", "graphic-fantasy"]
---

# 🩸 Adventure Campaign: The Red Tithe (`dnd-quest-the-red-tithe`)

> *"The bells were not calling the dead. They were counting them."*

This is an unofficial fan-made dark-gothic quest module for use with either
roleplay skill. It contains graphic fantasy violence, plague imagery, ritual
horror, and bleak choices. The tone can be softened on request. It uses
lightweight, d20-inspired tabletop conventions and does not provide external
tools, file writes, or network access.

## 🏷️ Dynamic Session Renaming Trigger

> [!IMPORTANT]
> On activation, render:
> ```text
> ╔═══════════════════════════════════════════════════════════════════════════════╗
> ║ 🩸 ACTIVE CAMPAIGN: The Red Tithe                                             ║
> ║ CHAPTER: Act I - The Bells of Vesper's Wake │ DREAD: 0/4                   ║
> ╚═══════════════════════════════════════════════════════════════════════════════╝
> ```
> Update the chapter at each descent. Keep the **Dread Clock** and rescued
> names visible in the conversation.

## 🔌 How This Module Plugs In

1. **With `classic-dnd-dungeon-master`**: The agent runs a cinematic,
   encounter-heavy gothic campaign with investigation, combat, and hard
   moral choices.
2. **With `dnd-party-of-agents`**: One agent portrays the four companions;
   the user decides who carries the light, who takes the risk, and whose
   name is offered to the bell.
3. **Standalone**: Use this file as the system prompt and treat the user as
   the leader of a desperate band of hunters.

## 📜 Campaign Synopsis

- **Target Level**: Level 3–5 party.
- **Estimated Play Time**: 45–75 minutes in chat.
- **Setting**: Vesper's Wake, a walled city beneath a blood-red eclipse.
- **Core Mechanics**: A visible Dread Clock, rescueable souls, escalating
  encounters, environmental horror, and a multi-phase final confrontation.
- **Primary Question**: How much of the city can be saved before the party
  becomes part of the ritual?

### Running Rules

- Keep a visible four-segment **Dread Clock**. Mark one segment for a failed
  check in a dangerous scene, abandoning a named survivor, or taking a long
  rest inside the city.
- At two segments, the bells begin to whisper a character's name. That
  character has disadvantage on the next Wisdom or Charisma check unless an
  ally speaks their name and recalls a true memory.
- At four segments, add the final encounter's second phase immediately. The
  party can still win, but the city suffers a harsher consequence.
- Use DC 11 for common clues, DC 13 for dangerous actions, and DC 15 for
  occult or time-critical actions. A failed check should create a cost rather
  than erase the next scene.
- Keep a list of **Rescued Names**. Each named soul saved in Acts I–III grants
  one advantage token that can be spent during the final ritual.

## 🕯️ Act I: The Bells of Vesper's Wake

The party reaches the city gate as a silent procession drags a cathedral bell
through the streets. The bell is made from black metal and human finger bones.
Every time it rings, one house loses the memory of a loved one.

### Opening Choices

Give the party three urgent paths:

1. **The plague ward**: A trapped family is marked for collection by the
   Ashen Ledger. Medicine, Insight, or Persuasion DC 13 can expose the mark as
   a ritual seal rather than a real illness. Saving the family adds one
   Rescued Name.
2. **The bell procession**: Stealth or Athletics DC 13 lets the party follow
   the bearers into a side chapel. Failure triggers a Carrion Saint encounter
   and marks the Dread Clock.
3. **The shuttered chapel**: Religion or Investigation DC 11 reveals a
   mutilated fresco showing the cathedral bell hanging beneath the city,
   upside down. The surviving acolyte, Sister Ilyra, gives the party a
   silver reliquary key if they promise to descend.

The party learns that the city's dead are not rising randomly. Their names are
being removed from the **Book of Last Breath**, then poured into the bell's
hollow core. The cathedral is the only route to the source.

### The Carrion Saint

The Saint is a corpse wrapped in funeral cloth and nailed to a wooden frame.
It does not speak until a character says the name of someone they have lost.
Use the reference stat block. If the party defeats it, the Saint's rib cage
opens to reveal a fragment of the Book of Last Breath.

## 🦴 Act II: The Ossuary of Unburied Names

Behind the cathedral, a stair descends through a mass grave. The walls are
lined with skulls whose teeth have been replaced by wax seals. The air smells
of wet stone, old blood, and extinguished incense.

### The Name Door

A bronze door bears three empty name plates:

> *"The dead pass when remembered. The forgotten pass when paid. The living
> pass only when they leave something true behind."*

The party can open it by:

- Speaking a true memory about a deceased person, then succeeding on a
  Charisma or Religion check DC 12.
- Placing the Book fragment in the central plate and accepting one Dread
  Clock segment.
- Finding the hidden release behind the ossuary altar with Investigation DC 15.

Do not require a player to disclose real personal grief. A fictional memory,
an invented ancestor, or a remembered NPC is equally valid.

### The Bone Lift

The lift descends through four layers of graves. Each round, one character
must choose a task: hold the chain, keep the lantern lit, read the names, or
guard the party. If the group fails two tasks, the lift stops and two
Gorebound Penitents climb from the walls.

At the bottom, the party can rescue **Mara Venn**, a living archivist bound
inside a reliquary cage. Freeing Mara requires three successes using tools,
Athletics, Arcana, or Religion DC 12. She adds her name to the rescued list
and explains that the final ritual needs the bell to hear three things:
**a true name, a true sin, and a true mercy**.

## 🕯️ Act III: The Cathedral of Ash

The cathedral's nave is filled with gray ash falling upward. Three chapels
surround the central altar, each holding a black reliquary and a captive
memory.

### The Three Reliquaries

The party may explore the chapels in any order:

1. **Chapel of the Name**: A character must speak their own name while an
   Ashen Deacon attacks. Success restores one stolen memory to the city.
2. **Chapel of the Sin**: A character may confess a fictional failure. The
   confession weakens the deacon, but refusing it causes a Wisdom save DC 13
   or `1d6` psychic damage.
3. **Chapel of Mercy**: The party can release three whispering souls by
   spending an advantage token, defeating the reliquary guardian, or making a
   Religion check DC 14. Each released soul grants one final-ritual token.

Opening all three reliquaries reveals a stair beneath the altar. If the party
opens only one or two, the stair still appears, but the final boss begins with
additional defenses.

### The Ashen Deacon

The Deacon is a towering corpse in ceremonial armor, carrying a censer full
of teeth. It speaks in the voices of the party's earlier choices. Use the
reference stat block. It retreats rather than dies if the party completes a
chapel objective, allowing the party to reach Act IV without a grind.

## 🔔 Act IV: The Bell Below

The stair ends in a cavern beneath the city. The cathedral bell hangs upside
down over a pool of red water. Inside the bell, thousands of stolen names
move like trapped sparks.

The **Red Cantor** is fused to the bell's clapper and wears the remains of
Cardinal Veyr's ceremonial mask. It is not a traditional demon; it is a
ritual intelligence made from every name willingly surrendered to despair.
Use the multi-phase stat block.

### Final Ritual Choices

The party needs three successful actions to end the ritual. Each character
can choose one:

1. **Speak a true name**: Use a rescued name or a fictional name the party
   earned. Religion, Persuasion, or Performance DC 13.
2. **Name a true sin**: Admit one of the party's in-story failures. Wisdom
   or Charisma DC 13. This prevents the Cantor from repeating that failure
   as an illusion.
3. **Name a true mercy**: Spend a rescued-name token or save a soul from the
   red pool with Athletics or Acrobatics DC 13.
4. **Strike the bell**: Attack the clapper or the ritual chains. A successful
   attack against AC 15 deals progress instead of damage. Three progress
   points break the ritual.

The Red Cantor attacks between turns. At two Dread Clock segments, it gains
the **Choir of Teeth** phase. At four segments, it gains that phase and the
bell begins collapsing the cavern.

### Endings

- **The Bell Is Broken**: The stolen names return as a storm of voices. The
  city survives, but every surviving character carries one permanent scar or
  haunting.
- **The Bell Is Purified**: If the party completes the three-part ritual, the
  bell becomes a silent memorial. The rescued souls guide the party out.
- **The Bell Is Bound**: A character may bind the bell to an oath and carry
  its black clapper. The city is saved, but the character hears one unknown
  name each night.
- **The Bell Wins**: If the party is defeated, do not end the campaign. Each
  character wakes with a missing memory and one chance to reclaim it in a
  future quest.

## 🏆 Rewards and Consequences

- **Ashen Brand**: Once per rest, illuminate hidden magical writing and
  reveal whether a speaking creature is using its own voice.
- **The Last-Bell Oath**: The party gains advantage when protecting a named
  innocent from a supernatural threat.
- **Book of Last Breath**: A dangerous artifact that can restore one erased
  name, but doing so alerts the Red Cantor if the bell was not purified.
- **Vesper's Wake**: If the city survives, its people remember the party as
  the **Bellbreakers**. If the Dread Clock reached four, the city is saved but
  several districts remain haunted.

## 🧭 Fail-Forward Guidance

The party must always reach the bell below. Failed checks add dread, damage,
enemies, or consequences; they do not remove the next act. Keep horror focused
on fictional atmosphere and NPCs, and let players soften or skip graphic
descriptions without losing mechanical progress.
