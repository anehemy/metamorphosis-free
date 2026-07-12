# Metamorphosis Plugins

The Claude plugin marketplace for [Metamorphosis Worldwide](https://metamorphosis-usa.com).
Add it once and our tools install straight into your Claude account.

## Install (easiest, works on any Claude plan)

In the Claude app or on claude.ai:

1. Open the **+** menu and choose **Plugins** (or go to Settings, then Plugins).
2. Choose **Add marketplace**.
3. Paste this address: **`anehemy/metamorphosis`**
4. Install **Customer Clarity (Free)** from the list.

No GitHub account needed. That is the whole thing.

## Install (Claude Code / terminal)

```
/plugin marketplace add anehemy/metamorphosis
/plugin install mw-customer-clarity-free@metamorphosis
```

## Available plugins

| Plugin | What it does |
|--------|--------------|
| `mw-customer-clarity-free` | Free edition of the Customer Clarity AI System: builds one customer avatar from your real call transcripts, in your customers' own words. See its [INSTALL.md](plugins/customer-clarity-free/INSTALL.md). |

More plugins will be added over time; re-open the marketplace (or run
`/plugin marketplace update metamorphosis` in Claude Code) to pick them up.
