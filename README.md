# 🐉 DnD-Agents (`#tabletop-ai`)

> **Play Authentic Classic D&D in Your Terminal with Autonomous AI Companions**  
> *Did your real-life gaming group cancel game night for the 4th consecutive week?*  
> Summon an autonomous 4-member adventuring party or an old-school Dungeon Master right in your CLI.  
> Compatible with **Claude Code**, **Cursor**, **Windsurf**, **Antigravity**, **GitHub Copilot CLI**, and **Hermes**.

[![GitHub Topics](https://img.shields.io/badge/topic-%23tabletop--ai-purple.svg)](https://github.com/topics/dnd)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![SkillsMP Indexed](https://img.shields.io/badge/Indexed-SkillsMP-success.svg)](https://skillsmp.com)
[![Pure Tabletop](https://img.shields.io/badge/Rules-100%25%20Pure%20D%26D-red.svg)](README.md)

---

## ❓ Why Does This Exist?

Every tabletop RPG player knows the heartbreak: the campaign is planned, your character sheet is polished, your dice are ready... and then three people cancel at 6:30 PM.

**DnD-Agents solves the scheduling curse forever.**

Whether you want to play a solo dungeon crawl with a vintage 1980s Gary Gygax-style Dungeon Master, or run an adventure where an autonomous AI party argues over marching order, investigates pit traps, and casts Fireball in character—DnD-Agents brings full tabletop roleplaying to your terminal.

---

## 📦 What's Inside the Box?

```text
dnd-agents/
├── skills/
│   ├── classic-dnd-dungeon-master    # The 1980s DM Engine (ASCII maps, d20 checks, AC, HP, wandering monsters)
│   ├── dnd-party-of-agents           # The 4 Autonomous AI Companions (Paladin, Barbarian, Rogue, Wizard)
│   └── dnd-quest-the-lost-shrine     # Starter Adventure Module: "The Lost Shrine of the Sun-Stone"
```

### 1. 🎲 `classic-dnd-dungeon-master`
The complete tabletop engine:
- **Automatic Session Naming**: Automatically titles your session after your origin (`D&D Campaign // The Ash-Fall of Elmridge`) and dynamically updates when quests trigger.
- **Neverwinter Nights Starting Origins**: Choose from 4 iconic origins—including the tragic midnight massacre of your home village Elmridge!
- **Roguelike ASCII tactical maps** for every chamber, corridor, burning street, and cavern.
- **D20 checks and saving throws** (Dexterity vs. dragon breath, Constitution vs. poison).
- **Turn-based initiative combat** tracking HP, Armor Class, and spell slots.
- **Authentic wandering monster tables** (Owlbears, Gelatinous Cubes, Mimics, Dragons).

### 2. 🛡️ `dnd-party-of-agents`
An opinionated, full 4-member adventuring party:
- **Sir Valerius (Paladin)**: Plate armor, holy longsword. Devout, honorable, protects the party with *Divine Smite* and *Lay on Hands*.
- **Thokk Ironbreaker (Barbarian)**: Greataxe, unarmored defense. Kicks down doors, rages, screams war cries, and hates complicated plans.
- **Lyra Nightshade (Rogue)**: Dual daggers, shortbow, thieves' tools. Checks for tripwires, picks rusted iron locks, and strikes with *Sneak Attack*.
- **Ignis Shadowweaver (Wizard)**: Starry robes, arcane focus, spellbook. Casts *Detect Magic*, *Fireball*, *Shield*, and complains when his robes get muddy.

### 3. 🗝️ `dnd-quest-the-lost-shrine` (Modular Adventure Quest)
A turnkey starter quest (*The Lost Shrine of the Sun-Stone*) designed to test and showcase all core mechanics:
- **Act I**: Wilderness tracking, Passive Perception vs. Goblin Stealth, Ranged Ambush.
- **Act II**: Poison dart pressure plates, Thieves' Tools disarm check, the ancient Sun-Riddle.
- **Act III**: Tactical boss battle against *Kragthor the Bugbear Chief* and Skeleton Guardians (Bludgeoning vulnerability).
- **Act IV**: Relic recovery, potion looting, and leveling up to Level 2.

---

## ⚡ 1-Line Quick Install

### Claude Code
```bash
npx @agensi/skills add classic-dnd-dungeon-master
# Or install the full party
npx @agensi/skills add dnd-party-of-agents
```

### Antigravity & Agent Environments
```bash
git clone https://github.com/c4da/dnd-agents.git
cp -r dnd-agents/skills/* ~/.gemini/antigravity/skills/
```

### Cursor & Windsurf
Copy the contents of `classic-dnd-dungeon-master/SKILL.md` or `dnd-party-of-agents/SKILL.md` into your `.cursorrules` or `.windsurfrules`.

---

## 🎮 How to Play

### Mode A: You are the Dungeon Master (Run an Adventure for the AI Party)
Describe the environment, monsters, and traps. The AI party will talk in character, propose tactics, roll d20 dice, and react to your rulings:

```text
DM (You): You stand before the subterranean crypt of the Lich Lord. 
The double oak doors are sealed with three glowing purple warding runes.

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

### Mode B: Solo Dungeon Crawl (The AI is your Dungeon Master)
The DM generates the world, renders ASCII dungeon maps, and calls for your rolls:

```text
User: I carefully inspect the stone sarcophagus for traps before opening it.

DM:
*Behind the cardboard DM screen, polyhedral dice clatter against felt.*
"You step lightly around the stone perimeter, running your gauntlets along the carved elven runes."
Roll an Intelligence (Investigation) check, DC 13!

User: /roll

DM:
         / \
        / 15\    [ D20 ROLL: 15 + 0 (INT Mod) = 15 ]
       /_____\   >> SUCCESS! (DC 13 Passed)

"Your sharp eye catches a hairline groove along the rim of the lid. A thin silver wire 
leads down into a lead pipe filled with sleep gas!
With a steady hand and your dagger, you snip the tripwire cleanly. The trap is disarmed!
Inside lies a skeletal knight clutching a +1 Silver Shortsword and a velvet pouch with 45 ancient gold pieces!"
```

---

## 🗺️ Roguelike ASCII Visuals

```text
       # # # # # # # # # # # # # # # # # # # #
       # . . . . . . . [ALTAR/$] . . . . . . #   LEGEND:
       # . . . . . . . . . K . . . . . . . . #   K = Kragthor (Bugbear Boss)
       # . . P . . . . . . . . . . . . P . . #   P = Stone Pillar (Half-Cover)
       # . . Z . . . . . . . . . . . . Z . . #   Z = Skeleton Guardians (Vulnerable to Bludgeoning)
       # . . . . . . . . . . . . . . . . . . #   $ = Sun-Stone on Altar
       # . . . . . . . . @ . . . . . . . . . #   @ = The Party
       # # # # # # # # # + # # # # # # # # # #
```

---

## ✍️ How to Write Custom Quest Modules

Want to write your own adventure module? Simply create a new folder under `skills/dnd-quest-<your-adventure-name>` following this template:
1. `SKILL.md`: Frontmatter, synopsis, and 3–4 Acts detailing scenes, traps, and boss encounters.
2. `references/encounter-maps.md`: ASCII maps with coordinate legends.
3. `references/monster-statblocks.md`: D&D 5e / AD&D stat blocks (AC, HP, Actions, Weaknesses).
4. Run `python tools/validate_catalog.py` to cryptographically sign your quest into `registry.json`!

---

## 🛠️ Verification & Cryptographic Provenance

Every skill and quest module includes an official `manifest.json` and cryptographically verifiable SHA-256 hash:
```bash
python tools/validate_catalog.py
```

---

## 📄 License
MIT License. Open-source tabletop gaming for solitary adventurers everywhere.
