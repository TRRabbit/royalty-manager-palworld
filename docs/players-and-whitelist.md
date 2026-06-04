# Players & whitelist

Manage who is on your server, and who is allowed in.

## The Players screen

Open a server and go to the **Players** tab. You'll see two tables:

- **Online now** — players currently connected, refreshed live from the server.
- **History** — players who have connected before, with their total play time
  and last session.

For each player you can:

- **Kick** — disconnect them now.
- **Ban** — block them. If they're offline, the ban is queued and applied the
  moment they try to reconnect.
- **Unban** — the Unban button only appears for players who are currently
  banned, so the list stays clean.

## Whitelist (allow-list)

A whitelist lets you restrict your server to **only approved players**.

1. Go to the **Whitelist** tab of the server.
2. Add players (by their Steam ID). The app validates the ID format for you.
3. Choose the enforcement mode:
   - **Native** — uses Palworld's own kick mechanism.
   - **PalDefender** — stronger, mod-enforced blocking (requires the
     [PalDefender mod](mods.md)). If PalDefender isn't installed, the app warns
     you and falls back to Native.

When the whitelist is active, anyone not on the list is automatically removed
when they try to join.

> **Finding a Steam ID:** ask the player for their 17-digit SteamID64, or copy
> it from the Players history after they've connected once.

---

**Related:** [RCON console](rcon-console.md) · [Mods (PalDefender)](mods.md) · [Discord integration](discord.md)
