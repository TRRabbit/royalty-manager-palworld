# Updating the app

Royalty Manager keeps itself up to date — you don't have to reinstall it
manually for every new version.

## Automatic updates

- When a new version is released, the app updates **itself** on launch.
- Updates are **delta updates**: it only downloads what changed (often just a
  few tens of kilobytes), not the whole app again.
- New versions are published here on **GitHub Releases**, which is where the app
  fetches them from.

You normally don't need to do anything — just keep using the app.

## Updating manually

If you ever want to update by hand (for example after a long time offline):

1. Go to the **[latest release](https://github.com/TRRabbit/royalty-manager-palworld/releases/latest)**.
2. Download and run the installer.
3. It updates your existing installation in place. Your servers, settings, and
   backups are kept.

## Updating the Palworld **game** server

That's separate from updating the app. To update the Palworld dedicated server
itself, use the **Update** button on the server card, or set up an automatic
update task in the [Scheduler](scheduler.md). See [Server controls](server-controls.md).

## Release notes

Each release on the [Releases page](https://github.com/TRRabbit/royalty-manager-palworld/releases)
lists what changed, so you can see what's new.

---

**Related:** [Installation](installation.md) · [Server controls](server-controls.md)
