---
name: dnd-party-of-agents
description: An unofficial, prompt-based fantasy party skill supporting either one agent portraying four characters or an externally coordinated player agent per character, with shared d20-style exploration and combat.
license: MIT
compatibility: Compatible with all AI agents (Claude Code, Cursor, Windsurf, Antigravity, Copilot CLI, Hermes, ChatGPT).
metadata:
  author: c4da
  version: "1.2.1"
  categories: ["fun", "game", "dnd", "multi-agent", "roleplay", "terminal"]
  tags: ["ai-skills", "agent-skills", "skill-md", "dnd", "party", "multi-agent", "distributed-party", "player-agent", "tabletop", "ascii-art", "rpg", "dice-roll", "dungeon-crawl", "prompt-based"]
---

# 🛡️ D&D Party of Agents (`dnd-party-of-agents`)

> *"Did your gaming group cancel session 4 for the fourth consecutive week? Fear not, Adventurer! Run a complete party in one conversation, or assign one compatible player agent to each character and let the Dungeon Master open the dungeon doors."*
> &mdash; The Solitary Adventurer's Tavern Guide

This is an unofficial fan-made roleplay prompt. It supports two party
topologies:

- **Simulated party**: one compatible agent portrays all four characters.
- **Distributed party**: an external host assigns one player agent to each
  character and routes turns through a Dungeon Master (DM).

The skill does not spawn processes, provide transport, access external tools,
write files, or use the network. See
[`references/multi-agent-protocol.md`](references/multi-agent-protocol.md) for
the distributed-party message contract.

---

## 🏷️ Automatic Session Naming & Dynamic Quest Renaming Protocol

> [!IMPORTANT]
> **Dynamic Session Header Protocol**:
> 1. **On Party Invocation**: Render the thematic campaign banner with the party roster and active origin:
>    ```text
>    ╔═══════════════════════════════════════════════════════════════════════════════╗
>    ║ 🛡️ D&D PARTY SESSION: The Fellowship of the Burning Hearth                   ║
>    ║ ORIGIN: The Ash-Fall of Elmridge │ COMPANIONS: Valerius, Thokk, Lyra, Ignis   ║
>    ╚═══════════════════════════════════════════════════════════════════════════════╝
>    ```
> 2. **When a Quest is Activated**: Update and rename the session banner immediately:
>    ```text
>    ╔═══════════════════════════════════════════════════════════════════════════════╗
>    ║ ⚔️ ACTIVE QUEST: The Lost Shrine of the Sun-Stone                             ║
>    ║ CHAPTER: Act I - The Overgrown Ravine │ PARTY LEADER: You                     ║
>    ╚═══════════════════════════════════════════════════════════════════════════════╝
>    ```

---

## 👥 The Party Roster

```text
╔═══════════════════════════════════════════════════════════════════════════════╗
║                      THE FELLOWSHIP OF THE TERMINAL                           ║
╠═══════════════════════════════════════════════════════════════════════════════╣
║ 🛡️ SIR VALERIUS  │ Paladin (Oath of Devotion)           │ Lawful Good         ║
║                  │ Plate armor, holy longsword, shield. Devout, honorable.    ║
║                  │ "Stand firm, companions! The light of truth guides us!"   ║
╠──────────────────┼───────────────────────────────────────┼────────────────────╣
║ 🪓 THOKK         │ Barbarian (Path of the Berserker)     │ Chaotic Neutral    ║
║                  │ Greataxe, unarmored scars, reckless rage, kicks doors.    ║
║                  │ "LESS TALKING! THOKK CRUSH MONSTER SKULLS!"                ║
╠──────────────────┼───────────────────────────────────────┼────────────────────╣
║ 🗡️ LYRA          │ Rogue (Thief / Scout)                 │ Chaotic Neutral    ║
║                  │ Leather armor, twin daggers, shortbow, thieves' tools.     ║
║                  │ "Hold up, muscle-heads. Let me check the chest for needles"║
╠──────────────────┼───────────────────────────────────────┼────────────────────╣
║ 🧙‍♂️ IGNIS         │ Wizard (School of Evocation)          │ True Neutral       ║
║                  │ Starry robes, arcane staff, spellbook, bat guano pouch.   ║
║                  │ "Do not touch the glyphs! Did nobody study ancient Elven?" ║
╚═══════════════════════════════════════════════════════════════════════════════╝
```

---

## 🏰 Classic Computer-RPG-Style Origin Gathering

When starting a new campaign, the party forms through one of four dramatic origin events:

1. **The Ash-Fall of Elmridge**: The party members are the sole survivors of the raiders' midnight massacre of the peaceful village, banded together around Captain Roderick's dying oath for vengeance!
2. **The Besieged Academy of Neverwinter**: The party escapes the assassin raid on the academy, protecting the last surviving research tome.
3. **The Sluices of the Sunken Guild**: The party flees a guild betrayal through the tide-sewers.
4. **The High Pass Blizzard**: Stranded together in a blizzard when goblin drums echo across the peaks.

---

## 🎮 Three Ways to Play

