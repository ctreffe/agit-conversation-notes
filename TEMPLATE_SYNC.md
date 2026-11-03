# Template synchronization state

## Comparison and adoption

- Verified source: https://github.com/ctreffe/ai-template-docs.
- Initial project provenance: [PROJECT_CONTEXT.md](PROJECT_CONTEXT.md).
- Previous full comparison: `490b57e8ef0cdef02cdc5285cd6edcc027005f6d`; later selected follow-ups were reviewed again.
- Last compared upstream commit/date: `c2ba938932f16cc67ab6d710489c662c04683a17` / 2026-11-03; exact local overlay below.
- Latest selected adoption checkpoint: `c2ba938932f16cc67ab6d710489c662c04683a17` plus local source snapshot `81aa1b1e4bb0e06e9acf560bf7d6054be0e42001b60b3a1a5efdf580a7538c00`; NOV03 outcomes independently validated on 2026-11-03.
- Fully resolved through: `c2ba938932f16cc67ab6d710489c662c04683a17` plus the identified local working-tree snapshot for the reviewed source delta and earlier applicable selections; deliberate rejections retained; no deferred/conflicting adoption item remains.
- [Pre-sync lineage, earlier selections, domain evidence and limitations](https://github.com/ctreffe/agit-conversation-notes/blob/5ac33c3ee1340ec97a83ca974a4c0e4f58f8ed2f/PROJECT_CONTEXT.md).
  No unresolved deferred/conflicting adoption item was carried from that record;
  deferred operational/domain tests remain open, not new template-adoption evidence.

## Change outcomes

All rows compare `490b57e8ef0cdef02cdc5285cd6edcc027005f6d` through `b6bb9c44ca5e403481d5153cfd5a674696159fc5` and recheck intervening selected
follow-ups. Applied outcomes are supported by the validation checkpoint below.

| Change ID | Source path/concept | Outcome | Local application or reason | Next review condition |
| --- | --- | --- | --- | --- |
| SYNC-001 | `.gitignore` | adapted | Selected source delta applied with local project rules preserved, or already present from earlier recorded follow-ups. | Next source delta or changed local rule. |
| SYNC-002 | `AGENTS.md` | adapted | Selected source delta applied with local project rules preserved, or already present from earlier recorded follow-ups. | Next source delta or changed local rule. |
| SYNC-003 | `CHANGELOG.md` | rejected | Project identity/history and completed initialization remain authoritative; no source release metadata, source task or initialization is copied. | New initialization or a separately selected project release/scope change. |
| SYNC-004 | `COLLABORATION.md` | adapted | Selected source delta applied with local project rules preserved, or already present from earlier recorded follow-ups. | Next source delta or changed local rule. |
| SYNC-005 | `DOCS_SETUP.md` | adapted | Completed setup retained as provenance; current document-context routing added without reopening initialization. | Document addition or changed local defaults. |
| SYNC-006 | `DOCUMENTATION.md` | adapted | Selected source delta applied with local project rules preserved, or already present from earlier recorded follow-ups. | Next source delta or changed local rule. |
| SYNC-007 | `DOCUMENTATION_PROCESS.md` | adapted | Selected source delta applied with local project rules preserved, or already present from earlier recorded follow-ups. | Next source delta or changed local rule. |
| SYNC-008 | `DOCUMENTS.md` | adapted | Selected source delta applied with local project rules preserved, or already present from earlier recorded follow-ups. | Next source delta or changed local rule. |
| SYNC-009 | `PROJECT_CONTEXT.md` | adapted | Selected source delta applied with local project rules preserved, or already present from earlier recorded follow-ups. | Next source delta or changed local rule. |
| SYNC-010 | `PROJECT_SETUP.md` | rejected | Project identity/history and completed initialization remain authoritative; no source release metadata, source task or initialization is copied. | New initialization or a separately selected project release/scope change. |
| SYNC-011 | `QUARTO.md` | adapted | Selected source delta applied with local project rules preserved, or already present from earlier recorded follow-ups. | Next source delta or changed local rule. |
| SYNC-012 | `README.de.md` | adapted | Selected source delta applied with local project rules preserved, or already present from earlier recorded follow-ups. | Next source delta or changed local rule. |
| SYNC-013 | `README.md` | adapted | Selected source delta applied with local project rules preserved, or already present from earlier recorded follow-ups. | Next source delta or changed local rule. |
| SYNC-014 | `REPOSITORY.md` | adapted | Selected source delta applied with local project rules preserved, or already present from earlier recorded follow-ups. | Next source delta or changed local rule. |
| SYNC-015 | `SYNCHRONIZED_STORAGE.md` | adapted | Selected source delta applied with local project rules preserved, or already present from earlier recorded follow-ups. | Next source delta or changed local rule. |
| SYNC-016 | `TASK_HANDOFF.md` | rejected | Project identity/history and completed initialization remain authoritative; no source release metadata, source task or initialization is copied. | New initialization or a separately selected project release/scope change. |
| SYNC-017 | `TEMPLATE_SYNC.md` | adapted | Selected source delta applied with local project rules preserved, or already present from earlier recorded follow-ups. | Next source delta or changed local rule. |
| SYNC-018 | `VERSION` | rejected | Project identity/history and completed initialization remain authoritative; no source release metadata, source task or initialization is copied. | New initialization or a separately selected project release/scope change. |
| SYNC-019 | `_quarto.yml` | adapted | Selected source delta applied with local project rules preserved, or already present from earlier recorded follow-ups. | Next source delta or changed local rule. |
| SYNC-020 | `input/CATALOG.md` | adapted | Selected source delta applied with local project rules preserved, or already present from earlier recorded follow-ups. | Next source delta or changed local rule. |
| SYNC-021 | `input/README.md` | adapted | Selected source delta applied with local project rules preserved, or already present from earlier recorded follow-ups. | Next source delta or changed local rule. |
| SYNC-022 | `materials/CATALOG.md` | adapted | Selected source delta applied with local project rules preserved, or already present from earlier recorded follow-ups. | Next source delta or changed local rule. |
| SYNC-023 | `materials/README.md` | adapted | Selected source delta applied with local project rules preserved, or already present from earlier recorded follow-ups. | Next source delta or changed local rule. |
| SYNC-024 | `scripts/Test-ExternalStorage.ps1` | adapted | Selected source delta applied with local project rules preserved, or already present from earlier recorded follow-ups. | Next source delta or changed local rule. |
| SYNC-025 | `scripts/Test-ExternalStorageHelper.ps1` | adapted | Selected source delta applied with local project rules preserved, or already present from earlier recorded follow-ups. | Next source delta or changed local rule. |
| SYNC-026 | `templates/DOCUMENT_CONTEXT.md` | adapted | Selected source delta applied with local project rules preserved, or already present from earlier recorded follow-ups. | Next source delta or changed local rule. |
| SYNC-027 | `templates/RESEARCH_REPORT.md` | adapted | Selected source delta applied with local project rules preserved, or already present from earlier recorded follow-ups. | Next source delta or changed local rule. |
| SKILLS | Full active skill-directory and metadata inventory | adapted | Current ongoing skills and explicit-only question research; local boundaries retained. Retired initialization/creation skills and aliases stay absent. | Next source skill change; preserve local-only skills. |
| INIT | Source start-project/create-local-project changes | rejected | Project initialization is complete; retained setup is provenance, not an ongoing executable workflow. | Only a separately authorized new project initialization. |
| STORAGE | Existing canonical mappings/manifests | adapted | Simplified layout applies to new approved areas; no existing file, marker, manifest or host mapping migrated. | Explicit storage migration or changed access/provider decision. |

## Local adaptations and evidence

- Research is explicit-only; reports and generated data are unversioned by default.
- Existing project READMEs, version, release history, license and domain safeguards remain unchanged.
- Project context points here for synchronization state; historical observations remain labeled historical.
- No research, live cloud check, private-input render or operational/device test is implied.

At the next sync compare new changes AND every deferred/conflicting item from its
original baseline. Revisit rejected items only when their condition applies.

Existing source paths and format/visual/disclosure requirements are retained.
Shared contexts own assembly rules and next actions; the catalog owns lifecycle.
Legacy hidden authoring notes are retained for a separately selected content
update; this sync does not rewrite reader QMD or invent research provenance.
The local draft-conversation-notes skill and asset remain unchanged.
CONVERSATION_STORAGE.md overrides all generic catalog, context and storage defaults;
conversation identifiers/content never enter tracked context, catalog or handoff.

## Validation checkpoint — 2026-10-19

- 11 changed skills passed the local Test-CodexSkill.ps1 wrapper with an
  existing pinned Python/PyYAML runtime; no installation or dependency change.
- Test-ExternalStorageHelper.ps1 passed 28 synthetic assertions under each of
  PowerShell 7 and Windows PowerShell 5.1 (56 total). The 5.1 process explicitly
  imported its installed Utility module after an autoload failure; no host repair.
- 178 selected local Markdown targets checked; no broken target or
  unresolved inspected anchor. Targeted English/German guide meaning and structure
  reviewed; project README pair and content sources remain unchanged.
- YAML syntax, explicit-only research metadata, full active skill inventory,
  retired initialization absence and ignored research/mapping/catalog paths checked.
- Quarto inspect selected exactly 2 maintained QMD files; contexts were
  excluded from render inputs. No artifact render or resource-copy test was run.

Full milestone/build/render/visual/domain tests, actual cloud convergence and
receiving-device/backup checks remain outside this ordinary workflow sync.
Existing pending document/device/production evidence is not completed by these tests.

## Selected Quarto HTML sync — 2026-10-22

Compared source `b6bb9c44ca5e403481d5153cfd5a674696159fc5..c2ba938932f16cc67ab6d710489c662c04683a17`.
No earlier deferred/conflicting adoption item remains. Prior deliberate
rejections retain their review conditions; this scope does not reopen project
initialization, releases or broader source adoption.

| Change ID | Source path/concept | Outcome | Local application or reason | Next review condition |
| --- | --- | --- | --- | --- |
| QHTML-001 | `_quarto.yml` HTML embedding | adopted | Enable embedding only for generic workflow HTML; document the explicit flag for separately authorized external HTML. Retain DOCX-first review and permanent unversioned conversation storage. | Changed HTML format/resource needs. |
| QHTML-002 | `QUARTO.md` portability guidance | adapted | Selected loading-reference, detached delivery and deliberate-exception checks fit the local output/access rules. | Changed delivery or runtime dependencies. |
| QHTML-003 | Source `CHANGELOG.md` | rejected | Keep project history; add a project-owned sync entry instead of importing source release history. | Separately selected source-history need. |
| QHTML-004 | Source `TASK_HANDOFF.md` | rejected | Record this project's actual task; never import the source-template checkpoint. | Separately selected project task. |
| QHTML-SKILLS | Complete skill-directory/metadata inventory | already present | Shared metadata match; completed initialization/creation definitions stay absent; documented local skills remain. No upstream skill change. | New source skill delta or changed local method. |
| QHTML-README | Source README pairs and adapted workflow guides | already present | Source README pair unchanged across this delta; preserve project introductions and adapted guide pairs. | New source README delta or selected project change. |

### Independent evidence and limits

- Semantic comparison with the entry project configuration confirmed only the
  selected embedding addition (or the existing setting); no output scope,
  default format, hook, filter, style or PDF profile was changed.
- A fresh ignored, conversation-free static fixture used a copy of the local
  configuration with synthetic render selection/navigation and local SVG/CSS/JS.
  Effective Quarto 1.9.38 configuration and explicit HTML render passed.
  The detached HTML had no external loading refs or CSS URLs among inspected
  markup/styles; no render warnings. Existing local hooks/filters were retained.
- Technical fixture evidence: `temp/quarto-html-sync-4f09cff4/results.json`.
  No maintained reader document, actual/fictional conversation, private input,
  screenshot, external mapping or material was processed.
- A separate generic technical probe verified the documented CLI embedding
  flag without repository website inheritance; no conversation fixture was used.
- Skill/README source deltas are empty; shared local skill metadata match.
  No skill edits, installs, browser/offline checks, visual/disclosure review,
  full milestone gate, live cloud or project-content render was selected.
  Static success does not establish whole-site or dynamic runtime portability.
  Source/link review is recorded with this task; earlier domain work stays open.

## Selected synchronization — 2026-11-03

Status: completed for the selected source-workflow adoption, with the
independent focused evidence below. Operational/domain limits remain separate.

The maintainer selected the current local source with project adaptations.
Compared from `c2ba938932f16cc67ab6d710489c662c04683a17` through source HEAD `c2ba938932f16cc67ab6d710489c662c04683a17`.
The working-tree overlay is not a commit. Snapshot: `81aa1b1e4bb0e06e9acf560bf7d6054be0e42001b60b3a1a5efdf580a7538c00`.
The [portable source manifest](template-sync/2026-11-03-source.json) records its
LF-normalized hashes and complete source-delta paths. No fetch or remote
freshness claim is included.

| Change ID | Source path/concept | Outcome | Local application or reason | Review condition |
| --- | --- | --- | --- | --- |
| NOV03-001 | `.agents/skills/perform-retrospective/SKILL.md` | adapted | Verified source delta; project-specific boundaries retained. | Next source or local-rule change. |
| NOV03-002 | `.agents/skills/record-idea/SKILL.md` | adopted | Verified source delta; project-specific boundaries retained. | Next source or local-rule change. |
| NOV03-003 | `.agents/skills/record-idea/agents/openai.yaml` | adopted | Verified source delta; project-specific boundaries retained. | Next source or local-rule change. |
| NOV03-004 | `.agents/skills/start-project/SKILL.md` | rejected | Initialization is complete; retained setup stays provenance. | Next source or local-rule change. |
| NOV03-005 | `.agents/skills/sync-template/SKILL.md` | adopted | Verified source delta; project-specific boundaries retained. | Next source or local-rule change. |
| NOV03-006 | `AGENTS.md` | adapted | Project-specific ongoing guidance/catalog integration; local authority retained. | Next source or local-rule change. |
| NOV03-007 | `CHANGELOG.md` | rejected | Keep project-owned history and continuation; record this sync locally. | Next source or local-rule change. |
| NOV03-008 | `COLLABORATION.md` | adapted | Project-specific ongoing guidance/catalog integration; local authority retained. | Next source or local-rule change. |
| NOV03-009 | `IDEAS.md` | rejected | Never import source-template entries; preserve/create project-owned backlog separately. | Next source or local-rule change. |
| NOV03-010 | `PROJECT_SETUP.md` | rejected | Initialization is complete; retained setup stays provenance. | Next source or local-rule change. |
| NOV03-011 | `README.de.md` | adapted | Project-specific ongoing guidance/catalog integration; local authority retained. | Next source or local-rule change. |
| NOV03-012 | `README.md` | adapted | Project-specific ongoing guidance/catalog integration; local authority retained. | Next source or local-rule change. |
| NOV03-013 | `RETROSPECTIVE_PATHS.example.md` | adopted | Verified source delta; project-specific boundaries retained. | Next source or local-rule change. |
| NOV03-014 | `TASK_HANDOFF.md` | rejected | Keep project-owned history and continuation; record this sync locally. | Next source or local-rule change. |
| NOV03-015 | `templates/IDEAS.md` | adopted | Verified source delta; project-specific boundaries retained. | Next source or local-rule change. |
| NOV03-IDEAS | Project-owned IDEAS.md and stable IDs | adapted | New empty backlog where absent; existing entries preserved. No source-template idea import. | Clear local idea-capture request or changed ownership. |
| NOV03-INVENTORY | All skill directories and invocation metadata | adapted | Preserve local-only/project-owned methods; completed creation/initialization definitions stay absent. | New source/local skill delta. |

No earlier deferred/conflicting adoption item was found in the current ledger.
Earlier deliberate rejections remain history: source release/task/version
metadata and completed initialization are still excluded. The newly selected
project backlog changes only the old assumption that no local idea intake was
needed; template-owned entries remain rejected.

Follow CONVERSATION_STORAGE.md. Versioned ideas and retrospective evidence
must remain conversation-free. Actual and fictional conversation content,
identifiers, contexts, metadata and outputs stay permanently unversioned in
approved mapped storage; never place them in IDEAS.md or a tracked transfer.
This sync grants no access to any conversation.

Operational/domain evidence and pending project work are unchanged. This sync
does not start tests, services, storage setup, data processing or publication.

### Independent validation — 2026-11-03

- 3 changed/new skills passed this project's `scripts/Test-CodexSkill.ps1`
  wrapper with the existing managed Governance Python and pinned PyYAML 6.0.3.
  No environment or package was installed.
- Full ongoing skill topology and invocation-policy comparison passed,
  preserving documented project-owned exceptions and local-only skills.
- Both focused intake/reflection source contracts passed. These are instruction
  and structural checks, not a live retrospective or automatic-routing trial.
- Markdown links: 93 local target(s) across 15 file(s).
- 2 local target(s) remain unverified by scope or access policy.
- Both README pairs retain aligned heading hierarchies; targeted bilingual
  meaning, catalog availability, role/navigation and rights were reviewed.
- Hash checks confirm the exact edit plan, preserved untargeted control files,
  unchanged existing idea entries, retained project continuation and local-only
  skills. HEAD, branch, worktree list and empty staging stayed unchanged.

No real/sensitive data, conversation, catalog contents, private mapping or
operational state was inspected. No real initialization, storage setup, runtime
test, installation, cloud operation, publication or protected Git action ran.
Full project/domain/release/milestone and family gates were not run except the
explicitly required static local gate above. Existing operational evidence gaps
remain project-owned and are not adoption blockers for these source methods.
No selected source-workflow implementation remains.
