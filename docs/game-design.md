# Town Escape — Game Design Pitch

## One-line pitch

A 2–4 player co-op survival game where a crew must cross a hostile town and escape while its AI population investigates, searches, and hunts them.

## Player fantasy

“We’re outnumbered, underprepared, and being watched. If we work together and stay clever, we might make it out.”

The players should feel hunted, resourceful, and responsible for one another. The AI is dangerous because the town reacts as a system, not because every enemy is a perfect fighter.

## Setting

A fictional small town under emergency lockdown. The crew begins in a safehouse near the edge of town. Their route to freedom crosses residential blocks, a commercial strip, and a final checkpoint or extraction zone.

Keep the setting grounded and eerie rather than graphic. The threat comes from uncertainty, pursuit, and dwindling time.

## Round structure

1. **Plan:** choose a starting route and a small kit.
2. **Search:** enter buildings to find supplies and clues.
3. **Complete an objective:** restore power, find a gate key, or contact an extraction point.
4. **Evade:** break line of sight, hide, create a distraction, or take a longer route.
5. **Extract:** reach the exit together, or decide whether to risk going back for a separated teammate.

A round should be short enough to replay and have more than one viable route.

## Cooperative roles

Avoid fixed classes at first. Let players specialize through equipment and moment-to-moment choices:

- **Scout:** spots patrols and marks safe routes.
- **Fixer:** opens locked doors and repairs equipment.
- **Medic:** stabilizes and revives teammates.
- **Decoy:** draws attention or creates noise away from the crew.

A player should still be useful when carrying no special item.

## AI threat model

The town’s response escalates through readable stages:

1. **Routine:** patrols follow routes; locals occupy homes and shops.
2. **Suspicion:** an unusual sound or missing item sends nearby AI to investigate.
3. **Search:** a sighting or repeated disturbance triggers a wider sweep.
4. **Hunt:** confirmed player locations bring pursuers and cut off common routes.

AI should communicate its state through footsteps, radios, lights, shouts, and changing patrol patterns. Players need a chance to understand why danger is rising.

### Initial AI behaviors

- Patrol between authored points.
- Hear loud events within a radius and investigate the source.
- Spot players based on distance, lighting, and line of sight.
- Chase a visible player, then search the last known location.
- Share sightings with nearby allies after a short delay.
- Return to routine if the crew stays hidden and creates no new evidence.

For the first prototype, these behaviors can be simplified to a single patrol type and one escalation meter.

## Key systems

- **Noise:** movement, broken objects, doors, and tools create different sound levels.
- **Visibility:** darkness and cover help, but do not make players invisible.
- **Evidence:** repeated disturbances raise the town’s alert level and alter routes.
- **Scarcity:** limited healing and utility items make sharing meaningful.
- **Downed state:** teammates can revive a player, but doing so costs time and creates risk.
- **Separation:** the group can split up, but distance makes communication and rescue harder.

## First playable milestone

Build the smallest complete experience:

- 2–4 connected players on one compact neighborhood map
- One shared objective and one extraction point
- Basic movement, interaction, and a tiny inventory
- One patrol AI with investigate, chase, and search states
- A simple alert meter that rises from noise and sightings
- Downed/revive interaction
- Win, loss, and round restart

Do not start with a huge town, many enemy classes, crafting trees, or a progression system. First prove that players enjoy coordinating while being hunted.

## Open decisions

- Engine and target platforms
- Online networking approach and host model
- Visual direction and camera style
- Whether rounds are session-based or part of a longer campaign
- How much information the AI shares across the town
- The exact tone and intended age rating

## Early success questions

- Does the team have meaningful choices when a route becomes unsafe?
- Can players tell what caused the town to react?
- Is rescuing a teammate tense without making a downed player wait too long?
- Do repeated runs produce different stories from the same compact map?
