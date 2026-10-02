# Weekly update style guide

Use this default format unless the user explicitly requests a different one. Historical messages and the fictional example provide style only; current inputs supply the facts.

## Exact structure

Start with `Hi {recipient},` (or `Hi,` when no recipient is known), one blank line, then the level-one title. Preserve the vertical bar, emojis, wording, and capitalization shown here. Keep `Focus Areas Passed Week` exactly as written. Render headings and bold text; do not expose literal Markdown in a code block.

The following is a structural template. Braced fields are instructions to substitute, not text to leave in a draft. Repeat project and risk entries only as warranted by current notes.

```markdown
Hi {recipient},

# 📅 Weekly Update | Week of {reporting date, e.g. 21st Sep 2026}

## 👀 Key Observations

🔹 {Observation and its practical implication.}

* * *

## 🎯 Focus Areas Passed Week

1. **{Focus area}**
   * {Work or investigation that received attention.}

* * *

## 📊 Outcomes

### {status marker} {Project or topic}

{Short factual paragraph about what happened, the result, and any unresolved point.}

* * *

## 🚧 Risks & Blockers

🔴 **{Risk or blocked topic}**

* {Specific constraint and its supported consequence.}

* * *

## 🎯 Next Focus

1. **{Focus area}**
   * {Planned action.}

* * *

## 📌 Summary

⚠️ **Main risk:** {One concise sentence summarizing the leading supported risk.}

🎯 **Main progress:** {One concise sentence summarizing actual progress.}
```

## Formatting details

- Five horizontal dividers separate the six major sections. No divider is inserted between the greeting/title and observations, or between individual outcome topics.
- Observations use separate paragraphs beginning with 🔹. They can be short or contain several sentences when the situation requires explanation.
- Both focus sections use ordered lists with bold topic names and indented unordered action bullets. A topic may stand alone when the notes supply no elaboration. Use as many topics as the inputs warrant; do not invent a fixed three-item quota.
- Outcomes use level-three headings with an inline status circle followed by the topic. Detail is primarily narrative paragraphs, sometimes multiple paragraphs for a complicated topic.
- Risks normally use 🔴 followed by a bold topic name and a bullet list. Do not add a red warning when no risk was supplied.
- Status circles reflect the supplied facts: 🟢 for completed work; 🟡 for ongoing, tentative, postponed, or awaiting-alignment work; 🔴 for a substantiated blocker or unresolved issue preventing progress. A successful experiment can remain 🟡 when the wider initiative is unfinished. If status cannot be established and materially affects the message, clarify it instead of guessing.
- Use a readable date with abbreviated month and full year, retaining the title's `Week of` construction. Prefer ordinal day styling unless the user supplies an intended title/date style.
- Keep a blank line between the two summary entries. "Two-line summary" means two logical entries; automatic line wrapping is not an extra entry.
- Do not copy connector-induced line wrapping, duplicated link titles, or broken URL line breaks. Preserve actual links from current inputs in normal Markdown form.
- The destination chat app controls final fonts and rendering. Match the content formatting faithfully; do not claim control over pixels, font metrics, or client-dependent spacing.

## Voice

The messages are direct, personal, and practical. They use `I` for the author's actions or view and `we` for shared work or agreements. They explain what happened, why it matters, and what is still unresolved. They can be candid about requirements gaps, coordination, and uncertainty without becoming accusatory.

Use plain verbs such as tried, discussed, agreed, identified, reviewed, and postponed. Preserve the user's natural phrasing; fix errors only when needed for clarity. Avoid turning a simple observation into polished corporate prose. Do not add celebratory claims, executive slogans, excessive softening, a closing thank-you, or a signature. Match the information density of the supplied material rather than padding to resemble the example.
