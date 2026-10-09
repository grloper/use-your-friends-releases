# v0.12.0 — INTAKE prototype (playtest advisory)

**Correction:** The original notes called this a completed story chapter. It is an unfinished greybox prototype and cannot yet be described as a playable chapter from start to finish.

What the v0.12.0 executable actually contains:
- A selectable INTAKE course with five named sections, platforms, walls, gaps, a sweeper, key/fuse/spanner props and an escape pad.
- A `Gulpable` item-state component and a pure Snap-Back position helper.

**Known gameplay blockers:** no player input invokes Gulp/Spit; the item-labelled hatch/gearbox use ordinary occupancy plates rather than checking those items; Snap-Back has no live tip-grip or rejoin interaction; there is an approximately 24m unbridged break between mixer decks. The scripted native fixture directly called item methods after teleporting a player and did **not** prove that ordinary players can traverse or finish the course.

The 13 native checks covered registration, object presence and direct method calls. The 13 pure checks covered item state and tip math. Neither established a continuous normal-start playthrough, cooperative solvability, narrative beats or human fun. Existing Classic modes remain available. Work to make INTAKE genuinely playable is ongoing.
