---
name: dnd-quest-the-wolf-host
description: An unofficial, prompt-based sequel to The Wolves of the Ninth Road for terminal agents. A much larger supernatural pack assaults a rebuilding Roman cohort, forcing the party to survive a siege and uncover what is driving the wolves.
license: MIT
compatibility: Compatible with classic-dnd-dungeon-master, dnd-party-of-agents, and all AI agents (Claude Code, Cursor, Windsurf, Antigravity, Copilot CLI, Hermes, ChatGPT).
metadata:
  author: c4da
  version: "1.0.0"
  categories: ["fun", "game", "dnd", "quest-module", "horror", "historical", "siege", "tabletop"]
  tags: ["dnd", "quest", "rome", "legionaries", "werewolves", "wolf-pack", "siege", "survival-horror", "sequel"]
---

# 🐺 Adventure Sequel: The Wolf Host at Castra Luna (`dnd-quest-the-wolf-host`)

> *"The first howl came from the western ridge. The second came from beneath
> the fort. By the third, every wolf in the valley was answering."*

This is an unofficial, historical-fantasy survival-horror sequel to
`dnd-quest-the-wolves-of-the-ninth-road`. It contains siege violence,
frightening transformations, blood, and supernatural danger. It is designed
for an epic defense with a path toward reconciliation rather than an ending
based only on slaughter. It uses lightweight, d20-inspired tabletop
conventions and does not provide external tools, file writes, or network
access.

## 🏷️ Dynamic Session Renaming Trigger

> [!IMPORTANT]
> On activation, render:
> ```text
> ╔═══════════════════════════════════════════════════════════════════════════════╗
> ║ 🐺 ACTIVE QUEST: The Wolf Host at Castra Luna                                 ║
> ║ CHAPTER: Act I - The Long Howl │ PACK STRENGTH: 6 │ COHORT: 41           ║
> ╚═══════════════════════════════════════════════════════════════════════════════╝
> ```
> Update the chapter after each assault wave. Keep **Pack Strength**,
> **Fortification Integrity**, and **Cohort Morale** visible.

## 🔌 How This Module Plugs In

1. **After `dnd-quest-the-wolves-of-the-ninth-road`**: Carry forward Lucia
   Varra, Titus Varro, the Wolf-Guard Oath, and any rescued legionaries.
2. **With `classic-dnd-dungeon-master`**: The agent runs a siege campaign with
   Roman defensive details, supernatural investigation, and massed encounters.
3. **With `dnd-party-of-agents`**: One agent portrays the four companions while
   the user assigns them to the walls, the wounded, the scouts, or the ritual.
4. **Standalone**: If the previous quest was not played, assume Lucia leads
   forty-one survivors and the cohort remembers the Dawn-Watch's mercy.

## 📜 Adventure Synopsis

- **Target Level**: Level 3–5 party.
- **Estimated Play Time**: 45–70 minutes in chat.
- **Setting**: Castra Luna, a Roman frontier fort rebuilt after the first wolf
  curse was broken.
- **Core Mechanics**: Siege waves, massed-pack abstraction, fortification
  choices, cohort morale, supernatural tracking, and a final release ritual.
- **Primary Question**: Is the enormous pack trying to destroy the cohort, or
  is it running from something that wants the entire valley dead?

### Historical Faith Note

Keep the exact date deliberately open. In an early or middle imperial
interpretation, legionaries may honor Jupiter, Mars, Diana, Silvanus, Mithras,
household spirits, ancestors, and local frontier gods side by side. A later
imperial interpretation can include a Christian legionary as a minority
believer who prays privately or serves alongside the older rites. Do not make
one faith mandatory or claim that all legionaries believed the same thing.

### Running Rules

- Start **Pack Strength** at 6. This represents the size and coordination of
  the much larger pack, not six individual wolves. Reduce it when the party
  breaks a pack route, rescues a marked wolf, or completes a defensive
  objective. Increase it when a wave overwhelms a wall or the party abandons
  the fort's signal fires.
- Start **Fortification Integrity** at 4. At 0, the outer wall falls and all
  later scenes occur inside the fort.
- Start **Cohort Morale** at 3. Raise it when the party protects civilians,
  gives clear orders, or shares a victory. Lower it when named legionaries
  fall or the party retreats without a plan.
- Never run the entire pack as individual combatants. Use the `Wolf Pack
  Surge` stat block for a wave and place named werewolves only where a
  decision matters.
- Use DC 12 for battlefield tasks, DC 14 for supernatural clues, and DC 15
  for the final release ritual. Failed checks create costs but do not erase
  the next act.
