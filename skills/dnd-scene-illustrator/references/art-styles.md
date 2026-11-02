# 🎨 Tabletop Scene Art Styles & Prompt Engineering

This reference guide provides prompt formulas, camera lenses, lighting setups, and negative prompts for each supported artistic style.

---

## 📜 1. Classic 1980s TSR Ink & Parchment (`classic`)

Evokes vintage 1st and 2nd edition rulebooks, boxed sets, and module covers (Erol Otus, Larry Elmore, David A. Trampier, Clyde Caldwell).

### Style Formula
```text
Vintage 1980s tabletop fantasy manual illustration, detailed pen and ink drawing on aged yellowed parchment, clean cross-hatching, stippling shadow gradients, dramatic hatching lines, hand-inked fantasy roleplay guidebook plate, high contrast black ink, archival aesthetic, no digital color
```

### Camera & Lighting
- **Composition**: Eye-level or slight worm's-eye view, strong foreground silhouettes.
- **Lighting**: Single harsh light source (torch or lantern), sharp ink shadows, heavy cross-hatching in corners.
- **Negative Prompt**: `photorealistic, digital painting, smooth airbrush, 3D render, vibrant neon, blurry, watermark`

---

## 🕯️ 2. Dark Gothic Oil Painting (`gothic`)

Evokes grim dark-fantasy classics, grimdark tabletop art, and gothic horror (Adrian Smith, Karl Kopinski, Frank Frazetta, *Darkest Dungeon*).

### Style Formula
```text
Dark gothic fantasy oil painting, thick impasto brushstrokes, deep chiaroscuro lighting, harsh flickering torchlight contrasting pitch-black subterranean shadows, heavy grime, rusted iron and damp stone textures, visceral tension, muted earthen palette with rich crimson and amber highlights, masterwork canvas
```

### Camera & Lighting
- **Composition**: Dutch angle or tight claustrophobic framing, low three-point lighting.
- **Lighting**: Embers, tallow candles, dying torches, casting long jagged silhouettes across wet flags.
- **Negative Prompt**: `bright pastel, cartoon, anime, low contrast, washed out, plastic skin, clean modern`

---

## 🌟 3. Cinematic High-Fantasy Matte Painting (`matte`)

Evokes modern flagship RPG concept art, ArtStation trending keyframes, and wide-format rulebook splash art.

### Style Formula
```text
Cinematic 16:9 high-fantasy digital matte painting, epic scale landscape, volumetric atmospheric god rays, glowing arcane particles floating in cool misty air, richly textured medieval architecture, photorealistic depth of field, 8k resolution, ArtStation trending, key art illustration
```

### Camera & Lighting
- **Composition**: Wide panoramic 16:9, rule of thirds, deep focal depth showing foreground, midground, and cavernous background.
- **Lighting**: Dual-temperature lighting (warm golden magic vs. cold obsidian blue stone), volumetric dust motes.
- **Negative Prompt**: `deformed, oversaturated flat colors, jpeg artifacts, poorly drawn anatomy, text overlay`

---

## 📟 4. Retro ANSI / ASCII Terminal Landscape (`pixel`)

Designed specifically for monospace terminal displays, combining ASCII typography, box-drawing runes, and shaded density blocks.

### Construction Principles
- **Width**: 60–76 characters wide (fits clean terminal windows without wrapping).
- **Depth Layers**:
  - Sky/Ceiling: `.` `*` `'` for cavern roofs, stars, or hanging stalactites.
  - Midground: `/ \` `| |` `[ ]` for pillars, arches, altars, and boss figures.
  - Foreground: `=` `-` `_` for steps, floors, and party markers (`@`, `P`, `B`, `R`, `W`).
- **Framing**: Clean double-line or hash borders (`#`, `║`, `═`) with a centered title placard.


---

## 🐺 5. Roman Frontier Horror & Dual-Tone Chiaroscuro (`frontier`)
*(The signature "Ninth Road" aesthetic featured on the official campaign cover)*

This style captures gritty, historical Roman military realism colliding with gothic lycanthropic horror on a frozen, unforgiving frontier.

### The Visual DNA
- **Setting**: High-altitude snowbound mountain passes, crumbling Roman border watchtowers, alpine pine forests, and isolated palisade outposts.
- **The Staging & Composition (Three-Tier Depth)**:
  - **Foreground**: Weary legionaries in detailed, battle-scarred iron *lorica segmentata*, Gallic/Montefortino helmets with brass cheek guards, dirt-stained woolen crimson cloaks, gripping *gladius* short swords, *pilum* javelins, and curved red *scutum* shields. A crimson *vexillum* standard flutters in the freezing gale.
  - **Midground**: Fortified bivouac with pointed wooden stakes, supply crates, and wolf paw tracks cutting through deep virgin snow.
  - **Upper Backdrop**: The silhouette of a massive bipedal werewolf perched menacingly on the precipice of a ruined Roman stone tower, dramatically framed against a huge, cratered full moon.
- **Tri-Light Color Harmony**:
  1. *Primary Foreground Light*: Crackling, intense amber-orange campfire casting vivid specular reflections off armor plates, weapon edges, and weathered faces.
  2. *Cold Ambient Moonlight*: Luminous silvery-white moonlight and deep midnight-indigo shadows bathing the snow, rocks, and the stalking werewolf.
  3. *Horizon Twilight*: A sliver of dying golden sunset glowing on the far distant valley horizon.

### Master Production Prompt
```text
Masterpiece cinematic fantasy illustration, gritty Roman frontier horror, snowbound mountain outpost at twilight, legionaries in battered iron lorica segmentata and dirt-stained crimson cloaks clutching gladius swords and red scutum shields behind a timber barricade, gathered around a crackling warm campfire, high above on a crumbling stone watchtower crag stands a massive terrifying bipedal werewolf silhouetted against a luminous cratered full moon, deep midnight indigo snow slopes, wolf paw tracks in deep drifts, dying golden sunset on the far distant mountain horizon, dual-temperature lighting with intense warm orange firelight and cold silvery moonlight, rich painterly brushwork, atmospheric mist, embers and frost, ultra-detailed textures, 8k resolution, cinematic widescreen composition, ArtStation key art --ar 16:9 --style raw
```

### Camera & Atmosphere
- **Lens & Angle**: Low-angle 35mm cinematic anamorphic perspective, looking slightly upward from the camp toward the towering rock crag and ruined watchtower.
- **Atmosphere**: Drifting snow particles, rising smoke and glowing embers, heavy frost clinging to iron and timber, visceral dread mixed with Roman military discipline.
- **Negative Prompt**: `modern gear, clean polished parade armor, sunny daylight, flat ambient lighting, cartoon, 3d render, anime, oversaturated neon, extra limbs, deformed fingers, low resolution, blurry, watermark`
