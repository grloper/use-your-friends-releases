# USE YOUR FRIENDS v0.13.0 — Night Shift Procedural Mode

This release introduces **NIGHT SHIFT**, the infinitely replayable procedural facility mode featuring contracts, randomized threats, and extraction gameplay.

## Night Shift Mode
- **Procedural facility generation:** Every shift generates a unique facility layout from seed using modular Van, Spine, Hub, and Vault chambers.
- **Contract cards:** Each shift generates a contract with specific Objectives (Rescue, Haul, Investigate Mimic), randomized Catches (Double Throws, Low Gravity syrup, Slippery butter floors), and Quotas.
- **Threat AI:**
  - **The Taster:** Hunts morphing blobs; startled and frozen for 2 seconds whenever any blob squelch-morphs!
  - **The Sweeper:** Vacuums still cargo and downed blobs, but completely ignores actively carried friends.
- **The Van & Extraction:** Start at the Escape Van, traverse the hazardous facility to haul cargo crates or rescue friends, and extract back to the Van before the Dawn Bell!
- **Stateful BFS solvability:** Every generated layout is mathematically verified by a breadth-first search across all lock requirements to guarantee 100% solvability with the player's available toolkit.

## Verification
- 12 native in-engine Night Shift checks pass (level generation, Escape Van, extraction pad, cargo crate spawning, swallowing crates, spitting).
- 16 pure unit tests covering contract seed determinism, BFS solvability, and threat AI state machines pass.
- All 13 Chapter 1 checks, 37 Readability checks, 15 FairRelease checks, and full regression suites pass.