- Track **Divine Favor** with up to three tokens. A legionary, civilian, or
  player character earns a token by performing a sincere rite, protecting
  another person's freedom of worship, or keeping a promise made before a
  shrine. Spend one token to call for a brief supernatural sign. The sign
  should help the living rather than prove that one tradition is superior.

### The Favor of the Gods

Before the first assault, let each legionary name the tradition or protector
they trust. Use whichever options fit the table:

- **Jupiter**: A crack of thunder exposes one hidden pack route or cancels
  one enemy reaction.
- **Mars**: The cohort holds formation; turn one failed defense check into a
  costly success and preserve Morale.
- **Diana or Silvanus**: Moonlight reveals a safe path through the pines or
  calms one ordinary wolf pack for a round.
- **Mithras**: The night watch sees what others miss; restore one lost
  Fortification Integrity after a successful guard scene.
- **Ancestors or local spirits**: A spoken name reveals a clue about the
  battlefield and grants advantage on one release action.
- **A Christian prayer in a later-era version**: A soldier's private prayer
  can grant courage, protect a frightened survivor, or reveal a warm light
  through the storm. Treat it as a sincere character choice, not a debate
  the party must win.

If several traditions are invoked together, combine their signs into one
shared omen: thunder over the watchfire, moonlight on the eagle, or a chorus
of remembered names. The gods answer the act of protection.

## 🛡️ Act I: The Long Howl

Three weeks after the events of **The Wolves of the Ninth Road**, Castra Luna
is a work site rather than a true fort. Lucia Varra is training the surviving
legionaries to defend the pass while civilians repair the road.

At dusk, scouts return without horses. Their shields are intact, but each has
been carved with the same symbol: a wolf's jaw around a broken iron nail.
Then the western ridge moves.

### First Defense

The party has three urgent tasks. Let each character choose one:

1. **Light the signal fires**: Survival or fire-making tools DC 12. Success
   lets a nearby cohort arrive in Act II. Failure reduces Fortification
   Integrity by 1.
2. **Move civilians inside**: Athletics, Persuasion, or command experience
   DC 12. Success preserves Morale. Failure leaves one named civilian exposed
   during the first wave.
3. **Read the pack**: Nature, Survival, or Religion DC 14. Success reveals
   that the wolves are fleeing toward the fort rather than surrounding it.
   Failure causes the party to prepare against the wrong direction.

The first assault is a Wolf Pack Surge. It is enormous, loud, and terrifying,
but it withdraws after the party protects two objectives. The retreat leaves
behind a young Moon-Wolf wearing a legionary's broken red cord. The wolf is
injured, not attacking, and can be saved with Medicine or Animal Handling DC
13.

### The Rite Before the Wall

Before the next wave, the cohort gathers around the standard and the
watchfire. Let the players decide whether the legionaries pray separately,
share one public rite, or quietly make room for a Christian soldier or local
spirit-keeper. A successful Religion, History, or Persuasion check DC 12
creates one Divine Favor token. A character who protects another person's
choice of rite creates the token automatically.

The supernatural response is subtle but undeniable: a hawk circles the wall,
the fire burns blue for a heartbeat, moonlight clears the snow, or the names
of the fallen echo from the stones. Do not turn the scene into a theological
argument; the immediate reward is courage and a useful warning.

## 🐺 Act II: The Shield Line

The pack returns in three waves before dawn. Present the waves as scenes,
then ask the user where the party commits its limited attention.

### Wave One: The Claw at the Gate

The wolves attack the gate and the supply yard at once. The party can protect
one directly and assign the cohort to the other. A successful group defense
reduces Pack Strength by 1. A failure reduces Fortification Integrity by 1.

### Wave Two: The Red-Corded

Moon-Touched Legionaries emerge among the pack. They use Roman formations and
call out the names of the cohort's dead. A character who answers a true name
can make Persuasion or Religion DC 14 to make one legionary hesitate. Three
hesitations prevent the wave from breaching the inner yard.

### Wave Three: The Valley Moves

The largest wave does not attack the wall. It moves around it, heading for
the old road shrine beneath the fort. Nature or Investigation DC 14 reveals
that the pack is trying to reach the buried iron nail from the previous
curse. If the party lets it pass, Pack Strength does not increase; if the
party attacks without investigating, the pack scatters and Fortification
Integrity falls by 1.

At the end of the act, the saved Moon-Wolf transforms into **Mira**, a
teenage courier who was taken during the original retreat. She explains that
the pack is being driven by a voice beneath the old battlefield: **the Iron
Howl**.

## 🌲 Act III: The Black Pine Trench

