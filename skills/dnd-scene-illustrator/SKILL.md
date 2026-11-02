---
name: dnd-scene-illustrator
description: An unofficial, prompt-based scene illustration and visual reward skill for tabletop roleplay campaigns. Renders atmospheric scene art, generates optimized image prompts for image generators, and creates ASCII landscape vignettes upon reaching campaign milestones or player command.
license: MIT
compatibility: Compatible with all AI agents (Claude Code, Cursor, Windsurf, Antigravity, Copilot CLI, Hermes, ChatGPT).
metadata:
  author: c4da
  version: "1.0.0"
  categories: ["fun", "game", "dnd", "art", "illustration", "tabletop"]
  tags: ["ai-skills", "agent-skills", "skill-md", "tabletop-ai", "dnd", "rpg", "scene-art", "illustration", "visual-rewards", "prompt-based"]
---

# 🎨 D&D Scene Illustrator & Visual Rewards (`dnd-scene-illustrator`)

> *"The wizard's hands still tremble with electric charge as the giant stone idol crashes into the flooded chasm. Light filters through cracks in the vaulted ceiling, catching the swirling dust and the glittering gold coins scattered across the altar steps. In that breathless silence, you realize you have survived."*  
> &mdash; Field Chronicler & Court Cartographer

This is an unofficial, fan-made roleplay enhancement skill. It adds **visual reward milestones** and **on-demand scene illustrations** to any tabletop roleplaying campaign, whether running solo with a Dungeon Master or accompanied by an autonomous party.

---

## 🏆 The Visual Reward Philosophy

In tabletop roleplaying, the greatest moments deserve more than brief text—they deserve to be commemorated visually. This skill rewards players when they conquer critical milestones by presenting vivid scene depictions.

### Milestone Reward Triggers

Whenever the campaign reaches a dramatic turning point, the agent proactively offers a **Visual Reward**:

| Milestone | Context | Trigger Example |
|---|---|---|
| 👑 **Boss Fall** | A climactic nemesis or dungeon boss is defeated | *"Kragthor collapses upon the shattered flagstones!"* |
| 🌅 **Epic Vista** | Arriving at a legendary ruin, cavern, or panorama | *"You step out onto the rain-lashed ledge of Compass Ridge."* |
| 🎲 **Critical Feat (Nat 20)** | An extraordinary maneuver, spell save, or skill check | *"A Natural 20! Your arrow severs the rope holding the portcullis!"* |
| 🔥 **Campfire Haven** | Taking a long rest after surviving a grueling ordeal | *"You light a small fire beneath the sheltering boughs of the pine."* |
| 💎 **Vault Unsealed** | Discovering an ancient relic, tomb, or hidden treasure | *"The heavy sarcophagus lid grates back to reveal the Sun-Stone."* |

When a milestone is reached, the agent appends a reward prompt:
```text
⚔️ [VISUAL REWARD UNLOCKED]
Would you like to illustrate this moment? Type `/render` or "Show me the scene".
```

---

## ⚡ On-Demand Commands

Players can command a visual representation at any time during play:

- `/render` or `/illustrate`: Illustrate the current chamber, wilderness vista, or environment.
- `/render boss` or `/illustrate enemy`: Focus the artwork on the current enemy, monster, or boss.
- `/render party`: Render a group portrait of the adventuring party in their current condition and marching order.
- `/render action`: Capture the dramatic peak of the current turn's combat action.
- `/style <classic|gothic|matte|pixel>`: Switch the preferred rendering style.

---

## 🛠️ Multi-Environment Adaptation

Different AI environments offer different visual capabilities. This skill automatically adapts to the host:

### 1. Environments with Native Image Generation Tools (e.g. Antigravity, ChatGPT/DALL-E)

When the host agent has access to an image generation tool (such as an `image-generator` subagent, DALL-E, or an MCP image tool):
1. Construct an optimized high-detail prompt incorporating lighting, focal length, color grading, and texture details.
2. Invoke the image generation tool directly.
3. Save the image to the local conversation artifact directory.
4. Render the clickable image markdown preview directly in the response:
   ```markdown
   ![Scene: The Sunken Star Dome](artifact://path/to/image.png)
   ```

