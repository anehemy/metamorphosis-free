# Metamorphosis Plugins

Claude tools from [Metamorphosis Worldwide](https://metamorphosis-usa.com).

## Which install do I use?

It depends on **where you use Claude** — because a skill bundled in a plugin
currently runs in **Claude Code** and Cowork, but **not** in the plain
claude.ai chat app.

- **You use the Claude app or claude.ai in a browser** → upload the skill file
  (below). This is the path for most people.
- **You use Claude Code** (the terminal / IDE tool) → add the marketplace
  (below); the skill works automatically.

## claude.ai / Claude desktop app (any plan, including Free)

1. Download **`mw-customer-avatar-builder.zip`** from this repo.
2. In Claude, go to **Customize → Skills → + → Upload a skill** and choose the
   file. Turn it on. (One-time: enable code execution under Settings →
   Capabilities.)
3. Ask *"who is my customer really?"* or paste a call transcript.

## Claude Code (terminal / IDE)

```
/plugin marketplace add anehemy/metamorphosis
/plugin install mw-customer-clarity-free@metamorphosis
```

Then ask *"who is my customer really?"* or paste a transcript. You can also
invoke it directly: `/mw-customer-clarity-free:mw-customer-avatar-builder`.

## What's inside

| Item | What it does |
|--------|--------------|
| `mw-customer-avatar-builder` (skill) | Builds one customer avatar from your real call transcripts, in your customers' own words. Pulls from Fathom or Microsoft 365 when connected, or works from pasted transcripts. |

More tools will be added over time.
