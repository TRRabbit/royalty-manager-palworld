# Discord integration

Connect your server to Discord to get **alerts** and even **control the server
from Discord**. Open a server and go to the **Discord** tab.

> Discord integration is a [VIP feature](free-vs-vip.md). In the free edition the
> Discord tab is visible as a **preview** (disabled), so you can see what it
> offers.

## 1. Webhook alerts (notifications)

The simplest option: have the app post messages to a Discord channel when things
happen.

**Events you can announce:** server started, stopped, crashed, backup success,
backup failure, player joined, player left, scheduled task ran, event mode
started/ended.

Highlights:

- **Multiple webhooks** — not just one global channel. You can route different
  event types (and different servers) to different channels.
- **Visual routing** — map each event to one or more webhooks.
- **Filter by server** — only broadcast events from the servers you choose.
- Webhook URLs are **encrypted at rest** (Windows DPAPI).

To set one up: create a webhook in your Discord channel
(*Channel settings → Integrations → Webhooks*), paste the URL into the app,
pick which events to send, and **Test** it.

## 2. The control-panel bot

Go further with a real Discord bot that posts an interactive **control panel**:

- Buttons to **Start / Stop / Restart / Backup** your server, right from Discord.
- A **status panel** showing the server state, uptime, and players.
- **Target server selection** when you manage several.
- **Per-role permissions** — only members with the Discord role you choose can
  press the action buttons. Every click is permission-checked before anything
  happens.

You'll need to create a bot in the
[Discord Developer Portal](https://discord.com/developers/applications) and paste
its token into the app (the token is stored encrypted).

## 3. Voice-channel status

The bot can rename a **voice channel** to reflect your server status — for
example *"Server — 🟢 — 3/16 online"* — so members see at a glance whether the
server is up, without opening anything.

> Discord limits how often a channel can be renamed (about twice per 10 minutes),
> so the status refreshes on a fixed interval of a few minutes, not instantly.

## Language

Discord messages are in **English** by default, with French available.

---

**Related:** [The Guardian](guardian.md) · [Free vs VIP](free-vs-vip.md)