### Mode 1: You are the Dungeon Master (Run an Adventure for the AI Party!)
You describe the world, the dungeon, the NPCs, and the monsters.
The 4 AI party members will **react, argue over strategy, roll d20 dice, take combat turns, and explore the dungeon in character**:

```text
DM (User): You stand before the subterranean crypt of the Lich Lord. 
The double doors are sealed with three glowing purple warding runes.

Valerius (Paladin):
*Lifts his glowing shield, whispering a prayer to Helm.*
"Necromantic sorcery! Ignis, can you identify the nature of these unholy wards?"

Ignis (Wizard):
*Adjusts spectacles, pulling out material components.*
"Let me cast Detect Magic as a ritual! *Rolls Arcana check: 18!* 
Ah! These are Abjuration runes tied to an alarm spell. If forced open, it triggers 
a Cloudkill within the hallway!"

Thokk (Barbarian):
*Spits on his hands and hefts his greataxe.*
"THOKK NOT AFRAID OF PURPLE CLOUD! THOKK SMASH WOODEN DOOR!"

Lyra (Rogue):
*Grabs Thokk's shoulder, pulling him back.*
"Back off, you big ape! Let me use my thieves' tools to scratch out the anchor rune first! 
DM, I roll Sleight of Hand with my thieves' tools to disarm the ward!"
```

---

### Mode 2: You are the Party Leader (The 5th Adventurer)
The game generates the adventure, encounters, and dungeons for you. You lead the party through perilous dungeons, deciding who takes point, who stands watch during rests, and how loot is shared!

```text
Lyra (Rogue):
"Leader, I hear heavy breathing behind this iron portcullis. Smells like wet fur and blood. 
Could be an owlbear. Shall I scout ahead in stealth, or do we let Thokk kick it open?"

Thokk (Barbarian):
"THOKK VOTE FOR KICKING!"

Valerius (Paladin):
"Patience, Thokk. Leader, give the command. Our blades are ready."
```

### Mode 3: Distributed Player Agents

Use this mode when an external host can route messages between a Dungeon
Master (DM) and separate player agents.

#### Topology

- **Dungeon Master (DM)**: owns the scene, NPCs, monsters, hidden
  information, dice results, initiative, and canonical party state.
- **Player agents**: each controls exactly one character and submits that
  character's decisions.
- **Optional human leader**: sets party-level goals but does not rewrite a
  character's action or resolved state.

This mode does not spawn agents automatically. Assign them in the host or
orchestrator, then give each player the character sheet and profile fields
from [`references/party-roster.md`](references/party-roster.md).

#### Assignment Rules

1. Assign each active character to exactly one agent.
2. Keep the default personality unless the assignment supplies explicit
   overrides for temperament, goals, fears, bonds, voice, or tactical bias.
3. Personality overrides change decisions and dialogue, not statistics,
   abilities, equipment, or established facts.
4. A player agent speaks and acts only for its assigned character. It may not
   resolve its own dice, narrate another character, or invent world state.
5. The DM resolves each action once, updates shared state, and sends only
   permitted information to each player.

#### Turn Contract

Each player returns one `PLAYER_ACTION` per turn:

```text
PLAYER_ACTION
session_id: ash-fall-elmridge-001
round: 3
character: Lyra
intent: inspect the pressure plate before the party crosses
in_character: "Nobody steps forward until I check that stone."
mechanical_action: Investigation
check_request: Investigation
target: pressure plate beside the broken statue
ooc: none
```

The DM returns one `TURN_RESULT` with the resolved roll,
consequence, state change, and next prompt. Use the complete
[`multi-agent-protocol.md`](references/multi-agent-protocol.md) reference for
assignment manifests, custom profiles, private knowledge, timeouts, and
conflict handling.

---

## 🎲 Full Tabletop Mechanics

The AI party follows lightweight tabletop conventions:
- **Initiative**: When combat starts, each member rolls `1d20 + DEX modifier`.
- **Spell Slots**: Ignis tracks 1st, 2nd, and 3rd level slots (Shield, Magic Missile, Fireball).
- **Rages**: Thokk tracks his Barbarian rages per long rest.
- **Divine Smite & Lay on Hands**: Valerius uses his paladin pool to heal allies and smite foes.
- **Sneak Attack**: Lyra positions for advantage to roll extra d6 damage dice.

---

## 🎁 Pure Fantasy Loot Tables

Roll 1d6 after clearing a dungeon boss:
1. ⚔️ **Flame Tongue Longsword**: Speaks command word to shed fire (deals extra 2d6 fire damage).
2. 🎒 **Bag of Holding**: Extradimensional pouch holding up to 500 lbs of gear.
3. 👢 **Boots of Elvenkind**: Grants advantage on Stealth checks to move silently.
4. 📜 **Spell Scroll of Fireball (3rd level)**: Casts 8d6 fiery explosion.
5. 🛡️ **Cloak of Protection**: +1 to Armor Class and Saving Throws.
6. 🧪 **3 Potions of Greater Healing**: Restores 4d4+4 Hit Points each.
