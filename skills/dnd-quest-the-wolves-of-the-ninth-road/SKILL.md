---
name: dnd-quest-the-wolves-of-the-ninth-road
description: An unofficial, prompt-based Roman frontier survival-horror adventure for terminal agents. The party escorts battered legionaries through a supernatural winter, faces werewolves, and can break the curse for a hard-won hopeful ending.
license: MIT
compatibility: Compatible with classic-dnd-dungeon-master, dnd-party-of-agents, and all AI agents (Claude Code, Cursor, Windsurf, Antigravity, Copilot CLI, Hermes, ChatGPT).
metadata:
  author: c4da
  version: "1.0.0"
  categories: ["fun", "game", "dnd", "quest-module", "horror", "historical", "survival", "tabletop"]
  tags: ["dnd", "quest", "rome", "roman-frontier", "legionaries", "werewolves", "supernatural", "survival-horror", "hopeful-ending"]
---

# 🐺 Adventure Module: The Wolves of the Ninth Road (`dnd-quest-the-wolves-of-the-ninth-road`)

> *"At sunset, the legionaries counted eighteen survivors. At moonrise, they
> heard nineteen heartbeats in the snow."*

This is an unofficial fan-made historical-fantasy survival-horror module. It
uses an imaginative Roman frontier setting rather than claiming historical
accuracy. It contains frightening transformations, blood, predation, and
supernatural danger, but is designed to reach a hopeful ending when the party
protects the living and breaks the curse. It uses lightweight, d20-inspired
tabletop conventions and does not provide external tools, file writes, or
network access.

## 🏷️ Dynamic Session Renaming Trigger

> [!IMPORTANT]
> On activation, render:
> ```text
> ╔═══════════════════════════════════════════════════════════════════════════════╗
> ║ 🐺 ACTIVE QUEST: The Wolves of the Ninth Road                                ║
> ║ CHAPTER: Act I - Snow on the Ninth Road │ COHORT: 18 survivors             ║
> ╚═══════════════════════════════════════════════════════════════════════════════╝
> ```
> Update the chapter at each camp or major discovery. Keep the **Nightfall
> Clock**, **Cohort Morale**, and surviving names visible.

## 🔌 How This Module Plugs In

1. **With `classic-dnd-dungeon-master`**: The agent runs a tense frontier
   journey with survival choices, Roman military details, and supernatural
   investigations.
2. **With `dnd-party-of-agents`**: One agent portrays the four companions
   while the user decides whether the party protects, abandons, or trusts the
   surviving legionaries.
3. **Standalone**: Use this file as the system prompt and treat the user as
   the leader of a mixed civilian and military escort.

## 📜 Adventure Synopsis

- **Target Level**: Level 2–4 party.
- **Estimated Play Time**: 30–50 minutes in chat.
- **Setting**: Rome's snowbound northern frontier, between a ruined fort and a
  remote mountain shrine.
- **Core Mechanics**: Travel survival, cohort morale, moonlit hunts, Roman
  camp discipline, werewolf investigation, and a hopeful curse-breaking
  finale.
- **Primary Question**: Can the party save the people who were turned into
  monsters without becoming monsters themselves?

### Running Rules

- Keep a visible four-segment **Nightfall Clock**. Mark one segment for a
  failed travel check, abandoning a wounded survivor, or spending too long
  exposed after sunset.
- At two segments, the wolves begin circling camp. At four segments, the
  final confrontation starts under a full moon and the first ritual check has
  disadvantage.
- Keep **Cohort Morale** at 3. Reduce it when the party loses a named
  survivor, breaks a promise, or flees without a plan. Raise it when the party
  shares supplies, protects the standard, or gives the cohort a clear order.
- Werewolves are cursed people, not disposable monsters. Give the party clues
  that allow mercy before every major fight.
- Use DC 11 for routine survival, DC 13 for dangerous travel or military
  decisions, and DC 15 for curse-breaking or occult actions.

## 🛡️ Act I: Snow on the Ninth Road

The party finds a broken Roman convoy at dusk. Eighteen legionaries and
camp-followers are crowded around a splintered wagon. Their fort, **Castra
Alba**, fell two nights earlier. They carry the eagle standard of the
fictional **Cohors XII Vespera**, but no one agrees on who gave the order to
retreat.

### Three First Clues

1. **The torn ration sack**: Survival or Investigation DC 11 reveals that the
   claw marks began inside the wagon. The first transformed soldier was
   already among the survivors.
2. **The silver nail**: History or Religion DC 13 identifies a moon-silver
   nail driven into the standard's base. It is not a weapon; it is part of an
   old oath-binding.
3. **The witness**: Medicine or Persuasion DC 12 helps the wounded signifer,
   **Lucia Varra**, remember that the wolves stopped attacking when a
   legionary recited the names of the dead.

### The Marching Choice

The party chooses one route:

- **The military road**: Faster, exposed, and easy for the wolves to track.
  Success on a group Survival check DC 12 preserves one Morale.
- **The old shrine path**: Slower but protected by stone markers. A Religion
  or History check DC 13 reveals that the markers predate Rome and were later
  incorporated into the road.
- **The frozen river**: Avoids the road but risks collapse. Athletics or
  Nature DC 13; failure separates one named survivor until Act II.

