# meeting-engine

> 🇰🇷 [한국어 README](./README.ko.md)

**A full-lifecycle meeting engine that designs agendas, facilitates decisions, extracts action items, and diagnoses meeting dysfunction — grounded in behavioral science and facilitation research.**

## Prerequisites

- **Claude Cowork or Claude Code** environment

## Goal

Most meetings fail not because people are lazy, but because the structure is wrong. This skill replaces gut-feel meeting design with research-backed protocols — from Kaner's Diamond of Participation to Kahneman's Decision Hygiene — ensuring every meeting has the right decision framework, defenses against group pathology, and a facilitation pattern matched to the situation.

## When & How to Use

Triggers automatically when you mention meetings, agendas, facilitation, or meeting minutes. Three modes: **Design** (before a meeting), **Review** (after a meeting — structuring notes into minutes), and **System** (diagnosing recurring meeting dysfunction). Say things like "내일 이사회 아젠다 짜줘" or "회의록 정리해줘" or "주간회의가 비효율적이야".

## Use Cases

| Scenario | Prompt | What Happens |
|---|---|---|
| Board meeting prep | `"내일 이사회 아젠다 짜줘"` | Screens for group pathology risks, selects optimal decision framework (RAPID/Consent/Advice Process), designs timed agenda with facilitation script |
| Meeting notes cleanup | `"회의 노트 정리해줘"` | Structures raw notes into decisions, action items (Who+What+When), parking lot, and discussion summary |
| Recurring meeting audit | `"주간회의가 비효율적이야"` | Diagnoses which of 7 inefficiency patterns apply, matches to behavioral science root causes, prescribes structural fixes |

## Key Features

- **Group Pathology Screening** — Mandatory pre-design check for 7 behavioral risks (Groupthink, Abilene Paradox, Production Blocking, Social Loafing, Anchoring, Status Effects, Noise)
- **Decision Framework Selection** — Routes to optimal framework: RAPID, Sociocracy Consent, Advice Process, Amazon Silent Reading, Toyota Nemawashi, or Bridgewater Transparency
- **Facilitation Pattern Routing** — Matches situation to Kaner's Diamond phases, Liberating Structures (33 microstructures), or ToP ORID model
- **Hub+Spoke Architecture** — Lean SKILL.md hub with 4 deep reference files loaded on demand

## Works With

- **[ceo-pipeline](https://github.com/jasonnamii/ceo-pipeline)** — Roadmap milestones feed into progress review agendas
- **[metric-tracker](https://github.com/jasonnamii/metric-tracker)** — Dashboard metrics integrated into review meetings
- **[risk-radar](https://github.com/jasonnamii/risk-radar)** — Risk review meeting agendas auto-generated
- **[management-skill](https://github.com/jasonnamii/management-skill)** — Execution system meeting protocols

## Installation

```bash
git clone https://github.com/jasonnamii/meeting-engine.git ~/.claude/skills/meeting-engine
```

## Update

```bash
cd ~/.claude/skills/meeting-engine && git pull
```

Skills placed in `~/.claude/skills/` are automatically available in Claude Code and Cowork sessions.

## Part of Cowork Skills

This is one of 25+ custom skills. See the full catalog: [github.com/jasonnamii/cowork-skills](https://github.com/jasonnamii/cowork-skills)

## License

MIT License — feel free to use, modify, and share.
