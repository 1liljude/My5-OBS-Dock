# My5 OBS Dock

My5 OBS Dock is a Windows stream command center for OBS. It combines multi-platform chat, song requests, viewer counts, moderation shortcuts, optional chat voice, and matching OBS browser sources in one dock.

## Download

Open the repository's **Releases** page and download:

`My5-OBS-Dock-Windows-v1.3.4.zip`

## Install

1. Extract the ZIP.
2. Open `My5iveSetup.exe`.
3. Select **Install / Repair My5ive**.
4. Select **Start Service**.
5. Use the **OBS Setup** tab to copy the dock and browser-source URLs into OBS.
6. Open the dock's **Connect** tab and sign in to the platforms you stream on.

The installer includes the local service and everything needed to run it. Testers do not need Node.js or npm.

## Platform sign-in

- **Twitch:** Select Connect, enter the approval code, and authorize.
- **YouTube:** Select Connect and approve the Google Production login. Google may display an unverified-app warning until the app finishes OAuth verification.
- **Kick:** Select Connect and authorize through the hosted My5ive relay.
- **TikTok LIVE:** Enter the exact live `@username` used by the community connector.

Tokens are stored under each person's own Windows account. Developer secrets, creator tokens, chat history, and personal credentials are not included in the download.

## OBS sources

The setup app provides copy buttons for:

- My5 OBS Dock
- Chat overlay
- Request player and viewer counts

Use one request-player browser source at a time and enable **Control audio via OBS** for that source to avoid doubled audio.

## Verified build

- Clean-package checks: **80/80 passed**
- Twitch managed sign-in start: passed
- Kick managed sign-in and relay security checks: passed
- OBS dock, overlays, request player, playback controls, search, Auto DJ, and viewer endpoints: passed

SHA-256:

`ED30B57F25DA5F188E609FC3D329C0B5ED69BD93E56A06D081FA8A81EAF2DD6C`