At the end of the act, a lone wolf watches from a ridge. It wears a strip of
Roman red cloth around its neck and does not attack. If the party follows it,
they find a bloodless legionary helmet and the first mark of the moon shrine.

## 🌨️ Act II: The White Pass

The convoy enters a narrow pass where snow muffles every command. Roman
discipline keeps the group moving, but every campfire reveals more tracks than
there are travelers.

### Survival Scenes

Run two scenes and one night encounter:

1. **Avalanche shelf**: Athletics, Acrobatics, or clever rope work DC 13.
   Failure costs one Morale or leaves a pack animal behind.
2. **The frozen watchpost**: Investigation DC 12 finds a sealed message from
   the fort's commander: *"Do not kill the marked. The curse is a sentence,
   not a nature."*
3. **The hungry camp**: The party has enough food for either the legionaries
   or the civilians. Sharing the ration and making a group Constitution check
   DC 11 preserves Morale; hoarding it marks the Nightfall Clock.

### The Night Hunt

During the encounter, use one Cursed Legionary and two Moon-Wolves. The
legionary fights from the edge of the firelight, then drops its weapon when a
character calls it by its human name. A successful Persuasion, Medicine, or
Religion check DC 13 reveals that the transformed soldier is **Titus Varro**,
the missing standard-bearer.

Titus cannot remain human until the curse is broken, but he gives the party a
crucial warning: the wolves gather at **Mons Luna**, where the old shrine and
the ruined watchtower stand together. The pack's leader is not hunting the
cohort for sport. It is trying to keep the curse from spreading beyond the
mountains.

## 🏛️ Act III: Mons Luna and the Old Oath

At the mountain shrine, the party finds Roman stones built around an older
moon altar. The ruined watchtower contains the names of legionaries who died
when the first road was cut through the sacred grove.

### The Truth of the Curse

Long ago, a frightened Roman commander ordered the grove burned to clear a
road. The soldiers obeyed, but the centurion **Gaius Aemilius** refused to
burn the shrine. He took the moon-silver nail and swore that no soldier
would ever abandon the innocent again. The oath saved the village, but bound
the centurion and anyone who carried the eagle standard to the wolf curse.

The curse has three anchors:

1. **The Eagle Standard**: It must be planted at the shrine.
2. **The Names of the Dead**: The fallen must be spoken without omission.
3. **The Watchfire**: A living person must keep the fire lit until dawn.

The party can discover each anchor with Investigation, History, or Religion
checks DC 13. At least two discoveries are enough to attempt the finale; all
three grant advantage on the first ritual action.

### The Watchtower Choice

The party may:

- **Defend the survivors** while Lucia prepares the names. This raises
  Morale if successful.
- **Hunt the wolf-centurion** before moonrise. This gives the party the
  initiative but risks losing the standard.
- **Invite the pack to the fire**. A character who lowers a weapon and speaks
  a true name can make a Persuasion check DC 14. Success reveals that several
  wolves are transformed legionaries who want to return to human form.

No choice removes the happy ending. Violence makes the final ritual harder,
but a character can still call the centurion back from the curse.

## 🌅 Act IV: Dawn at Castra Luna

The final confrontation begins at the ruined fort as the moon reaches its
highest point. The wolf-centurion, Gaius Aemilius, stands before the broken
gate with the eagle standard in his claws. Use the Wolf-Centurion stat block.

### The Three-Part Release

The party needs three successful actions before the centurion reaches 0 hit
points:

1. **Plant the standard**: Athletics or History DC 13. A legionary can assist.
2. **Speak the names**: Religion, Performance, or Persuasion DC 13. Every
   rescued survivor or restored Morale grants one advantage token.
3. **Keep the watchfire**: Survival, Arcana, or a fire-making tool check DC
   13. A character must spend the round protecting the flame.

The centurion attacks between ritual actions, but at half hit points it
hesitates when someone speaks the name of a fallen soldier. A successful
Persuasion or Religion check DC 14 immediately lets the party attempt the
next ritual action without another attack.

### Happy Ending

When the third ritual action succeeds, dawn breaks over the pass. The
werewolves collapse into exhausted human soldiers, the moon-silver nail
shatters, and the wolves that were never human retreat into the forest.
Lucia raises the eagle standard over the survivors, not as a symbol of
conquest but as a promise that no one will be abandoned on the road again.

If the party killed some transformed soldiers, the curse still breaks for the
survivors. The ending becomes mournful rather than tragic: the cohort builds a
memorial and carries the names to Rome.

## 🏆 Rewards and Consequences

- **The Wolf-Guard Oath**: Once per rest, call a spectral wolf to track a
  supernatural creature or warn the party of an ambush.
- **The Silver Nail**: Reforged into a small pendant, it grants advantage on
  one saving throw against a curse or transformation.
- **The Cohort's Standard**: The surviving legionaries escort the party safely
  to the nearest Roman settlement and testify to the party's mercy.
- **A Living Legend**: The people of the frontier remember the party as the
  Dawn-Watch, protectors who returned monsters to human form.

## 🧭 Fail-Forward Guidance

The party must reach Mons Luna and receive enough information to attempt the
release. Failed checks cost supplies, Morale, time, or hit points; they do not
force a hopeless ending. Keep the horror in the fictional setting, let the
players skip transformation details, and preserve the possibility of mercy
until the final ritual.
