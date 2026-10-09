# USE YOUR FRIENDS v0.11.0 — Clearer cues and fair releases

This update adds clear visual onboarding cues to Gloop Gauntlet, fixes split-screen camera layout bugs, and introduces the fair loaded-tool release system to protect friends from accidental drops.

## Clearer cues before hazards
- **Caramel U-notches** embedded on the starter island clearly mark where a Plank bridge belongs before you reach the gap.
- **Pink scalloped candy rings** on the lower island deck mark the launch pad area before the tall cliff.
- **Purpose sign:** a high-visibility sign clearly marks "REMELT OVERFLOW / KEEP MOVING" near the rising goo, engineered to stay visible and un-clipped across both shared and split-screen camera modes.
- Visual cues use custom mesh geometry and materials without adding colliders or perturbing physics snapshot orders.

## Fair loaded-tool release
- **Accident protection:** When a friend is actively riding your Plank or Boing form, a quick button tap no longer drops them into the goo. Reverting or switching tools while carrying a rider now requires a deliberate **0.5-second hold**.
- **Unladen tools stay snappy:** If no friend is standing on you, morphing back to blob form remains instant.
- **1.0-second OOPS grace:** When voluntarily dropping a friend while carrying them, an accusation is held pending for 1 second. The carrier can press OOPS to immediately dismiss the accusation as an accident.
- Accidental drops (running out of jelly, entering sour zones, or being killed) are classified as accidents and never trigger betrayal replays or traitor counters.
- **On-screen accessible release:** Dedicated on-screen controls allow keyboard and controller players to arm, confirm, or cancel releases without complex gamepad chord combinations.

## Split-screen and controller fixes
- Three-player split-screen now tiles cleanly with two upper viewports and a full-width lower viewport, eliminating blank quadrants.
- Prevented a bug where holding the join button on a single physical controller could spawn duplicate players.
- Input protocol updated to v2 with explicit held-form masks and lease expiration, ensuring dropped network packets cannot lock players in a held state.

## Verification
- 37 native Readability checks verified across shared and split camera viewports with real controller input from spawn.
- 15 native FairRelease checks verified in-engine covering unladen reverts, rider detection, hold gating, OOPS cancellation, and betrayal commits.
- 33 pure fair-release policy unit tests and 29 wire codec tests pass.
- Full regression suites (AI, Progression, Split, Social, Feel) and 2-process UDP network tests on both co-op maps verified.
