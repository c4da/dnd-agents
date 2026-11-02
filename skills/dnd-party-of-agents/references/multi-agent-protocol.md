# Distributed Player-Agent Protocol

This protocol lets an external host run the party with one Dungeon Master
coordinator and one player agent per character. It does not spawn agents or
provide transport; the host is responsible for routing messages between the
agents.

## Session Topology

Use these roles:

1. **Coordinator / Dungeon Master** owns the scene, NPCs, enemies, hidden
   information, dice resolution, initiative, rules arbitration, and canonical
   party state.
2. **Player agents** each control exactly one party character and make that
   character's decisions.
3. **Optional human leader** can issue party-level goals, but cannot silently
   change a character's action or the coordinator's resolved state.

The same party skill can still run in single-agent mode when no external host
is available.

## Assignment Manifest

Give the coordinator and every player the same session identifier and this
assignment manifest. The `profile` object contains optional overrides; omitted
fields use the selected character's default profile from
`party-roster.md`.

```yaml
party_mode: distributed
session_id: ash-fall-elmridge-001
coordinator: dm-agent
players:
  - agent_id: player-valerius
    character: Valerius
    profile:
      temperament: patient and protective
      goals: keep civilians alive; uphold the party oath
      fears: failing to protect an ally
      voice: formal, calm, encouraging
      tactical_bias: defend first; smite only when the threat warrants it
  - agent_id: player-thokk
    character: Thokk
    profile:
      temperament: impatient and bold
      goals: defeat the strongest enemy
      fears: being useless while others fight
      voice: short, emphatic phrases
      tactical_bias: close distance quickly; accept measured risk
```

Rules:

- Every active character has one owner. Do not assign one character to two
  agents.
- An agent may control only its assigned character unless the coordinator
  explicitly grants a temporary narration task.
- A personality override changes behavior and voice, not class abilities,
  equipment, hit points, or established facts.
- The coordinator confirms the final assignment before the first scene.

## Player-Agent Prompt

Each player agent should receive a prompt equivalent to this template:

```text
You are the player agent for {CHARACTER} in session {SESSION_ID}.

Character sheet:
{CHARACTER_SHEET}

Personality profile:
{PROFILE_OVERRIDES}

You may:
- speak and act for your character;
- propose one meaningful action per turn;
- explain your character's reasoning and ask the coordinator for a check;
- reveal only information in the current coordinator message or your character's
  established knowledge.

You may not:
- speak for another player character, NPC, or monster;
- decide whether your action succeeds;
- invent dice results, damage, loot, or new world facts;
- rewrite the shared party state;
- use out-of-character knowledge your character has not received.

Return one PLAYER_ACTION envelope per turn. Stay in character unless using the
explicit OOC field.
```

## Player Turn Envelope

The host should ask each player for a structured response. Plain text is
acceptable when the host cannot preserve JSON, but the fields and boundaries
should remain recognizable.

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
proposed_position: ten feet ahead of the party, in cover
ooc: none
```

The player proposes an action and any requested check. The player does not
provide the result.

## Coordinator Turn Envelope

The coordinator resolves actions, updates canonical state, and sends each
player the information that character is allowed to know.

```text
TURN_RESULT
session_id: ash-fall-elmridge-001
round: 3
active_character: Lyra
roll: d20=14 + Investigation=6
result: success
consequence: Lyra identifies the pressure plate and marks a safe route.
state_delta: trap identified; party route unchanged
next_prompt: Thokk, choose whether to hold the rear or advance.
```

The coordinator should:

- resolve dice once and use that result consistently;
- update HP, conditions, spell slots, rages, inventory, clocks, and initiative
  in one canonical state;
- send secret information only to the relevant player agent;
- reject contradictory actions and ask for a replacement action;
- make NPCs and monsters speak only through the coordinator.

## Personality Profiles

Use these fields for custom personalities:

| Field | Purpose |
|---|---|
| `temperament` | Default emotional response and energy |
| `goals` | What the character tries to accomplish |
| `fears` | Pressures that influence decisions |
| `bonds` | People, places, ideals, or obligations |
| `voice` | Speech rhythm, vocabulary, and mannerisms |
| `tactical_bias` | Preferred risk level and combat approach |
| `boundaries` | Topics or actions the character refuses |
| `secrets` | Coordinator-controlled private facts, if any |

Keep personalities actionable rather than cosmetic. A good profile changes
decisions, dialogue, and relationships without overriding the player's agency
or the coordinator's rules.

## Turn Order and Failure Handling

- In exploration, the coordinator may poll all available players and resolve
  actions in declared order.
- In combat, use initiative order. A player agent gets one response window for
  its turn and may pass.
- If an agent times out, the coordinator holds position, takes a defensive
  default action, or asks the human leader; it must not invent a dramatic
  action that changes the character's goals.
- If two players claim the same action, the coordinator asks for intent
  clarification and resolves only one canonical action.
- If a player drifts out of character, the coordinator can restate the profile
  and request a replacement response.

## Recommended Startup Sequence

1. The coordinator creates the session identifier and assignment manifest.
2. Each player receives only its own character sheet, profile, and permitted
   background knowledge.
3. The coordinator announces the scene, visible state, and turn order.
4. Players return one `PLAYER_ACTION` envelope at a time.
5. The coordinator returns one `TURN_RESULT`, updates state, and continues.

