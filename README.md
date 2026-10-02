# agent-skills
Reusable AI agent skills, templates, and workflows in the open [Agent Skills format](https://agentskills.io/specification).

Each skill is a folder with a `SKILL.md` entry point and any supporting references. The instructions are plain Markdown with a small YAML header describing the skill. No vendor-specific configuration or plugin is required for the skills in this repository.

## Available skills

| Skill | Purpose |
| --- | --- |
| [weekly-engineering-update](skills/weekly-engineering-update/SKILL.md) | Turn engineering notes into a weekly manager update with observations, focus areas, outcomes, risks, next steps, and a two-entry summary. |

## Use a skill

Download or clone this repository, then copy the **whole skill folder**, including its references, into a location supported by your agent:

| Agent | For one project | For all your projects |
| --- | --- | --- |
| Codex | `.agents/skills/weekly-engineering-update/` | `~/.agents/skills/weekly-engineering-update/` |
| GitHub Copilot | `.github/skills/weekly-engineering-update/` | `~/.copilot/skills/weekly-engineering-update/` |

Here, `~` means your home folder. Current Codex and Copilot documentation also lists `.agents/skills/` and `~/.agents/skills/` as shared locations, so one copy can serve both agents. Choose one location per scope to avoid duplicate installations. Copilot support depends on the client; see the linked documentation below.

The `skills/` directory in this repository is the source collection. Cloning it alone does not install the skills into an agent's discovery location.

Then ask your agent, for example:

> Use the weekly-engineering-update skill to draft my update to Alex for the week of 21 September 2026. Here are my notes: ...

For an assistant without native skill support, provide `SKILL.md` and its linked reference files in the conversation and ask it to follow them. File access and automatic discovery vary by assistant.

## Weekly update defaults

The exported skill preserves the original six-section format, status markers, candid voice, and two-entry risk/progress summary. It deliberately retains the heading `Focus Areas Passed Week`; ask for different wording if preferred.

Supply the recipient, reporting period, and current notes. The recipient is configurable, and missing information is never treated as proof of success or absence of risk. The [fictional example](skills/weekly-engineering-update/references/fictional-example.md) shows the expected result.

This portable edition omits personal Teams conversation identifiers, historical message links, local machine paths, and Codex UI metadata. It uses ordinary Markdown output and needs no connector when the supplied notes are sufficient. Generating a draft does not send it.

## Format and installation references

- [Agent Skills specification](https://agentskills.io/specification)
- [Codex skill discovery and usage](https://learn.chatgpt.com/docs/build-skills)
- [GitHub Copilot skill installation](https://docs.github.com/en/copilot/how-tos/copilot-on-github/customize-copilot/customize-cloud-agent/add-skills)
