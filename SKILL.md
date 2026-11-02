---
name: dnd-agents
description: A collection of unofficial, prompt-based tabletop fantasy skills for AI agents, including a Dungeon Master, a single-agent or distributed four-character party, and seven original adventure modules.
license: MIT
compatibility: Compatible with all AI agents that support SKILL.md or system prompts, including Claude Code, Cursor, Windsurf, Antigravity, GitHub Copilot CLI, Hermes, and ChatGPT.
metadata:
  author: c4da
  version: "1.1.0"
  categories: ["fun", "game", "dnd", "tabletop", "ai-skills"]
  tags: ["ai-skills", "agent-skills", "skill-md", "tabletop-ai", "dnd", "rpg", "adventure-modules", "open-source"]
---

# 🐉 DnD-Agents

This root skill is the main entrypoint and campaign router for the DnD-Agents collection.
It is a prompt-only catalog of tabletop roleplay tools and original adventure
modules. It does not spawn processes, access external tools, write files, or
use the network.

## 🎲 Choose a Mode

When this skill is loaded, ask the user which mode they want:

1. **Dungeon Master**: Use
   [`classic-dnd-dungeon-master`](skills/classic-dnd-dungeon-master/SKILL.md)
   to run a solo or group fantasy adventure.
2. **Four-character party**: Use
   [`dnd-party-of-agents`](skills/dnd-party-of-agents/SKILL.md) for either one
   compatible agent portraying a Paladin, Barbarian, Rogue, and Wizard, or a
   distributed setup with one player agent per character and a Dungeon Master
   (DM) coordinating the session.
3. **Adventure module**: Choose one of the quests below and run it with the
   Dungeon Master or party skill.

The distributed mode still requires an external host to assign agents and
route messages; the skill itself does not spawn processes or provide
transport. The single-agent mode asks one compatible agent to portray four
characters in a single conversation.

## 🗺️ Adventure Modules

| Module | Tone | Suggested party |
|---|---|---:|
| [The Lost Shrine of the Sun-Stone](skills/dnd-quest-the-lost-shrine/SKILL.md) | Classic fantasy adventure | 1–3 |
| [The Hollow Lighthouse](skills/dnd-quest-the-hollow-lighthouse/SKILL.md) | Coastal mystery | 1–3 |
| [The Ember Vault](skills/dnd-quest-the-ember-vault/SKILL.md) | Industrial dungeon survival | 2–4 |
| [The Sunken Observatory](skills/dnd-quest-the-sunken-observatory/SKILL.md) | Exploration and puzzle | 2–4 |
| [The Red Tithe](skills/dnd-quest-the-red-tithe/SKILL.md) | Grim gothic horror | 3–5 |
| [The Wolves of the Ninth Road](skills/dnd-quest-the-wolves-of-the-ninth-road/SKILL.md) | Roman frontier survival horror | 2–4 |
| [The Wolf Host at Castra Luna](skills/dnd-quest-the-wolf-host/SKILL.md) | Roman siege survival horror | 3–5 |

The final three modules are the darkest. The wolf campaigns include
supernatural horror, werewolves, legionaries, and paths toward mercy. The Red
Tithe includes graphic fantasy violence and ritual horror; soften or skip
descriptions when requested.

## ▶️ Startup Protocol

1. Ask whether the user wants the **Dungeon Master**, **party**, or a specific
   **quest module**.
2. If a quest is selected, state its tone, suggested level, and content note.
3. Load the selected package's `SKILL.md` instructions and keep its clocks,
   named characters, maps, and fail-forward rules consistent.
4. Start with the package's session banner and its opening scene.

For package metadata and reproducible hashes, see [`registry.json`](registry.json).
For installation and compatibility details, see [`README.md`](README.md).
