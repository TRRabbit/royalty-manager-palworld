# Troubleshooting

Quick fixes for the most common problems. If your issue isn't here, check the
[FAQ](faq.md) or ask on [Discord](https://discord.gg/RjzkFaJsC5).

## "Windows protected your PC" when installing

This is the normal SmartScreen warning for new independent software. Click
**More info → Run anyway**. See [Installation](installation.md#2-the-windows-protected-your-pc-warning).

## The install shows an error but seems to work

During install you might see a brief `ERROR! Failed to install` line from
SteamCMD. This is a **transient** message from Steam's own updater. The app
retries and only reports real success once `PalServer.exe` exists. If the server
ends up installed, you're fine.

## Players can't join

1. **Same network?** Make sure friends use your PC's local IP and port `8211`.
2. **Over the internet?** You must **forward the ports** on your router:
   - `8211` UDP (game) and `27015` UDP (query).
   - Keep `25575` (RCON) **private** — don't forward it unless you know you need
     remote RCON.
3. **Firewall:** allow `PalServer.exe` through Windows Firewall when prompted.
4. **Double-check the public IP** you gave them (search "what is my IP").

See [System requirements → Network](system-requirements.md#network).

## "Couldn't find an open port" / port conflict

This happens when two servers try to use the same port. Royalty Manager assigns
distinct ports per server automatically — if you hit this, open the profile and
make sure each server has its **own** game/query/RCON/REST ports (the app
suggests free ones). Restart the server after changing ports.

## The server status is stuck on "Starting"

- Loading a big world can take a minute — give it time.
- Make sure the **REST API** is enabled in the server's
  [settings](settings-editor.md) (the app needs it to read status).
- Check you have enough **free RAM** (see [System requirements](system-requirements.md)).

## The server keeps crashing

- Low RAM is the usual cause — close other programs or add more memory.
- Turn on the **[Guardian](guardian.md)** so it restarts automatically.
- If you just installed a mod, try removing it to see if it's the cause.

## A mod won't install

- Use **Check for update** in the [Mods](mods.md) tab to reinstall cleanly.
- Make sure the server is **stopped** while installing mods.
- Use **Open folder** to confirm the files actually landed in the server folder.

## The app opens with old test data / I want a clean start

Use **Reset application** in **Settings** (danger zone). It clears the app's own
data without deleting your Palworld server files. See
[Free vs VIP → Reset application](free-vs-vip.md#reset-application).

## Discord alerts/bot don't work

- Discord is a [VIP feature](free-vs-vip.md) — check your edition badge.
- For a webhook, re-create it in Discord and **Test** it in the app.
- For the bot, confirm the **token** is correct and the bot is invited to your
  server with permission to post.

## I lost my world

- Restore from a [backup](backups.md) if you have one.
- The Palworld server files are **not** deleted when you uninstall the app or
  reset it, so check the server folder you chose at creation.

---

Still stuck? **[Open a ticket on Discord](https://discord.gg/RjzkFaJsC5)** and
we'll help.
