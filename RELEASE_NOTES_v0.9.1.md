# USE YOUR FRIENDS v0.9.1 — AI friends that survive the level

Fixes found by watching AI friends play every course from the start with ordinary controls (no teleports): a pilot player plus three AI friends, recording every death, stall and stuck spot.

## AI fixes

- **No more permanent "Stuck".** AI friends retry automatically after a short cooldown or when you move, instead of freezing for the rest of the run.
- **Taffy presses:** AI times each press and only crosses when it stays up long enough and the gap beyond is free; it never idles underneath one. AI deaths in the Crush Zone dropped from 25 to about 3 per run.
- **Crumbly cookies:** AI waits until the whole cookie chain is intact and nobody is still crossing it, keeps moving on a shaking cookie, and hops on quickly.
- **Gusts:** AI takes shelter behind candy pillars or braces against the wind.
- **Zig-zag stepping stones:** AI searches left/right for the next landing pad instead of only straight ahead.

## Course fix

- **Pinball Palace:** the opening jump is now 2.2 m (was 3.2 m, at the very limit of a full-speed jump — even careful players often fell short).

## Still true

AI friends are command-assisted. They wait at gaps that need a plank and at co-op doors; use **F3 Hold Here** + **F5 Plank** or **F4 Help**. They do not solve every puzzle on their own.

## Verification

- New observational playthrough tool `tools/playthrough.ps1`: pilot + 3 AI friends on all seven courses, ordinary input only, zero exceptions.
- 54/54 native AI checks pass; installer, self-update and uninstall verified.
