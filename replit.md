# Minecraft AFK Bot

A Mineflayer-based Minecraft bot that keeps an Aternos server online 24/7 by automatically joining and preventing AFK kicks.

## How to run

The app starts with:
```
npm start
```

This launches the Express web dashboard on port 5000 and connects the bot to the configured Minecraft server.

## Configuration

Edit `settings.json` to change:
- `server.ip` / `server.port` — your Aternos server address
- `bot-account.username` — the bot's in-game name
- `utils.chat-messages` — messages the bot sends in-game
- `utils.auto-auth.password` — password for cracked-server auto-login
- `movement` — anti-AFK movement settings (circle walk, random jumps, etc.)
- `discord` — optional Discord webhook notifications

## Dashboard

Visit the app URL to see:
- `/` — live status dashboard (connected/disconnected, uptime, coords)
- `/logs` — bot log viewer with in-game command console
- `/tutorial` — setup guide
- `/health` — JSON health endpoint

## Stack

- Node.js 22
- [mineflayer](https://github.com/PrismarineJS/mineflayer) — Minecraft bot framework
- [mineflayer-pathfinder](https://github.com/PrismarineJS/mineflayer-pathfinder) — movement/navigation
- Express — web dashboard server

## User preferences

_No preferences recorded yet._
