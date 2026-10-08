# v0.8.0 — Earn your tools. Hear your friends. Keep the receipts.

## A campaign that rewards playing

- Start with **Plank + Boing**. Clear **Gloop Gauntlet → Ball**, **Taffy Factory → Sticky**, **Sky Bakery → Balloon**.
- Campaign completions unlock the next course; finishing Pinball Palace unlocks both advanced co-op courses, Sour Science Lab and Twin Tracks.
- Real level finishes now grant permanent rewards and show a visible celebration in Results, including multiple hats earned at once. A Continue button takes you back to the lobby.
- The lobby shows earned, borrowed and locked tools plus the Halo / Golden Crown requirements. Halo: escape any level. Golden Crown: earn a gold time on any level.
- Gloop's candy switch and normal-blob target let a fresh team finish before earning Ball. Existing save progress is retained.
- Friends joining a veteran online host borrow the session's available tools without gaining permanent unlocks just by joining. Participating in a completed run earns their own rewards.
- Empty or undersized teams cannot claim a finish after players leave.

## Opt-in proximity voice

Enable **PROXIMITY VOICE** in Settings; hold **T** or **L3** to talk. Separate microphone and incoming-voice mute controls are available.

Voices fade with avatar distance and sound muffled in Ball form. Releasing push-to-talk, losing focus, opening Settings, pausing or leaving the session stops microphone capture. Live voice is not stored in replays, logs or captures.

## Automatic betrayal capture

Enable **AUTO BETRAYAL CLIPS** in Settings. The game captures **five seconds after** a betrayal, with the logo overlay, no preview, a 30-second cooldown and bounded storage. It does not continuously record or include pre-event footage.

Manual F10 recording is protected; F10 during an automatic clip takes over as a manual recording. Automatic frames use compressed JPEGs; manual frames remain PNGs.

**Captures are silent.** MP4 export requires an optional external ffmpeg executable on PATH or at `tools/ffmpeg.exe` beside the game. No encoder is bundled or silently downloaded. Without one, the game clearly reports image-sequence output. Low-FPS export remains best effort.

## Online co-op and update fixes

- Plate occupancy, scale metadata and catapult-arm animation now travel with host snapshots.
- Online doors, bridges, lifts and catapults no longer overwrite host positions with client-side simulation.
- Client results use the current snapshot's time and stats before granting personal rewards.
- Installer and portable packages come from the same staged candidate. Packaging checks the baked version, installer hash, install/update/uninstall results, and only stops its own test processes.

## Playtest limits

Room-code connectivity depends on both routers and ISPs; strict networks may need Tailscale or the same Wi-Fi. Everyone in a room must use the same game version.

Voice is **unencrypted UDP**: use trusted rooms. Automated two-process checks use one PC; real microphones, voice quality, separate-home connections and human fun/difficulty still need playtesting. These checks are not a guarantee of compatibility on every machine.
