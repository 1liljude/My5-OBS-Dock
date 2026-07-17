# My5 OBS Dock

My5 OBS Dock is a Windows stream command center for OBS. It combines multi-platform chat, song requests, viewer counts, moderation shortcuts, optional chat voice, and matching OBS browser sources in one dock.

## Download

Open the repository's **Releases** page and download:

`My5-OBS-Dock-Windows-v1.3.5.zip`

## Three-step setup

1. Extract the ZIP and run `My5iveSetup.exe`.
2. Select **Install / Repair My5 OBS Dock**, then **Open My5 OBS Dock**.
3. Open **Channels**, select **Connect**, sign in on each platform's official page, and approve.

That is the entire platform setup. There is no Platforms tab and no developer-app configuration for streamers. Users never paste Client IDs, client secrets, callback URLs, or webhooks.

The shared public app identity is bundled, private service secrets remain on the hosted My5 backend, and every streamer's platform tokens stay protected under their own Windows account.

## Platform sign-in

- **Twitch:** Confirm the short approval code. The login renews automatically.
- **YouTube:** Choose the Google account that owns or manages the live channel and approve the managed Production app. Google may display an unverified-app warning until public verification finishes.
- **Kick:** Sign in and approve. The hosted backend handles private token exchange, renewal, webhook subscription, and chat relay.
- **TikTok LIVE:** Select Connect and enter the exact live `@username`.

Background watchers start with My5 OBS Dock and attach when an active stream appears. If a platform revokes a login, only that platform asks for reauthorization.

## Viewer song-request link

Open **Requests** and select **Share Request Link**. My5 OBS Dock automatically creates the private AUXDROP room and copies the simple public link.

## OBS sources

The setup app provides copy buttons for:

- My5 OBS Dock
- Chat overlay
- Request player and viewer counts

Use exactly one Request Player browser source and enable **Control audio via OBS** to avoid duplicate audio.

## Verified build

- Clean-package checks: **80/80 passed**
- Twitch, YouTube, and Kick managed authorization starts: passed
- No Platforms tab and no user-facing platform IDs: passed
- Automatic request-room setup: passed
- OBS dock, overlays, request player, playback controls, search, Auto DJ, viewer endpoints, and credential scans: passed

SHA-256:

`E37B0210684FD816D0559072545509921ED117CCBE373E188124A651148FE936`
