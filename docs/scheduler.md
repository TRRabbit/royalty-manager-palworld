# Scheduler

The scheduler runs maintenance tasks **automatically** so you don't have to
babysit your server.

## What it can do

| Task | Use it for |
|------|------------|
| **Restart** | A nightly restart keeps the server fast and clears memory |
| **Backup** | Regular automatic backups (see [Backups](backups.md)) |
| **Update** | Apply Palworld game updates on a schedule |

## Adding a scheduled task

1. Open the **Scheduler** from the sidebar (this is a [VIP feature](free-vs-vip.md)).
2. Click **+ Add schedule**.
3. Pick the **action** (Restart / Backup / Update).
4. Pick an **interval** from a simple list
   (1 h / 2 h / 3 h / 4 h / 6 h / 8 h / 12 h / 24 h) — no cron syntax to learn.
5. Save.

## Good to know

- **Tasks run while the app is open.** The scheduler works as long as Royalty
  Manager is running on your PC. If you close the app, scheduled tasks pause and
  resume next time you open it. (Tip: enable
  [launch at Windows startup](installation.md) on a dedicated server PC.)
- **Tasks are saved** between sessions — you set them once.
- **No conflicts:** a scheduled action won't fire while you're already doing
  something to that server manually, and it cooperates with the
  [Guardian](guardian.md).
- A **Restart** task starts the server if it's currently stopped.
- An **Update** task safely stops the server (with player warnings), updates,
  and starts it again.

---

**Related:** [Backups](backups.md) · [Server controls](server-controls.md) · [The Guardian](guardian.md)
