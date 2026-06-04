# Settings editor

The settings editor lets you change **every official Palworld server setting**
through a clean interface — no editing `.ini` files by hand.

## How to open it

Open a server (click its card), then go to the **Settings** tab.

## How it's organised

Settings are grouped into tabs so you can find things quickly:

| Tab | What's inside |
|-----|---------------|
| **General** | Server name, description, admin password, max players |
| **Network & API** | Ports, RCON, REST API toggles |
| **Multipliers** | XP rate, gather/craft rates, Pal capture rate, egg hatch time, etc. |
| **Rules** | PvP, friendly fire, death penalty, fast travel, raids, and more |
| **Advanced** | Less-common options for power users |
| **Optimization** | Performance-related recommendations |
| **All settings** | A full searchable list of every parameter |

## Help on every setting

Hover your mouse over any setting to see a **plain-language tooltip** explaining
what it does. The tooltip stays visible for about 20 seconds so you have time to
read it.

## Applying changes

1. Change the values you want.
2. **Save**.
3. **Restart** the server so the new settings take effect (a running server
   reads its settings at startup).

> Tip: change several settings at once, then do a single restart, rather than
> restarting after each change.

## Command-line arguments

Advanced users can add custom **launch arguments** for `PalServer.exe` per
profile. These are saved as a small file in the server's folder.

## World option conflicts

Palworld stores some choices in a `WorldOption.sav` file. If the app detects a
conflict between your settings and that file, it offers a one-click
**"Save and regenerate"** so your new settings win without corrupting the world.

---

**Related:** [Server controls](server-controls.md) · [Event mode](event-mode.md) · [Backups](backups.md)
