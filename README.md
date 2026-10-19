# Skillvize Free Skills

A small collection of free [Agent Skills](https://agentskills.io) (`SKILL.md` folders) from the Skillvize Team. They work with Claude Code, Cursor, and other agents that support the SKILL.md format.

They come from the free starter catalog on [Skillvize](https://www.skillvize.com), a marketplace where you can find, download, and sell agent skills.

## Skills

| Skill | What it does | On Skillvize |
|---|---|---|
| [code-review-companion](./code-review-companion/SKILL.md) | Paste in a diff and get a structured review: bugs, edge cases, naming, and the one thing worth fixing before merge. | [page](https://www.skillvize.com/skills/tech-code-review) |
| [bug-report-triage](./bug-report-triage/SKILL.md) | Turns a vague bug report into repro steps, a likely root-cause area, a severity call, and the info you still need. | [page](https://www.skillvize.com/skills/tech-bug-triage) |
| [error-message-explainer](./error-message-explainer/SKILL.md) | Explains a confusing error or stack trace in plain English, with the most likely cause and the first thing to try. | [page](https://www.skillvize.com/skills/tech-error-explainer) |
| [deep-research-brief](./deep-research-brief/SKILL.md) | Turns any question into a structured research brief with confidence levels, a counterargument, and a bottom line. | [page](https://www.skillvize.com/skills/research-deep-brief) |
| [meeting-notes-action-plan](./meeting-notes-action-plan/SKILL.md) | Turns messy meeting notes into decisions, owners and deadlines, open questions, and a follow-up email. | [page](https://www.skillvize.com/skills/productivity-meeting-notes) |

## Install

### Claude Code

Option 1: add this repo as a plugin marketplace.

```
/plugin marketplace add tyelf22/free-skills
/plugin install skillvize-free-skills@skillvize-free-skills
```

Option 2: copy the skill folders yourself.

```bash
git clone https://github.com/tyelf22/free-skills.git
mkdir -p ~/.claude/skills
cp -r free-skills/*/ ~/.claude/skills/
```

To install for a single project, copy the folders into `.claude/skills/` in that project instead.

### Cursor

Cursor loads Agent Skills from the `.cursor/skills/` folder in a project, or from `~/.cursor/skills/` for all projects:

```bash
git clone https://github.com/tyelf22/free-skills.git
mkdir -p .cursor/skills
cp -r free-skills/*/ .cursor/skills/
```

### Other agents

Each skill is just a folder with a `SKILL.md`. Copy it wherever your agent looks for skills.

## More skills

Browse the full catalog, or list your own skills for free, at **[www.skillvize.com](https://www.skillvize.com)**.
