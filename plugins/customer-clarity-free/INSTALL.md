# Install runbook — Customer Clarity AI System (Free edition)

The free lead-magnet tier of the Customer Clarity AI System by Metamorphosis
Worldwide. One skill, one job: turn a founder's real call transcripts into one
customer avatar written in their customers' own words.

## What this is

A Claude Code plugin bundling a single skill:

- **`customer-avatar-builder`** — pulls transcripts from Fathom when connected,
  or accepts pasted transcripts from any source (Teams, Zoom, Otter, exports),
  then builds ONE customer avatar from the strongest pattern across the calls.
  When it detects more than one customer type, it names that and points to the
  full paid system rather than forcing a blurry single avatar.

This is the **generic free edition** from the Skill Shop — not a casting tuned
to a specific client. It is deliberately capped at one avatar; the multi-avatar
engine, founder voice, content generation, scheduled intake, and CRM logging
are the **paid edition**.

## Prerequisites

1. **Claude Code installed** on the user's machine.
2. **A public marketplace** (`anehemy/metamorphosis`) — no GitHub account or
   auth needed to install. Claude Code clones the public repo itself.

This plugin ships inside the **metamorphosis** marketplace (one marketplace
repo, multiple plugins under `plugins/`). The marketplace entry uses a relative
source (`./plugins/customer-clarity-free`), so there is no external repo
reference to hijack and nothing to edit before installing.

## Install steps

Run inside Claude Code:

```
/plugin marketplace add anehemy/metamorphosis
/plugin install customer-clarity-free@metamorphosis
```

Verify: ask Claude "who is my customer really?" or paste a call transcript —
`customer-avatar-builder` should trigger.

## Connector setup (optional, not blocking)

- **Fathom** — for the skill to pull recordings directly. If not connected, the
  skill falls back to pasted transcripts, so this is **not** blocking for a
  first run. (Microsoft Teams recordings are supported today only via paste; a
  native Microsoft 365 pull is a tracked enhancement — see the product map.)

## What the founder needs on first run

The skill creates its own `customer-clarity/` working folder and, on the very
first analysis, walks the founder through six quick questions to build
`owner_profile.md` (so the founder's own voice is excluded from customer
analysis). Nothing to pre-create — the free skill bootstraps itself, unlike the
paid skills which expect the shared folder to already exist.
