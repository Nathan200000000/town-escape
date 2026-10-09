# HUSH — The Town Remembers

## One-line pitch

A tense co-op stealth-survival game where an entire town hunts the crew by remembering their actions—and the crew can plant false memories to rewrite the pursuit.

## The signature idea: a town with a memory

The town does not have one all-seeing monster. It has a **Civic Memory**: a distributed intelligence made from neighborhood cameras, radios, streetlights, alarms, domestic devices, and the people who pass information along.

It does not know exactly where the crew is. It knows where the crew made noise, what was disturbed, and where it last saw them. Every action becomes evidence, then rumor, then a patrol route.

Players can exploit that delay. A thrown radio, false alarm, or deliberately staged trail can make the town remember the wrong thing. The central question is not “Can we fight all the enemies?” It is “What story does the town believe about us right now?”

## Player fantasy

“We are ghosts in a town that keeps a record. We can survive by staying quiet, helping each other, and making the town believe a convincing lie.”

Players feel hunted and resourceful. Their strongest tool is coordination, not firepower.

## Visual identity

- **Camera:** readable isometric view, with carefully framed streets and rooftops.
- **Palette:** ink navy, oxidized teal, phosphor chartreuse, and warning amber.
- **Materials:** wet asphalt, aged plaster, dusty windows, radio static, and paper-thin fog.
- **Memory traces:** luminous, topographic sound rings and ghosted silhouettes that fade as the town forgets.
- **Threat communication:** windows blink when a signal is relayed; patrols turn their radio antenna toward remembered evidence; the siren changes the whole district’s light and sound.
- **Mood:** surveillance noir and strange civic ritual, not a generic zombie apocalypse.

The current browser slice explores this direction with procedural canvas art. It establishes the composition and palette; production 3D models, animation, lighting, and sound design are later work.

## Core round

1. **Slip out:** begin with a small kit and choose a route across a locked district.
2. **Recover route cassettes:** each cassette contains a piece of an obsolete evacuation route.
3. **Manage the town’s memory:** hide evidence, wait for echoes to decay, or plant a false one to draw patrols away.
4. **Keep the crew together:** share cover and supplies, rescue a caught teammate, and decide when to risk a sprint.
5. **Reach the extraction beacon:** both players must cross before the district-wide siren locks the route.

A round should be short and replayable, with several routes through a compact map.

## The memory hunt

The Civic Memory should follow legible stages:

1. **Routine:** patrols move through their district and report ordinary conditions.
2. **Echo:** sound, a missing object, or a sighting creates a trace with a location, strength, and age.
3. **Relay:** nearby devices and people pass the trace to one another after a delay.
4. **Search:** patrols converge on the strongest recent trace and inspect its neighborhood.
5. **Reconstruction:** repeated evidence narrows the likely route and closes convenient exits.
6. **Forgetting:** if no new evidence arrives, the trace decays and patrols gradually disperse.

A false echo is not invisibility. It gives the crew time by making the town investigate a believable alternative.

## Co-op verbs

- **Move quietly** and let old traces fade.
- **Sprint** to save time, at the cost of a louder and longer-lived memory.
- **Plant a false echo** to draw a patrol toward the wrong street.
- **Split up briefly** to search two sites, while increasing the risk of being isolated.
- **Recover a teammate** after a capture, spending a shared recovery signal.
- **Extract together**; nobody wins by leaving their partner behind.

Future equipment can add meaningful evidence choices: a cassette loop that replays a footstep, a dead relay that prevents a local signal from spreading, and a chalk mark that lets teammates read a route without using the radio.

## The playable slice

The browser prototype is a compact proof of the central loop:

- Two-player same-keyboard co-op
- Isometric night district and minimap
- Three roaming patrols with routine, memory, and witness states
- Recent sound traces that pull patrols toward the crew’s previous positions
- False-echo decoys
- Three route cassettes, a timed siren, extraction, and shared recovery signals

Controls: Mara uses WASD, Left Shift, and Q. Sol uses arrow keys, Right Shift, and /.

This is local co-op only. It is a gameplay and art-direction prototype, not the finished online game.

## Development path

### Next: make the slice deeper

- Add distinct patrol roles: listener, blocker, and relay runner.
- Show relayed evidence traveling between street devices.
- Add hiding spots, a noise-producing gate, and one route that can be opened in two ways.
- Improve player animation, building silhouettes, fog lighting, and spatial audio.
- Tune round difficulty so patrols feel clever but give fair warning.

### Then: choose the production platform

Select an engine and networking model based on the desired platform and visual target. Move the proven memory-hunt loop into a host-authoritative online co-op build before expanding the map.

### Later: make each district tell a story

Use authored neighborhoods, changing local rules, and multiple extraction paths. Let the town’s records reveal what happened during the evacuation without relying on long exposition.

## Design checks

- Can players explain why a patrol came to a location?
- Can they create a useful misdirection without making themselves untouchable?
- Does sprinting feel like a real trade rather than a free speed boost?
- Can a separated teammate be found and rescued?
- Does the town’s behavior make players tell different stories after each run?
