# USE YOUR FRIENDS v0.9.0 — Solo, but not alone

## Add AI friends

Join the lobby as a human, then choose **ADD AI FRIEND** to fill your group with up to three optional companions. AI occupies real party slots, uses normal physics and your earned/borrowed tools, and participates in the same co-op finish rules.

- **Follow:** move alongside you and gather inside the rocket area.
- **Hold Here:** walk onto your chosen pressure pad and stay while you cross.
- **Help:** find an accessible nearby linked plate or scale counterweight; respect colored Twin Tracks lanes.
- **Tools:** stay as Plank/Boing or another earned form where placed. You can carry and throw AI normally. Jelly and Sour restrictions still apply.
- Safe intent suspension during pause, replay, Settings, carrying and death. Ordinary checkpoint respawns; no AI teleporting, permanent unlock bypass or microphone identity.

## Controls

- Lobby: **I** adds an AI, **N** removes the last AI. Gamepad: **Y** adds; **LB + Y** removes. Mouse buttons are available too.
- **F1** selects the next AI. **F2** Follow, **F3** Hold Here, **F4** Help.
- **F5** Plank, **F6** Boing, **F7** Normal. Tool orders transform the AI where it currently stands.
- **F8** opens the orders panel. Gamepad: **Start** to pause, then **Y** for orders; D-pad + **A** select, **Y** cycles AI, **B** goes back.
- Locked tools remain locked; the panel exposes all earned forms. Join your human controller before adding AI.

## What this does not promise

These are **command-assisted companions, not autonomous all-course solvers**. They do not independently sequence every portal, catapult or maze, or guarantee automatic completion of all seven maps. Complex vertical routes still need human carrying, throwing, tool placement and orders. There is no cloud AI, API bill, generated conversation or simulated microphone.

## Verification

- 48 pure AI-policy assertions and 54 native AI checks cover party/UI limits, real locomotion, actual Lab pressure-plate holding/releasing, tool gates, pause/replay/carry/death, modal controls, minimum-team finish guards, and exact save restoration.
- 19 targeted campaign regression checks passed. The unchanged historical v0.8 integrated suite is documented separately, not claimed as a new full v0.9 run.
- Windows installer, self-update, uninstall and public download integrity are verified as release gates.

## Existing features and limits

Earned tools/rewards, seven courses, controller/fullscreen support, room-code co-op, opt-in proximity voice and automatic silent capture remain available. Captures save image sequences by default; MP4 requires an optional external FFmpeg encoder and no encoder is bundled. Voice transport is unencrypted: use trusted rooms and matching game versions. Real microphone quality, separate-home router connectivity and human fun/difficulty remain playtest work, not automated guarantees.

Windows 64-bit free playtest. If a friend cannot connect through their router, try a shared Tailscale network.
