# My5 OBS Dock

My5 OBS Dock is a Windows stream command center for OBS. Signal One 4.0 combines multi-platform chat, current-stream activity, song search and requests, Auto DJ, viewer signals, moderation shortcuts, optional chat voice, and matching OBS browser sources.

## Download

Open **Releases** and download `My5ive-Windows.zip`, or download `My5iveSetup.exe` for the one-file installer.

## Setup

1. Run `My5iveSetup.exe` and choose **Install / Repair My5 OBS Dock**.
2. Choose **Open My5 OBS Dock**.
3. In **Channels**, connect each platform on its official sign-in page.
4. Add the dock and browser-source URLs shown under **OBS Setup**.

There is no Platforms tab and streamers do not paste Client IDs, client secrets, callback URLs, or webhooks. Platform tokens stay protected under each streamer's Windows account.

### Upgrading a very old copy

Builds that already contain the GitHub updater will show the update inside the dock. Builds from before the updater existed cannot receive a popup because they have no update-checking code; run the 4.0 setup once. Install / Repair adopts the existing My5 folder and settings, and every later release can update from inside My5.

## Signal One 4.0

- Restored Player tab inside the OBS dock; the retired standalone My5 Player is removed.
- Explicit **Stream / OBS** and **Personal / Desktop** output modes with one playback owner, preventing doubled or echoed audio.
- Central Stream OS event bus, honest platform adapters and health, explicit stream lifecycle, feature flags, structured logs, and simulation hooks.
- Local, read-only My5tructure intelligence adapter. It imports only compact editing-style signals and never imports footage, transcripts, credentials, or private project content.
- Faster playback recovery with provider-aware buffering windows, queue cleanup, full-track completion checks, Auto DJ, and dual-deck crossfade support.
- Current-session chat, activity deduplication, Unicode and platform emoji rendering, exact viewer endpoints, and TikTok activity signals.
- Automatic GitHub update checks with SHA-256 verification. Existing settings, tokens, and request-room keys are preserved.

## Player audio routing

- Choose **Stream / OBS** when the audience should hear the Request Player browser source through the OBS mixer.
- Choose **Personal / Desktop** when only you should hear playback from the dock.
- Add exactly one Request Player browser source and enable **Control audio via OBS**.

## Verified build

- Clean package: **110/110 passed**
- Activity burst stress: **240/240 passed**, with bounded chat history
- Real browser playback: YouTube, SoundCloud, and Audius sustained playback passed
- Play/pause, skip, queue removal, next approval, Auto DJ, and output-owner handoff passed
- Twitch, YouTube, and Kick authorization starts passed
- TikTok current-chat, emoji, stale-session reset, and replay checks passed
- Stream OS, My5tructure adapter, simulation, health, update integrity, and legacy-player removal passed

`My5ive-Windows.zip` SHA-256:

`F73831F20A79AD14A2E6D4CB632708F4BFE1C638E759481C975E426561AA8276`

`My5iveSetup.exe` SHA-256:

`BA2337DC4633464DCE70F232CD905C1E70A2A7A62519A42E6268EC67F4F10078`
