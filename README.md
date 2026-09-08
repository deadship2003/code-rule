# code-rule — LIF Guidelines Library

A numbered engineering-guidelines library ("LIF" entries) that governs
all IT development work in this account's projects — any language,
platform, domain, or artifact.

## How it loads

The library is deployed at `~/.claude/rules/` and auto-loads into every
Claude Code session through a two-level import chain:

```
~/.claude/CLAUDE.md  →  @rules/LIF.md (index)  →  @rules/LIF-00N.md (entries)
```

The index file carries the library constitution (append procedure,
status marks, structure) and the Numbering History table; each entry
lives in its own file, imported individually in numbering order.

## Entries

| # | Guideline | Tier |
|---|---|---|
| LIF-001 | All text in English | Process · universal coding |
| LIF-002 | Design alternative selection and change confirmation | Process · development phase |
| LIF-003 | Major hazardous operations require prior consent | Process · runtime phase |
| LIF-004 | Git commit identity | Process · universal commits |
| LIF-005 | Unified CLI syntax and interaction standard | Technical · universal CLI |
| LIF-006 | Built-in service lifecycle CLI | Technical · service lifecycle |
| LIF-007 | Global debug flag `--debug` | Technical · personal enhancement (optional) |
| LIF-008 | Unified project build and environment script standard | Technical · engineering build |

Process standards (001–004) govern how work is done; technical
standards (005–008) are ordered by dependency — LIF-005 is the global
CLI law, LIF-006 implements it for service programs, LIF-007 is its
optional debug-enhancement layer, LIF-008 governs repository build
machinery and defers its build.sh interface to LIF-005.

## Maintenance

- Append a new guideline: numbers increment (LIF-009, LIF-010…) —
  create `LIF-00N.md` (Origin + Scope + Implementation Rules), add its
  import line to `LIF.md`, register it in the Numbering History table.
- Every entry records a one-line Origin (provenance of the source
  requirement); full verbatim history of pre-reorganization wording
  lives in local backups.
- Any renumbering must be registered in the Numbering History table;
  old references convert via the table.
