# Customer Avatar Builder — Output Templates


Use these structures exactly. Consistency across conversations is what makes the intelligence cumulative. Each template names "Where this goes": save the file at that path when a filesystem is available; otherwise produce the same content as a labeled, copyable Markdown block in the chat, and keep it available for the rest of the session.

### 1. Owner Profile

Where this goes: `customer-clarity/owner_profile.md`, when available; otherwise a copyable block.

```markdown
# Owner Profile

This file identifies the Owner of the Customer Avatar Builder.
The Owner's voice, language, and identity are EXCLUDED from customer analysis.
The system analyzes the OTHER person in every conversation, never the Owner.

- Name: [Answer 1]
- Business: [Answer 2]
- Role: [Answer 3]
- Industry / Customer Type: [Answer 4]
- Location: [Answer 5]
- Voice Patterns: [Answer 6, or "None specified"]

---

Generated [Date] by the Customer Avatar Builder onboarding interview.
To update, delete this file and re-run any analysis, or just say so if
we're working in-chat without a file.
```

### 2. Transcript

Where this goes: `customer-clarity/transcripts/transcript_YYYY-MM-DD_customer-name-lowercase-hyphenated.md`, when available; otherwise a copyable block.

```markdown
# Transcript: [Date], [Customer Name]

Date: [YYYY-MM-DD from transcript metadata]
Duration: [Length if visible, otherwise "Unknown"]
Source: [Fathom / Microsoft 365 / Teams / Zoom / Otter / Other if identifiable]
Owner: [Owner's name from the owner profile]
Customer: [Customer's name, or "Unknown"]
Context: [One-line summary if obvious, otherwise blank]

---

## Transcript

OWNER [Owner Name, timestamp]: [What they said]

CUSTOMER [Customer Name, timestamp]: [What they said]

[... continues through the entire transcript ...]
```

Formatting rules: real names are preserved in the filename (or block label) and inline labels, this is the audit trail. Role tags (`OWNER:` / `CUSTOMER:`) are baked in alongside names so analysis never re-asks who is who. Preserve timestamps when present, and preserve filler words and ums, do not clean the transcript. A third speaker gets the label `OTHER [Name, timestamp]` and a Context note: "Three or more speakers in this conversation."

### 3. Debrief questions (no-transcript path)

Ask one at a time, waiting for each answer:

1. What kind of conversation was this: sales call, networking, discovery, follow-up, customer call?
2. What did the other person say that stuck with you? Try to give me their exact words, even if rough.
3. What lit them up in the conversation? What made them go quiet?
4. What do they want vs what they have right now?
5. What did they push back on, even subtly? What did they refuse to consider?
6. Did they use sensory language, words like "see," "feel," "think," "hear," and which ones came up most?

After the sixth answer, produce a Conversation Insight (below) with Source marked "Debrief."

### 4. Conversation Insight

Where this goes: `customer-clarity/insights/insight_YYYY-MM-DD_archetype.md`, when available; otherwise a copyable block. The archetype in the name describes the customer type, never the individual.

```markdown
# Conversation Insight, [Date]

Source: [Transcript / Debrief]
Anonymized: Yes, identifying details stripped
Owner Excluded: Yes, analysis is of the customer, not the owner

## Customer Language (Verbatim)
[Direct quotes from the customer only. Word for word. No paraphrasing.
Categorized loosely: pain, hope, identity, objection, language patterns.
These phrases are the gold.]

## What This Conversation Reveals
[Short paragraph on what was learned about the customer archetype.
Not about the specific person; about what kind of customer they represent.
Service-oriented framing.]

## Demographic Signals
[Industry, role, business stage, scale. What kind of business is this customer?]

## Psychographic Signals
[What they value, what they fear, how they make decisions. What kind of mind is this customer?]

## Psychological Dimensions
[Brief notes where this conversation provides signal. Mark "no signal yet" where unclear.]

- Cognitive Style: [observation or "no signal yet"]
- Emotional Register: [observation or "no signal yet"]
- Authority Orientation: [observation or "no signal yet"]
- Pacing and Rhythm: [observation or "no signal yet"]
- Distinctive Vocabulary: [observation or "no signal yet"]
- Belief Topology: [observation or "no signal yet"]
- Decision Signals: [observation or "no signal yet"]

## Pattern Match
[How this conversation fits or breaks the pattern so far.
First conversation: "Initial baseline established."
Later: "Confirms / contradicts / extends prior pattern."
If 3+ insights now exist: "Enough signal to check for multiple avatars."]

## What Worked (Owner Messaging Intelligence)
[Did anything the Owner said produce a strong response from the customer?
Note it as messaging intelligence. This is the only context in which
the Owner's words are referenced.]

## One Question To Ask Next Time
[A single specific question that would deepen understanding of the archetype.]

---
Use this to serve them better, not against them.
```

### 5. Customer Avatar Profile

Where this goes: `customer-clarity/avatars/avatar_1_descriptive-name.md`, when available; otherwise a copyable block.

```markdown
# Customer Avatar, [Avatar Name]

Conversations contributing: [count]
Last updated: [date]
Owner Excluded: Yes, this profile is of the customer, not the owner
Confidence: [Developing / Building / Established]

## Who They Are (Demographic)
[2-3 paragraph aggregate description. Industry, role, business stage,
what their work looks like day to day. Built from patterns across
conversations, not from any single one.]

## How They Talk (Voice Signature)
[Distinctive phrases, recurring metaphors, the texture of how they speak.
This is the brand voice library: the actual words to use in marketing.]

## What They're Stuck On (Pain)
[Verbatim pain phrases organized by theme. Categorized:
external pain, internal pain, philosophical pain.]

## What They Actually Want (Hope)
[Verbatim outcome phrases organized by theme. What success looks like
in their words. What they're trying to become.]

## What They've Tried
[Patterns across what they've already attempted. What worked, what didn't,
what they're skeptical of now because of past attempts.]

## Identity Markers
[How they describe themselves. What they identify as. What they reject.
The role they're trying to grow into vs the role they're stuck in.]

## Psychological Profile

### Cognitive Style
[How this avatar thinks: story-driven, principle-driven, evidence-driven,
intuition-driven? What shape do their explanations take?]

### Emotional Register
[Clinical to warm to fierce. What animates them, what silences them.]

### Authority Orientation
[Told, asked, or shown? How do they establish their own credibility?]

### Pacing and Rhythm
[Long discursive or short punchy? Build to climax or front-load?
Repeat or move on?]

### Distinctive Vocabulary
[Words they reach for that most don't. Words they avoid.
Recurring metaphors. Filler patterns.]

### Belief Topology
[What they treat as obvious. What they refuse to accept.
Relationship to mainstream wisdom: amplify, complicate, invert?]

### Decision Signals
[What they need to see, feel, or hear before yes. Recurring objections.
What builds confidence, what kills it.]

## Voice Signature
[The 5-10 phrases that capture how this avatar actually talks.
The specific lines for headlines, ads, sales copy.]

## What's Still Unclear
[Gaps in the profile. What to listen for in upcoming conversations.]

---
Use this to serve them better, not against them.
```

