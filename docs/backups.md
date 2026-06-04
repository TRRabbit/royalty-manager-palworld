# Backups

Backups protect your world. If something goes wrong — a bad update, a corrupted
save, a griefer — you can roll back to a known-good copy.

## Manual backup

1. Open a server and go to the **Backups** tab.
2. Click **Create backup**.
3. The app packages your configuration and world data into a single `.zip`
   archive, listed with its date and size.

## Scheduled (automatic) backups

You can have the app back up on a fixed interval without you doing anything:

1. Go to the [Scheduler](scheduler.md).
2. Add a **Backup** task and pick an interval
   (1 h / 2 h / 3 h / 4 h / 6 h / 8 h / 12 h / 24 h).

The task runs as long as the app is open, and is remembered between sessions.

## Rotation (no full disk)

Backups rotate automatically: the app keeps a sensible number of recent copies
and removes the oldest, so your disk doesn't fill up over time.

## Restoring

1. In the **Backups** tab, pick the backup you want.
2. Click **Restore** and confirm.
3. The app puts the saved files back in place.

> **Restore replaces your current world** with the backup. Make a fresh backup
> first if you're unsure, so you can go back either way.

## Where backups are stored

Backups are stored as `.zip` files in a folder you can configure. Because
they're plain ZIPs, you can also copy them to another drive or cloud folder for
extra safety.

## Safety

- Archives are built with protection against malicious paths.
- A manifest marks sensitive files inside each archive.

---

**Related:** [Scheduler](scheduler.md) · [Import / export setups](marketplace.md)
