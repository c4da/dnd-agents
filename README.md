# 🐉 DnD-Agents (`#tabletop-ai`)

> **Unofficial tabletop fantasy roleplay skills for AI agents**
> Play a solo dungeon crawl, run one of several original starter quests, or ask one compatible agent to portray a four-character adventuring party.
> Prompt-based, terminal-friendly, and compatible with **Claude Code**, **Cursor**, **Windsurf**, **Antigravity**, **GitHub Copilot CLI**, and **Hermes**.

[![GitHub Topics](https://img.shields.io/badge/topics-ai--skills%20%7C%20agent--skills%20%7C%20skill--md-purple.svg)](https://github.com/c4da/dnd-agents/topics)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![SkillsMarket](https://img.shields.io/badge/SkillsMarket-submit-blue.svg)](https://aiskillsmarket.com/submit)
[![Fan-made](https://img.shields.io/badge/status-unofficial%20fan--made-orange.svg)](NOTICE.md)

> **Notice:** This is an unofficial fan-made project. It is not affiliated with
> or endorsed by Wizards of the Coast or any other rights holder. See
> [NOTICE.md](NOTICE.md) before redistributing or monetizing listings.

**Discovery tags:** `#ai-skills` `#agent-skills` `#skill-md` `#tabletop-ai`
`#dnd` `#rpg` `#open-source`

Marketplace indexes can use [`registry.json`](registry.json) for the catalog or
install an individual package from `skills/<skill-name>/`. Each package is
self-contained and includes `SKILL.md`, machine-readable `manifest.json`, and
any referenced content files.

## 🖼️ Campaign Flyers

<p align="center">
  <img src="assets/dnd-agents-cover.jpg" alt="Original high-fantasy DnD-Agents campaign flyer" width="900">
</p>

<p align="center">
  <img src="assets/the-red-tithe-flyer.jpg" alt="The Red Tithe dark-gothic campaign flyer" width="49%">
  <img src="assets/the-wolves-of-the-ninth-road-flyer.jpg" alt="The Wolves of the Ninth Road Roman frontier horror flyer" width="49%">
</p>

These are original promotional illustrations for this repository. They do not
depict Forgotten Realms or any other third-party setting, characters, logos,
or trademarked artwork.

---

## ❓ Why Does This Exist?

Every tabletop RPG player knows the heartbreak: the campaign is planned, your
character sheet is polished, your dice are ready... and then three people
cancel at 6:30 PM.

DnD-Agents turns a compatible AI agent into a lightweight, in-chat tabletop
roleplay partner. It is intentionally prompt-only: there is no executable
runtime, no external tool access, no file writing, and no network dependency.

---

## 📦 What's Inside the Box?

```text
dnd-agents/
├── assets/                         # README campaign flyers
├── skills/
│   ├── classic-dnd-dungeon-master    # Prompt-based fantasy DM with ASCII maps and d20-style checks
│   ├── dnd-party-of-agents           # One agent portraying a Paladin, Barbarian, Rogue, and Wizard
│   ├── dnd-quest-the-lost-shrine     # Starter Adventure Module: "The Lost Shrine of the Sun-Stone"
│   ├── dnd-quest-the-hollow-lighthouse # Coastal mystery with a rising-tide clock
│   ├── dnd-quest-the-ember-vault     # Underground rescue with a rising-heat clock
│   ├── dnd-quest-the-sunken-observatory # Flooded ruin with a star-map puzzle
│   ├── dnd-quest-the-red-tithe        # Dark-gothic, graphic-fantasy campaign
│   └── dnd-quest-the-wolves-of-the-ninth-road # Roman frontier werewolf survival horror
```

### 1. 🎲 `classic-dnd-dungeon-master`
The complete roleplay prompt:
- **In-chat Session Banners**: Starts a campaign header and updates it when a quest is activated.
- **Four Cinematic Origins**: Choose from atmospheric fantasy prologues, including the Ash-Fall of Elmridge.
- **Roguelike ASCII tactical maps** for every chamber, corridor, burning street, and cavern.
- **Lightweight d20 checks and saving throws** (Dexterity vs. dragon breath, Constitution vs. poison).
- **Turn-based initiative combat** tracking HP, Armor Class, and spell slots.
- **Wandering encounter tables** with classic fantasy creatures.

### 2. 🛡️ `dnd-party-of-agents`
An opinionated, four-character party portrayed by one compatible agent:
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

### Additional quest modules

- **`dnd-quest-the-hollow-lighthouse`**: Investigate missing crews, navigate
  flooded tunnels, and redeem or defeat a bound lighthouse keeper.
- **`dnd-quest-the-ember-vault`**: Rescue trapped stonewrights, manage a
  rising heat clock, and stabilize or seal a dangerous ember engine.
- **`dnd-quest-the-sunken-observatory`**: Climb Compass Ridge, solve a
  constellation map, and decide the fate of a lonely astral caretaker.
- **`dnd-quest-the-red-tithe`**: Cross a dying city, descend through an
  ossuary of stolen names, and confront the bell beneath the cathedral.
- **`dnd-quest-the-wolves-of-the-ninth-road`**: Escort Roman legionaries
  through a supernatural winter, face werewolves, and break the curse before
  dawn.

> **Content note:** `dnd-quest-the-red-tithe` is intentionally grim and
> includes graphic fantasy violence, ritual horror, plague imagery, and bleak
> choices. The skill includes guidance for softening or skipping descriptions.
> `dnd-quest-the-wolves-of-the-ninth-road` contains survival horror and
> frightening transformations, but is written toward a hopeful ending.

---

## ⚡ Install

### SkillsMarket

Browse or submit the skills at [SkillsMarket](https://aiskillsmarket.com/submit).
The marketplace requires an account to submit a skill.

### Manual installation

```bash
git clone https://github.com/c4da/dnd-agents.git
cp -r dnd-agents/skills/* ~/.gemini/antigravity/skills/
```

On Windows PowerShell:

```powershell
git clone https://github.com/c4da/dnd-agents.git
Copy-Item -Recurse .\dnd-agents\skills\* "$HOME\.gemini\antigravity\skills\"
```

For another compatible agent, install the selected skill according to that
agent's `SKILL.md` directory convention or paste the file into its supported
system-prompt configuration.

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
3. `references/monster-statblocks.md`: Fantasy stat blocks (AC, HP, Actions, Weaknesses).
4. Run `python tools/validate_catalog.py` to update the catalog hashes, then
   run `python tools/validate_catalog.py --check` before publishing.

---

## 🛠️ Verification & Cryptographic Provenance

Every skill and quest module includes a manifest and a reproducible SHA-256
package hash covering `SKILL.md` and its reference files. The generated
manifest is excluded to avoid a self-referential hash:
```bash
python tools/validate_catalog.py
python tools/validate_catalog.py --check
```

The hash proves package integrity after publication; it is not a digital
signature or proof of author identity.

---

## Optional AgentTrace integration

AgentTrace is a separate project. These skills do not require it, but an
AgentTrace gateway can be used by agent workflows that need session telemetry,
policy enforcement, or an audit trail.

## 📄 License
Original project material is released under the [MIT License](LICENSE). See
[NOTICE.md](NOTICE.md) for the fan-made and third-party rights notice.
