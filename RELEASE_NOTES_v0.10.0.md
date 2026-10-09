# USE YOUR FRIENDS v0.10.0 — Foundations and better throws

This is a foundations update, **not the new story campaign or generated mode yet**. Existing courses, AI friends and split-screen remain available.

## New throw options

While carrying a friend:
- Tap Grab/Throw for the familiar forward throw.
- Hold Grab/Throw for at least **0.3 seconds**, then release, to **lob** them higher with less forward speed.
- Carried planks are still placed as bridges.

Thrown friends retain momentum when they release the stick and can steer in the air. Real knockbacks remain harder to steer. A fresh launch no longer inherits the short-hop state of an earlier jump.

A carried player can escape with **one Jump press** after a short 0.25-second grab grace period, rather than mashing repeatedly. Classic catapults retain their existing tuned trajectories.

## Campaign groundwork

- New courses can use stable keys and sparse network IDs without being added to the old Classic level enum.
- Lobby selection, metadata, chapter successors, rewards and saves use registered definitions. Existing Classic saves keep their original keys and unlock behavior.
- Clearing the Classic campaign cannot accidentally unlock every future chapter.
- The game manager is split into smaller, responsibility-focused files.
- Measured throw, jump, Boing and plank ranges are packaged for future level-design checks. Existing levels are not automatically reshaped around one measurement sample.
- The latest completed run keeps at most 256 local gameplay events for future story features. It contains no microphone audio, network addresses or player names.

## Verification

The candidate passed 22 native throw/range/event checks, 12 native chapter-identity checks, 19 campaign checks, 54 AI checks, five split-screen checks, both classic co-op room tests at simulated 10% packet loss, and synthetic voice transport checks. Pure tests cover 28 progression cases and eight registry scenarios.

An earlier M1 candidate passed the 190-check integrated suite. Later targeted changes were verified separately; this is not a claim that the entire integrated suite was rerun after every change or that human playtesting is complete.

Host-authoritative physics is retained. Clock-driven client hazards and latency rewind from the initial roadmap are deferred, not silently claimed as implemented. The next campaign milestone remains a playable chapter prototype with real-player feedback before expanding the full story.
