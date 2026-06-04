# Updating the app

Royalty Manager checks for new versions for you and makes updating a couple of
clicks — you don't have to hunt for downloads.

## How update checks work

- When you open the app, it quietly checks here on **GitHub Releases** for a
  newer version (in the background — if you're offline or there's nothing new,
  you won't see anything).
- If a newer version is available, the app shows a small window:
  **"An update (vX.Y.Z) is available. Download and install?"** with
  **Download & install** and **Later** buttons.
- If you choose **Download & install**, the app downloads the new installer,
  then launches it. Windows will ask for permission (the standard "Do you want
  to allow this app to make changes?" prompt) — click **Yes**. The installer
  updates your existing installation, keeping your servers, settings, and
  backups.
- Choose **Later** and you'll simply be asked again next time you open the app.

> Nothing is ever installed without your confirmation.

## Check manually

You can also check any time from **Settings → Check for updates**. If you're
already on the latest version, it tells you so.

## Updating manually (alternative)

You can always update by hand:

1. Go to the **[latest release](https://github.com/TRRabbit/royalty-manager-palworld/releases/latest)**.
2. Download and run the installer.
3. It updates your existing installation in place.

## Updating the Palworld **game** server

That's separate from updating the app. To update the Palworld dedicated server
itself, use the **Update** button on the server card, or set up an automatic
update task in the [Scheduler](scheduler.md). See [Server controls](server-controls.md).

## Release notes

Each release on the [Releases page](https://github.com/TRRabbit/royalty-manager-palworld/releases)
lists what changed, so you can see what's new.

---

**Related:** [Installation](installation.md) · [Server controls](server-controls.md)
