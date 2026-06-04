# The Guardian (anti-crash)

The Guardian is a built-in watchdog that keeps your server alive. If the server
crashes or freezes, the Guardian brings it back — even at 3 a.m. while you sleep.

## What it watches

For each server you enable it on, the Guardian checks:

- **Is the process alive?** If the server process dies (a crash), it restarts it.
- **Is the server responding?** It pings the server regularly (RCON health
  check, about every 5 minutes). If the server is frozen and stops answering,
  it's treated as hung and restarted.
- **Is there a game update?** It can detect when Palworld has a new version
  available and, when configured, stop the server gracefully, update it, and
  start it again.

## Turning it on

1. Open the server's profile editor.
2. Find the **Guardian** section and tick **Enable** for that server.

The setting is **per server**, so you can protect one server and leave another
unmanaged. Your choice is remembered.

## It won't fight with you

The Guardian is designed to never get in your way:

- If **you** (or a [scheduled task](scheduler.md)) are starting, stopping,
  updating, or backing up the server, the Guardian stays out of the way and
  won't trigger a restart in the middle.
- If you **stop the server yourself**, the Guardian understands that's
  intentional and does **not** restart it.
- It uses a back-off so it won't loop forever — after a few failed attempts it
  gives up and (if Discord is set up) can alert you.

## Crash alerts

When a crash happens, the Guardian can send a [Discord](discord.md) notification
so you know about it immediately (only if you've set Discord up — otherwise it
stays silent).

---

**Related:** [Scheduler](scheduler.md) · [Discord integration](discord.md) · [Server controls](server-controls.md)
