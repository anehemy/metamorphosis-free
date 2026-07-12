# Install — Customer Clarity AI System (Free edition)

By Metamorphosis Worldwide. Build one customer avatar from your real call
transcripts, in your customers' own words. This is the free lead-magnet tier of
the Customer Clarity AI System (CCAIS); the full multi-avatar system, founder
voice, content generation, and CRM logging are the paid edition.

## Install (works in the Claude app, claude.ai, and Claude Code)

Open the plugins screen — in the Claude app / claude.ai it's the **+** menu (or
Settings) → **Plugins**; in Claude Code it's the `/plugin` command — then:

1. **Add marketplace:** `anehemy/metamorphosis-free`
2. **Install** this plugin (`mw-ccais-free`).

Then ask "who is my customer really?" or paste a call transcript and the
`mw-ccais-free-avatar-scan` skill runs. Claude Code equivalent:

```
/plugin marketplace add anehemy/metamorphosis-free
/plugin install mw-ccais-free@metamorphosis-free
```

## Alternative: upload the skill as a file (claude.ai)

Prefer not to add a marketplace? Download `mw-ccais-free-avatar-scan.zip` from
the marketplace repo (`anehemy/metamorphosis-free`), then in Claude go to
**Customize → Skills → + → Upload a skill** and choose it. (One-time: enable
code execution under Settings → Capabilities.)

## Connectors (optional either way)

- **Fathom** — pulls recent recordings and triages which look like real
  customer calls before analyzing.
- **Microsoft 365** — checks your calendar for call-shaped meetings and looks
  for their transcripts in the Teams meeting Recap and your SharePoint/OneDrive
  files. When a transcript is not found, it falls back to paste without fuss.
- **Nothing connected?** Paste a transcript from any source (Teams, Zoom, Otter,
  Fathom export). The skill runs the same way.

## First run

The skill walks you through six quick questions to build an owner profile (so
your own voice is excluded from the customer analysis), then works one
transcript at a time. Nothing to pre-create; it bootstraps itself.
