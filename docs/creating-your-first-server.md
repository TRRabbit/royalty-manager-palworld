# Creating your first server

This is the most important guide. By the end, you'll have a running Palworld
server that your friends can join.

## Step 1 — Add a profile

1. On the main window, click **+ Add a profile** (or the **+** in the sidebar).
2. Give your server a **name** (for example, *My Palworld Server*).
3. Choose a **root folder** where the server files will live. The app creates a
   dedicated sub-folder per server automatically, so two servers never mix.
4. The app pre-fills the **ports** for you (game, query, RCON, REST) and makes
   sure they don't clash with another server. You can leave the defaults.
5. Confirm. Your new server appears as a **card**.

## Step 2 — Install the Palworld server

Your new server is created but the game files aren't downloaded yet.

1. On the server card, click **Install**.
2. The app downloads and runs **SteamCMD** (Steam's official tool) for you — you
   don't need a Steam account or any setup.
3. It then downloads the Palworld dedicated server (~4 GB). A progress bar keeps
   you informed.

> **This takes a while** the first time (it's a 4 GB download). You can keep
> using the rest of the app while it works.

> You may briefly see a transient `ERROR! Failed to install` line from SteamCMD
> during its own self-update. This is normal — the app retries and only reports
> success once the real server file (`PalServer.exe`) is present.

## Step 3 — Adjust settings (optional)

Before the first start, you may want to set a few things:

- Open the server, go to the **Settings editor**, and set your **server name**,
  **admin password**, **max players**, and any gameplay rules you like.
- Not sure? The defaults work fine — you can change everything later and
  restart. See [Settings editor](settings-editor.md).

## Step 4 — Start the server

1. On the server card, click **Start**.
2. The status changes to **Starting**, then **Online** once it's ready (this can
   take a minute as the world loads).
3. The card now shows uptime, player count, CPU, and memory.

🎉 **Your server is live.**

## Step 5 — Let friends join

- **Same network (LAN):** friends use your PC's local IP address and port `8211`.
- **Over the internet:** you must **forward the ports** on your router (see
  [System requirements → Network](system-requirements.md#network)). Then friends
  connect using your **public IP** and port `8211`.

In Palworld, players join via **Join Multiplayer Game → Connect to a server**
and enter `your-ip:8211`.

Trouble? See [Troubleshooting → Players can't join](troubleshooting.md#players-cant-join).

## Step 6 — Protect it

Now that it works, set up:

- **[Backups](backups.md)** — so you never lose your world.
- **[The Guardian](guardian.md)** — so the server restarts itself if it crashes.
- **[Scheduler](scheduler.md)** — for automatic nightly restarts.

---

**Next:** [Server controls →](server-controls.md)
