# Server controls

Once a server is installed, you control it from its **card** and its detail
view.

## The action buttons

| Button | What it does |
|--------|--------------|
| **Start** | Launches the server. Status goes *Starting → Online*. |
| **Stop** | Asks the server to shut down cleanly (saves the world first). |
| **Restart** | Stops then starts again — handy after changing settings. |
| **Kill** | Forces the server process to close immediately. Use only if it's frozen and won't stop normally. |
| **Cancel** | While a Start/Stop/Restart/Update is in progress, cancels it. |

> **Graceful stop with warnings:** when you Stop or Restart, the app can warn
> connected players in-game at **T-15, T-10, T-5, and T-1 minutes** before the
> shutdown, so nobody is surprised. You set the warning delay in the settings.

## Server status

Each card shows the live status:

- **Starting** — the server is loading the world.
- **Online** — ready for players. Shows uptime, player count, CPU and memory.
- **Stopping** — shutting down.
- **Crashed / Unreachable** — something went wrong (the [Guardian](guardian.md)
  can restart it automatically).
- **Updating / Backing up** — a maintenance task is running.

## Update the game

- Click **Update** to fetch the latest Palworld server files from Steam.
- You can also turn on **auto-update before each start** per profile, so your
  server is always current when it launches.

## Running several servers

You can create as many **profiles** as you like. Each one is fully isolated:
its own folder, ports, settings, and backups. Starting one never touches
another.

> Running **more than one server at the same time** is a
> [VIP feature](free-vs-vip.md). In the free edition you can create extra
> profiles but only run one server at a time.

## Where files live

- The **app's data** (your profiles, settings, backups list) is stored under
  your Windows user folder.
- The **Palworld server files** live in the folder you chose when creating the
  profile.

If you ever want a completely clean slate, the **Reset application** button in
[Settings](free-vs-vip.md) wipes the app's own data (it does **not** delete your
Palworld server files on disk).

---

**Related:** [Settings editor](settings-editor.md) · [Scheduler](scheduler.md) · [The Guardian](guardian.md)