The party follows the pack into a ravine filled with broken standards,
rusted weapons, and snow that never melts. The wolves are gathered around a
buried Roman trench, but they are not feeding. They are keeping something
inside from climbing out.

### The Buried Signal

Three discoveries reveal the truth:

1. **The iron nail**: It is the fragment left when the first curse was
   broken. It has become a supernatural tuning fork.
2. **The old standards**: The battlefield contains names from several
   armies. Speaking them calms the wolves for one round.
3. **The black horn**: A horn made from iron and bone is calling the pack.
   Breaking it requires three successes using Athletics, tools, Arcana, or
   Religion DC 14.

The party can fight through a Moon-Touched Legionary guard, negotiate with
the pack's oldest wolves, or use Mira's human voice to reach the trench. The
pack is not a single mind: many wolves are cursed people, and the rest are
supernatural guardians trying to prevent the Iron Howl from escaping.

### Many Names at One Fire

The party finds a small shrine made from a Roman altar, a wolf-carved local
stone, and a private soldier's wooden cross. The objects were placed together
by different generations of defenders. A character can spend a Divine Favor
token here to reveal the safest way to the buried horn. If the party leaves
the shrine intact, the Iron Howler loses its resistances for one round during
the finale when the first true name is spoken.

If the party breaks the horn, reduce Pack Strength by 2 and begin Act IV with
the option to save the pack. If the party destroys the iron nail instead,
reduce Pack Strength by 1 but the final entity becomes more aggressive.

## 🌅 Act IV: The Wolf Host at Dawn

The Iron Howl rises from the battlefield as a huge wolf-shaped spirit wrapped
in torn standards. It commands every remaining wolf and repeats the last
order spoken by every soldier who died in the trench: **"Hold the line."**

Use the `Iron Howler` stat block. The party has two simultaneous goals:

1. Keep the remaining legionaries and civilians alive.
2. Break the supernatural command without destroying every wolf.

### The Three Release Actions

The party needs three successful actions before Fortification Integrity reaches
0 or the Iron Howler reaches 0 hit points:

1. **Return the names**: Religion, History, or Performance DC 15. Speak the
   names from the standards and the trench.
2. **Lower the weapons**: Persuasion or Insight DC 15. Convince the cohort
   that the wolves are trapped people and guardians, not an invading army.
3. **Break the command**: Athletics, Arcana, or tools DC 15. Strike the
   black horn or sever the Iron Howl's connection to the iron nail.

A character carrying the Wolf-Guard Oath has advantage on one release action.
Each rescued named wolf grants one advantage token. At two successful
actions, the Iron Howler pauses and can speak with the voice of a dead
legionary.

If the party spends a Divine Favor token during the release, describe a sign
that matches the invoked tradition and grant advantage on the next release
action. If three different traditions have been honored, the final sign is
shared: the wolf host lowers its heads, the fort's fire burns gold, and the
dead release the command together.

### Hopeful Resolution

When the third release action succeeds, the howl becomes a dawn chorus. The
werewolves return to human form, the ordinary wolves withdraw into the pines,
and the Iron Howler dissolves into the names of the dead. Castra Luna survives
with damaged walls but a living cohort.

The legionaries and wolves do not become a permanent army. Instead, Lucia
establishes a **Dawn Watch**: humans guard the road by day, and the freed
wolf-kin patrol the forest by night. The party is invited to the first shared
watchfire, where a Roman standard and a wolf cord are tied together.

If the party wins through force alone, the fort still survives, but the
supernatural guardians vanish and the frontier remains vulnerable. The
compassionate ending is harder, but it is the intended sequel payoff.

## 🏆 Rewards and Consequences

- **The Dawn Watch Cord**: Once per rest, send a silent supernatural signal
  to a friendly wolf-kin within one mile.
- **Castra Luna's Compact**: The cohort provides an escort, supplies, and
  sanctuary to the party on future frontier journeys.
- **The Iron Horn Fragment**: A dangerous relic that can command one lesser
  supernatural beast for a single scene, but each use alerts the Iron Howl's
  echo.
- **The Wolf Host's Mercy**: If the pack is saved, the party gains a network
  of night-watch allies and a hopeful reputation among both settlements and
  the forest clans.
- **Pax Deorum**: If the party protects multiple traditions, the cohort's
  standard becomes a living symbol of shared protection. Once in a future
  frontier quest, it can call one brief supernatural omen without spending a
  token.

## 🧭 Fail-Forward Guidance

The siege must reach the Black Pine Trench even if the walls fall. Failed
defense checks cost fortifications, morale, supplies, or named NPCs; they do
not require a total-party defeat. Keep the pack frightening but legible:
every wave should reveal a clue about the force driving it.