### 2. Terminal & Text-Only Environments (Claude Code, Copilot CLI, Cursor, Windsurf, Hermes)

When operating in text-only CLI mode without native image generation tools, deliver a complete **Three-Part Visual Reward Card**:

```text
================================================================================
  🖼️ SCENE ILLUSTRATION: THE FALL OF KRAGTHOR AT THE SUN-STONE ALTAR
================================================================================
       /\                                                        /\
      /  \       [ . . . . . . . ( CRACKED VAULT ) . . . . . . ]/  \
     /    \====================================================/    \
     |  | |               .   *   .    *    .   *              | |  |
     |  | |   /\             _____/\_____             /\       | |  |
     |  | |  /  \           /   SUN-STONE\           /  \      | |  |
     |  | | / /\ \         (   [GLOWING]  )         / /\ \     | |  |
     |  | |/ /__\ \       /================\       / /__\ \    | |  |
     |  | / /====\ \     /   ___    ___     \     / /====\ \   | |  |
     |  |/ /======\ \   /   /---\  /---\     \   / /======\ \  | |  |
     |  |============| /   |     ||     |     \ |============| | |
     |               |==========================|              | |
     |       @                 X           @                   | |
     |   [Valerius]         [KRAGTHOR]   [Ignis]               | |
     ============================================================
```

#### 1. Sensory Vignette
*A rich 2-3 sentence atmospheric snapshot capturing light, shadows, temperature, audio echoes, and character postures.*

#### 2. Copy-Paste AI Image Generator Prompt
A production-grade prompt ready for Midjourney, Stable Diffusion, DALL-E 3, or Imagen:
```text
Prompt: Dark high-fantasy oil painting, volumetric torchlight cutting through ancient subterranean mist, a defeated bugbear chieftain slumped beside a crumbling basalt altar, glowing amber sun relic pulsating with golden light, cracked flagstones, dust motes, rim lighting, 8k resolution, cinematic composition, painterly brushstrokes --ar 16:9 --style raw
```

#### 3. Framing Legend & Details
Key elements depicted:
- **Focus**: The fallen chieftain and the pulsing altar relic.
- **Lighting**: Warm golden radiance contrasting cold damp cavern blues.
- **Party State**: Valerius leaning on his greatshield; Ignis dusting his robes.

---

## 🎨 Artistic Styles

The illustrator supports four signature tabletop art aesthetics:

1. **`classic` (TSR 1980s Ink & Parchment)**:
   - Crisp black pen-and-ink cross-hatching, stippled shading, vintage rulebook manual aesthetic. Evokes Erol Otus, Larry Elmore, and David C. Sutherland.
2. **`gothic` (Dark Fantasy Oil)**:
   - Deep chiaroscuro, torchlight flickering on rusted mail and wet granite, heavy shadows, visceral tension. Evokes Karl Kopinski, Adrian Smith, and *Darkest Dungeon*.
3. **`matte` (Cinematic Modern High-Fantasy)**:
   - Widescreen 16:9 digital matte painting, volumetric atmospheric haze, radiant magical glows, rich saturated color palettes.
4. **`pixel` (Retro Roguelike ANSI / ASCII)**:
   - Terminal-native multi-block ASCII art with borders, glyph legends, and tactical depth.

For complete prompt formulas and camera directives, see [`references/art-styles.md`](references/art-styles.md).

---

## 🔗 Campaign Integration

This skill functions as a companion to the core roleplay engines:
- Works with [`classic-dnd-dungeon-master`](../classic-dnd-dungeon-master/SKILL.md) to illustrate chambers and boss rooms.
- Works with [`dnd-party-of-agents`](../dnd-party-of-agents/SKILL.md) to render character interactions, marching orders, and campfire resting scenes.
- Includes pre-built visual templates for all official adventure modules in [`references/scene-templates.md`](references/scene-templates.md).
