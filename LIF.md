# LIF Guidelines Library (numbered guidelines, globally auto-loaded)

> This file is the library index, imported by ~/.claude/CLAUDE.md via
> @import; it in turn imports each entry file individually. Effective
> for ALL IT development projects — any language, platform, domain, or
> artifact — and all sessions. Text generated or modified by Claude
> follows this library equally.
> Layout: one entry per file (LIF-001.md … LIF-008.md in this
> directory), imported below in numbering order. Each entry contains:
> Origin (one-line provenance of the source requirement) + Scope +
> Implementation Rules. Status marks: [Effective YYYY-MM-DD] / [Draft] /
> [Retired YYYY-MM-DD, reason].
> Appending guidelines: numbers increment (LIF-009, LIF-010…) — create
> a new LIF-00N.md in this directory containing the entry, add its
> import line to the Entries section below, and register it in the
> Numbering History table.
> Structure: LIF-001~004 Process Standards (001 = universal coding
> language, 002 = development phase, 003 = runtime phase, 004 = universal
> commits); LIF-005~008 Technical Standards in dependency order (005 =
> universal CLI, 006 = service lifecycle, 007 = debug enhancement,
> 008 = engineering build).
> 2026-09-07: library created alongside the CLAUDE.md @import; rewritten
> in pure English (user-confirmed), Chinese originals retired — snapshots
> in ~/.claude/backups/LIF.md.bak-*.
> 2026-09-08: full reorganization per user instruction (applicable to
> all IT development projects) — every entry rewritten as a clean English
> distillation of its complete revision history (all requirements
> preserved, nothing normative dropped), entries renumbered into the
> dependency order above, verbatim original quote blocks replaced by
> one-line Origins (full pre-reorganization text preserved in backups,
> snapshot LIF.md.bak-20260908-115528). Mapping registered in the
> Numbering History table.
> 2026-09-08 (2nd): split into one file per entry — this file became the
> index and imports the entry files (import depth 2, within the 5-hop
> limit); entry content unchanged (snapshot of the single-file version:
> LIF.md.bak-20260908-120342-presplit).
> Any reorganization / renumbering must be registered in the Numbering
> History table; old references convert via the table.

## Numbering History

| Current (2026-09-08) | 2026-09-07 numbering | Original | Guideline | Tier |
|---|---|---|---|---|
| LIF-001 | LIF-007 | — (new 2026-09-07) | All text in English | Process · universal coding |
| LIF-002 | LIF-003 | LIF-004 | Design alternative selection and change confirmation | Process · development phase |
| LIF-003 | LIF-004 | LIF-003 | Major hazardous operations require prior consent | Process · runtime phase |
| LIF-004 | LIF-005 | LIF-002 | Git commit identity | Process · universal commits |
| LIF-005 | LIF-008 | — (new 2026-09-08) | Unified CLI syntax and interaction standard | Technical · universal CLI |
| LIF-006 | LIF-001 | LIF-001 | Built-in service lifecycle CLI | Technical · service lifecycle |
| LIF-007 | LIF-002 | LIF-005 | Global debug flag --debug | Technical · personal enhancement (optional, non-standard) |
| LIF-008 | LIF-006 | BLD-001 (draft name, never activated) | Unified project build and environment script standard | Technical · engineering build |

## Entries (imported individually, in numbering order)

@/home/xx/.claude/rules/LIF-001.md

@/home/xx/.claude/rules/LIF-002.md

@/home/xx/.claude/rules/LIF-003.md

@/home/xx/.claude/rules/LIF-004.md

@/home/xx/.claude/rules/LIF-005.md

@/home/xx/.claude/rules/LIF-006.md

@/home/xx/.claude/rules/LIF-007.md

@/home/xx/.claude/rules/LIF-008.md
