# Import / export setups

You can export a full configuration to a file and import it back later — useful
for moving to a new PC, sharing a tuned setup, or keeping a master template.

> This is a [VIP feature](free-vs-vip.md).

## What's included

A setup export bundles things like your server profile, its settings, scheduled
tasks, and extensions into a single file with a manifest.

## Exporting

1. Open **Tools** and choose **Export**.
2. Pick what to include.
3. Save the file.

## Importing

1. Open **Tools** and choose **Import**.
2. Select the file and confirm.
3. The app recreates the profiles and settings. Imported profiles get an
   `-imported` suffix so they never overwrite an existing server.

## About secrets

For your security, **secrets are never exported** — things like admin passwords
and Discord tokens. After importing on a new machine, re-enter those in the
relevant screens.

---

**Related:** [Backups](backups.md) · [Settings editor](settings-editor.md)
