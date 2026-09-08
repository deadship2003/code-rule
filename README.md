# code-rule — LIF Guidelines Library

A numbered engineering-guidelines library ("LIF" entries), binding on
all IT development work in this account's projects — any language,
platform, domain, or artifact.

## How it loads

The library is deployed at `~/.claude/rules/` and auto-loads into every
Claude Code session through a two-level import chain:

```
~/.claude/CLAUDE.md  →  @rules/LIF.md (index)  →  @rules/LIF-00N.md (entries)
```

The index file carries the library constitution (binding scope,
structure, status marks, citation convention, append procedure); each
entry lives in its own file, imported individually in numbering order,
and contains only normative content (Scope + Implementation Rules +
Exemptions / Related where present). Provenance and revision history
live in git history and the tables below — never in the auto-loaded
rule text.

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

Old references convert via this table. No renumbering has occurred
since 2026-09-08.

## Library History

- 2026-09-07: library created alongside the CLAUDE.md @import;
  rewritten in pure English (user-confirmed), Chinese originals
  retired (snapshots in ~/.claude/backups/LIF.md.bak-*).
- 2026-09-08: full reorganization — every entry rewritten as a clean
  English distillation of its complete revision history (all
  requirements preserved, nothing normative dropped), entries
  renumbered into the dependency order above; mapping registered in
  the Numbering History table.
- 2026-09-08 (2nd): split into one file per entry; the index became
  an import-only file.
- 2026-09-08 (3rd): amendment pass — LIF-001 gained three scoped,
  owner-confirmed exemptions (vendored third-party trees / realistic
  test fixtures / runtime user-facing locale copy); name-first
  citation convention added; Related footers completed on all entries.
- 2026-09-08 (4th): cleaned to pure normative form — Origin provenance
  blocks, dated notes, and revision-history narratives removed from
  the auto-loaded files and preserved here and in git history; every
  requirement kept (the LIF-006 "no built-in log command" rule was
  promoted from provenance text into rule 10). No renumbering.

## Maintenance

- Append a new guideline: numbers increment (LIF-009, LIF-010…) —
  create `LIF-00N.md` (Scope + Implementation Rules), add its import
  line to `LIF.md`, register it in the Numbering History table.
- Amend an entry: edit LIF-00N.md in place, preserving all normative
  content; take a local backup snapshot first (convention:
  `~/.claude/backups/rules.bak-*`), and register the amendment in
  Library History above.
- Any renumbering must be registered in the Numbering History table;
  old references convert via the table.
- Cite entries by name first, number second (e.g. "service lifecycle
  guideline (LIF-006)") — names survive renumbering, numbers do not.
- LIF-001 carries three scoped exemptions (vendored third-party
  trees, realistic test fixtures, runtime user-facing locale copy);
  see that entry's Exemptions section.
