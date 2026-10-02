---
name: weekly-engineering-update
description: Draft or revise a weekly engineering update for a manager in a structured chat-message style, using notes and supplied project updates. Use for a weekly manager update or its risk/progress summary; not for ordinary chat replies, daily triage, or generic status reports.
---

# Weekly Engineering Update

Create a ready-to-paste weekly manager update for Teams or another chat channel. Follow the structure, formatting, and direct, practical voice in the reference. Use current notes for facts and historical messages only for style. A new explicit user instruction takes precedence over these defaults.

## Reference and inputs

Read [the weekly update style](references/style-guide.md) before drafting. It defines the format, voice, and status conventions. For a realistic illustration of that format, read [the fictional example](references/fictional-example.md); none of its facts belong in a real update.

Use the user's notes, supplied project updates, reporting period, and relevant links. Use the recipient and channel supplied by the user or established in the conversation. If the recipient is unknown, use "Hi," rather than inventing a name. Ask only for missing information that materially affects the message, such as an ambiguous reporting week or contradictory delivery status. When the user says "this week" or "last week", determine the period from the current date and timezone. Never copy a historical date or infer the reporting week from when an old message was sent.

No live connector is required when the supplied inputs suffice. If the user asks to gather fresh information or refresh the style, use available read tools within that request's scope. The saved style remains usable when Teams is unavailable; do not claim to have checked live messages unless that actually happened.

## Drafting

- Use the reference greeting with the actual recipient, and keep the title pattern, six section headings, heading levels, emojis, list structure, separators, and two-entry summary in the reference. In particular, preserve `Focus Areas Passed Week`; do not silently correct that heading. This specific weekly style takes precedence over generic preferences to shorten chat messages or avoid emojis.
- Map observations to implications, past focus to what received attention, outcomes to what actually happened, risks to current constraints, and next focus to intended actions. Keep separate facts separate when combining them would change certainty, ownership, or timing.
- Distinguish a discussion, experiment, proposal, agreement, completed implementation, demo, and release. Never promote one into another. A future milestone belongs in a plan or clearly qualified outcome context, not as an achievement.
- Preserve first-person judgments and caveats: "I tried", "I see", "seems", "most likely", "no consensus yet", and "we agreed to continue discussion" only when supported by the input. Keep wording plain, candid, and practical. Do not manufacture uncertainty for confirmed facts or certainty for tentative ones.
- Retain supplied names, technical terms, links, deadlines, blockers, and meaningful details. Do not import old projects, people, commitments, or risks from the reference. Do not embellish with invented metrics, owners, business impact, or promises.
- Follow the evidence-based status marker guidance in the reference. Missing information does not mean success or absence of risk. For an otherwise empty section, use a short neutral statement such as "No update provided." instead of inventing content. Ask a targeted question if the missing fact is needed to avoid a misleading message.
- End with exactly two summary entries: `⚠️ **Main risk:**` followed by `🎯 **Main progress:**`. Summarize the body without adding new claims. If no risk or progress information was provided, say so; do not assert there are no risks or recast a plan as progress.

## Output and check

Return only the ready-to-paste message as rendered Markdown. Keep formatting outside code fences. Do not add an email subject, sign-off, process notes, source appendix, or offer after the draft. Embed useful supplied links naturally in the body, as shown in the example.

Before returning, compare the draft with the reference for structure and voice; compare every achievement, uncertainty, deadline, and summary statement with the current inputs. Preserve the information density the content needs rather than imposing an arbitrary word count. Replace all illustrative fields with actual content.

If asked only to fill or revise the summary, return only the two requested entries and leave the rest untouched. If asked to revise a full draft, preserve its facts and intended emphasis while bringing its format into line with the reference.

Generating an update produces a draft. It does not authorize sending a message, scheduling a task, or updating project systems. Send only when the user explicitly requests sending in the active task.
