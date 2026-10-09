# USE YOUR FRIENDS v0.12.0 — Chapter 1: INTAKE

This milestone introduces the first full story campaign chapter, **CHAPTER 1: INTAKE**, featuring the new **GULP** verb and **Snap-Back** cooperative mechanics.

## Chapter 1: INTAKE (The Remelt Vats)
- **Setting:** The remelt vats where Batch 13 awakens. Warm gooey vats where a slip is a soothing bath, not an instant splat.
- **Stage 1 (Reject Bin):** A 2.2m tall caramel wall that cannot be jumped alone. Lob a teammate over to the raised gold ring to reach the key chamber.
- **New Verb: GULP:** Narrow bars enclose the hatch key. Blobs can squeeze through the bars, but held objects cannot. Walk into the hatch key to swallow it into your jelly belly! Swallowing keeps your hands free to morph into bridges and springs. Squeeze back through the bars and spit the key forward to unlock the door.
- **Stage 2 (Plank Walk):** A 5m gap over warm goo requiring a Plank bridge, followed by a 4.2m cliff requiring Boing.
- **Stage 3 (Vat Wall & Snap-Back):** A 5m gap over a deep vat with no ladder. Cross as a Plank, have your friend grip the tip, and snap the bridge holder across the gap with a rubbery Snap-Back! Transport the licorice fuse to power the gate.
- **Stage 4 (The Mixer):** A giant vat with a rotating 3-blade mixer. Reach the central hub and drop the spanner into the gearbox to stop the blades and open the exit chute.
- **Stage 5 (Exit Chute):** The whole team reaches the escape rocket pad to clear Chapter 1!

## New Mechanics & Components
- **`Gulpable`:** items (keys, fuses, spanners) that can be swallowed, stored in belly while morphing, and spat out with forward velocity.
- **`SnapBack`:** plank tip calculation, reach detection, and rubbery hinge override snapping.

## Verification
- 13 native Chapter 1 in-engine checks pass (level building, checkpoints, gulping, spitting, morphing while swallowing, mixer blades).
- 13 pure unit tests covering Gulpable item state and SnapBack mathematics pass.
- Full regression suite (Readability 37/37, FairRelease 15/15, AI 54/54, Progression 28/28, Input wire 29/29) passes.
