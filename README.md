# HUSH — The Town Remembers

A co-op stealth-survival game about a town that hunts the crew by remembering where they have been.

The town is a **distributed memory system**. Noise, sprinting, and sightings leave echoes that patrols can follow after the crew has moved on. Players can exploit that rule by planting a false memory and sending the hunt down the wrong street.

## Play the prototype

Open `index.html` in a browser, or serve the repository locally:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

### Local co-op controls

- **Mara:** WASD to move, Left Shift to sprint, Q to plant a false echo
- **Sol:** Arrow keys to move, Right Shift to sprint, / to plant a false echo

Find three route cassettes, then get both players to the extraction beacon before the 2:30 siren. The crew shares three recovery signals. Sprinting travels faster but leaves louder echoes; false echoes can pull the patrols away from your real route.

## Visual direction

A hand-rendered isometric night district in oxidized teal, signal-chartreuse, and warning amber. Fog, radio-noise scanlines, lit windows, and phosphor-like memory traces make the town feel like a surveillance instrument instead of a generic zombie arena.

## What makes HUSH different

- **Enemies hunt remembered actions:** patrols pursue decaying sound memories, not just the players' current position.
- **Misdirection is a core verb:** a false echo lets the crew rewrite the AI's short-term story.
- **The world shows its attention:** the memory meter, patrol states, and glowing echo traces communicate what the town knows.
- **Co-op is about managing evidence:** a sprint can save a teammate now while making the whole team easier to find later.

## Current slice

The browser prototype contains a compact isometric district, two-player same-keyboard movement, three patrols, echo investigation, false-memory decoys, route cassettes, extraction, and a shared recovery budget.

This is **local co-op only** so far. Online matchmaking, real networked co-op, authored interior levels, and production 3D art are future work. The art direction is established in code; production-quality 3D assets are not in this first slice.

## Project notes

See [the game design pitch](docs/game-design.md) for the wider game, systems, and next milestone.
