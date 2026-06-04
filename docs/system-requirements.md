# System requirements

Before you install Royalty Manager, make sure your PC can host a Palworld
server. Hosting a server is more demanding than just *playing* the game,
because your PC runs the world for everyone connected.

## The app itself

| Requirement | Minimum |
|-------------|---------|
| Operating system | Windows 10 or Windows 11, **64-bit** |
| Disk space for the app | ~150 MB |
| Internet | Required (to download the Palworld server and updates) |

> The app includes everything it needs to run. You do **not** need to install
> .NET, Steam, or any other software first.

## To host a Palworld dedicated server

These are recommendations for a smooth experience. Palworld servers are
memory-hungry.

| Players | RAM (free, for the server) | CPU | Disk |
|---------|----------------------------|-----|------|
| Up to 4 | 8 GB | 4 cores | ~10 GB |
| Up to 8 | 16 GB | 4–6 cores | ~10 GB |
| 16+ | 32 GB | 8 cores | ~15 GB |

A few notes:

- **RAM is the most important factor.** A Palworld server can use 8–15 GB on
  its own once a world fills up. If your PC runs out of memory, the server
  becomes laggy or crashes.
- The numbers above are *in addition to* what Windows and your other programs
  use. Hosting **and** playing on the same PC needs more RAM than the table.
- An **SSD** is strongly recommended — worlds save faster and the server starts
  quicker.

## Network

To let friends join over the internet, you usually need to **open ports** on
your home router (port forwarding). By default Palworld uses:

| Port | Type | Purpose |
|------|------|---------|
| 8211 | UDP | Game traffic (players connecting) |
| 27015 | UDP | Steam query (server list) |
| 25575 | TCP | RCON (admin commands — keep this private) |

Royalty Manager assigns these automatically and avoids conflicts when you run
several servers. See [Creating your first server](creating-your-first-server.md)
and [Troubleshooting](troubleshooting.md#players-cant-join) for help.

---

**Next:** [Installation →](installation.md)
