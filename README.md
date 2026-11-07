# Atlas — Aternos AFK Bot (Minecraft Java 26.3)

Configured for `qc64.aternos.me:27977` and Minecraft Java `26.3`. The bot account name is `Atlas`.

## Run locally or on a Node.js host

1. Install **Node.js 20 or newer**.
2. Extract this folder.
3. Run `npm install`.
4. Run `npm start`.

The bot must run on a separate computer or Node.js hosting service; Aternos does not run arbitrary Node.js bot projects inside the Minecraft server itself. Keep the Aternos server online before starting Atlas.

## Important account setting

`settings.json` currently uses `"type": "offline"`. This only works if the Aternos server allows cracked/offline accounts (`online-mode` disabled). If the server is in online mode, Atlas needs a real Microsoft-authenticated Minecraft account and the bot's authentication setup must be changed; an offline username alone will not join.

## Configuration

- Server: `qc64.aternos.me`
- Port: `27977`
- Minecraft Java version: `26.3`
- Bot name: `Atlas`

Auto-auth and repeating chat messages are disabled by default so the bot does not send an unknown password or promotional spam. If your server uses `/login`, set your own password in `settings.json` and enable `utils.auto-auth`.

## Compatibility note

This build uses the `@wp2508/mineflayer` fork, which advertises Minecraft 26.3 support. This is a third-party fork rather than the standard upstream Mineflayer release.
