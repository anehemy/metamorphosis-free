# Install — Customer Clarity AI System (Free edition)

By Metamorphosis Worldwide. Build one customer avatar from your real call
transcripts, in your customers' own words. This is the free lead-magnet tier;
the full multi-avatar system, founder voice, content generation, and CRM
logging are the paid edition.

## Pick your install based on where you use Claude

A skill bundled in a plugin currently runs in **Claude Code** (and Cowork),
**not** in the plain claude.ai chat app. So there are two paths:

- **claude.ai / Claude desktop chat** (any plan, including Free): upload the
  skill file directly. This is the path for most people.
- **Claude Code** (terminal / IDE): add the marketplace; the skill works
  automatically.

## Path A — claude.ai / Claude desktop app

1. Download `mw-customer-avatar-builder.zip` from the marketplace repo
   (`anehemy/metamorphosis`).
2. In Claude: **Customize → Skills → + → Upload a skill**, choose the `.zip`,
   turn it on. (One-time: enable code execution under Settings → Capabilities.)
3. Ask "who is my customer really?" or paste a call transcript.

## Path B — Claude Code

```
/plugin marketplace add anehemy/metamorphosis
/plugin install mw-customer-clarity-free@metamorphosis
```

Verify: ask "who is my customer really?" or paste a transcript and the
`mw-customer-avatar-builder` skill triggers. You can also invoke it directly
with `/mw-customer-clarity-free:mw-customer-avatar-builder`.

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
