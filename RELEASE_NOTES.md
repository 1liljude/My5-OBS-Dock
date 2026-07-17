# My5 OBS Dock v1.3.5 - Dock-First Managed Sign-In

## Streamer setup is now three steps

1. Install or repair My5 OBS Dock.
2. Open the dock and choose Channels.
3. Click Connect, sign in on the platform's official page, and approve.

The setup app now contains only Welcome, OBS Setup, and Guide. The old Platforms tab, Client ID fields, client-secret fields, callback instructions, developer-portal buttons, webhook setup, and Save Platform Setup workflow were removed.

## Managed platform login

- Twitch authorization starts from the local service and stores renewable tokens.
- YouTube authorization now starts from the local service; the dock no longer reads or displays the bundled client ID.
- Kick authorization, token exchange, renewal, webhook subscription, and relay continue through the hosted My5 backend.
- TikTok asks for the exact live @username only when Connect is clicked.
- Legacy local app-ID and Kick-secret overrides are removed during Install / Repair so every tester uses the supported managed configuration.
- The user-facing config endpoint returns provider readiness only; it does not return platform Client IDs or secret status.

## Request link and OBS

- AUXDROP room creation now happens automatically through the managed backend.
- Requests includes a Share Request Link button that creates and copies the viewer link.
- Opening the dock from Setup starts the service and waits for it before loading, preventing the old page-not-loaded screen.
- The OBS source URLs remain under OBS Setup.

## Verified

- Clean-package suite: 80/80 passed.
- Twitch, YouTube, and Kick managed authorization starts: passed.
- No Platforms tab and no exposed user-facing platform IDs: passed.
- Automatic request-room setup: passed.
- OBS dock, chat overlay, request player, viewer endpoints, playback controls, search, and Auto DJ checks: passed.
- Private credential filename scan: passed.

## Download

My5-OBS-Dock-Windows-v1.3.5.zip

SHA-256: E37B0210684FD816D0559072545509921ED117CCBE373E188124A651148FE936
Size: 103828903 bytes
