# Metamorphosis Plugins

The Claude plugin marketplace for [Metamorphosis Worldwide](https://metamorphosis-usa.com).
Add it once and the tools install into your Claude account.

## Install (works in the Claude app, claude.ai, and Claude Code)

Open the plugins screen — in the Claude app / claude.ai it's the **+** menu (or
Settings) → **Plugins**; in Claude Code it's the `/plugin` command — then:

1. **Add marketplace:** `anehemy/metamorphosis`
2. **Install** the **Customer Clarity (Free)** plugin.

No GitHub account needed. Then ask *"who is my customer really?"* or paste a
call transcript, and the skill runs.

Claude Code equivalent:

```
/plugin marketplace add anehemy/metamorphosis
/plugin install mw-customer-clarity-free@metamorphosis
```

## Prefer a single file? (claude.ai alternative)

You can also skip the marketplace and upload the skill as a file:
download **`mw-customer-avatar-builder.zip`** from this repo, then in Claude go
to **Customize → Skills → + → Upload a skill**.

## What's inside

| Item | What it does |
|--------|--------------|
| `mw-customer-avatar-builder` (skill) | Builds one customer avatar from your real call transcripts, in your customers' own words. Pulls from Fathom or Microsoft 365 when connected, or works from pasted transcripts. |

More tools will be added over time.
