# v0.13.0 — Night Shift prototype (playtest advisory)

**Correction:** The original notes overstated this update. Night Shift is a prototype course and contract-data experiment, **not** a completed procedural extraction mode. We are correcting this public description while building the playable mode.

What the v0.13.0 executable actually contains:
- A selectable Night Shift course with a van prop, fixed facility geometry, a crusher, crates and an extraction pad.
- A separate seeded contract/layout *data* generator. The runtime course currently uses a hardcoded seed and does not build its geometry from the generated layout.
- Standalone Taster/Sweeper decision-state classes. They are **not spawned as hunting threats** in the runtime course.
- `Gulpable` crate methods. Player input is not yet wired to swallow/spit these objects.

**Known gameplay blockers:** the extraction pad is beside the spawn and the standard finish logic does not require quota/cargo; a party can finish without doing a contract. Investigate/Rescue objectives, catch effects, threat behaviors and bot-certified seeds are not implemented in the runtime game. A simple lock-mask check is **not** stateful BFS or a 100% solvability proof. Do not rely on v0.13.0 as the promised generated mode.

The prior 12 native checks verified registration/build, props, and direct test calls to swallow/spit; the 16 pure checks verified data/state helpers. Neither verified a continuous normal-input contract playthrough. Existing Classic modes remain in the build. This is a free Windows playtest, not a finished campaign/generated-mode release.
