# My5 OBS Dock v4.0.0 — Signal One

Signal One turns My5 into a dock-first stream operating layer while keeping today’s behavior compatible and future automation safely feature-flagged.

## What changed

- The full Player is back inside the My5 OBS dock.
- The old standalone My5 Player app and desktop shortcut are removed during Install / Repair.
- A clear output switch selects **Stream / OBS** or **Personal / Desktop**. Web Locks plus the server output mode ensure only one audio owner is active.
- The new Stream OS core provides a normalized event bus, bounded event history, structured logs, explicit stream states, platform adapters, module health, feature flags, and a safe simulation endpoint.
- My5tructure is connected through a local read-only intelligence adapter. Only compact style metadata is used; footage, transcripts, secrets, and private project data never enter My5.
- Playback now distinguishes buffering from true blocking, gives each provider a realistic startup window, nudges stalled embeds before rescue, and avoids premature source switching.
- Existing Player features remain: mixed-source search, viewer requests, queue cleanup, approval flow, Auto DJ, transport controls, full-track completion, and crossfade preparation.
- The installer, setup guide, updater, package verifier, and legacy cleanup now match the dock-only Player architecture.

## Verification

- Clean-package checks: **110/110 passed**
- Activity stress: **240/240 passed**
- Real browser playback: YouTube, SoundCloud, Audius, pause/resume, skip, completion, next approval, and output handoff passed
- Managed authorization-start checks passed for Twitch, YouTube, and Kick
- TikTok current-chat, Unicode/emoji, stale-session reset, and replay checks passed
- No legacy My5 Player executable, launcher, or desktop shortcut remains in the package

## Assets

- `My5iveSetup.exe` — one-file Windows x64 setup
- `My5ive-Windows.zip` — portable release package
- `My5ive-update.zip` — SHA-256-verified automatic update payload
- matching `.sha256.txt` files

Setup SHA-256: `BA2337DC4633464DCE70F232CD905C1E70A2A7A62519A42E6268EC67F4F10078`

ZIP SHA-256: `F73831F20A79AD14A2E6D4CB632708F4BFE1C638E759481C975E426561AA8276`

Update SHA-256: `23B352744544E2866800F2B83A25DEFE2A30D3C367B08D99EF3B545F960232F8`
