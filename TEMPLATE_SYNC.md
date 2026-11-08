# Template synchronization state

## Sync-state storage

TEMPLATE_SYNC.md is the sole durable owner of source revisions, baseline/overlay
evidence, selected outcomes and reconsideration conditions. Keep that evidence
here, including the source snapshots below. Do not create a template-sync/
directory or separate JSON manifest in this project. Temporary comparison work
is disposable and must not be required to reconstruct the recorded sync state.
This storage correction changes no adoption checkpoint or project authority.

## Comparison and adoption

- Verified source: https://github.com/ctreffe/ai-template-docs.
- Initial project provenance: [PROJECT_CONTEXT.md](PROJECT_CONTEXT.md).
- Previous full comparison: `490b57e8ef0cdef02cdc5285cd6edcc027005f6d`; later selected follow-ups were reviewed again.
- Last compared upstream commit/date: `95b7cf2f18f059875f6bbe8dc50b477b94a6e937` / 2026-11-08; clean local source.
- Latest selected adoption checkpoint: `95b7cf2f18f059875f6bbe8dc50b477b94a6e937`; NOV08 selected workflow/output methods independently validated on 2026-11-08.
- Fully resolved through: `95b7cf2f18f059875f6bbe8dc50b477b94a6e937` for compared source changes, adopted/adapted or deliberately rejected below; no deferred/conflicting adoption item remains.
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
The [source snapshot 2026-11-03](#source-snapshot-2026-11-03) records its
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

## Selected synchronization — 2026-11-08

Status: completed for the maintainer-selected workflow and output-layout package.

The comparison covers the previous commit plus its exact 2026-11-03 overlay
through clean AI Documentation Template 0.9.0 at
`95b7cf2f18f059875f6bbe8dc50b477b94a6e937`. The
[source snapshot 2026-11-08](#source-snapshot-2026-11-08) preserves baseline and
per-path source evidence. Earlier ledger sections are historical; deliberate
rejections resolve their deltas without adopting them. No remote freshness is claimed.

| Change ID | Source path/concept | Outcome | Local application or reason | Next review condition |
| --- | --- | --- | --- | --- |
| NOV08-001 | `.agents/skills/commit-changes/SKILL.md` | adopted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-002 | `.agents/skills/commit-milestone/SKILL.md` | adopted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-003 | `.agents/skills/manage-codex-config/SKILL.md` | adapted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-004 | `.agents/skills/manage-codex-config/agents/openai.yaml` | adopted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-005 | `.agents/skills/manage-restricted-storage/SKILL.md` | adapted | Explicit ongoing protection/config workflow; remove completed initialization route and preserve conversation-specific mapping/access gates. No active profile change. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-006 | `.agents/skills/manage-restricted-storage/agents/openai.yaml` | adopted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-007 | `.agents/skills/manage-restricted-storage/assets/native_git_ssh.cs` | adopted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-008 | `.agents/skills/manage-restricted-storage/references/codex-permissions.md` | adopted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-009 | `.agents/skills/manage-restricted-storage/references/profile-usability.md` | adopted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-010 | `.agents/skills/perform-retrospective/SKILL.md` | adapted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-011 | `.agents/skills/record-decision/SKILL.md` | adopted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-012 | `.agents/skills/reuse-fixes/SKILL.md` | adopted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-013 | `.agents/skills/review-project/SKILL.md` | adopted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-014 | `.agents/skills/start-project/SKILL.md` | rejected | Preserve project identity/history, private domain boundary and completed initialization; no source release/task/idea/setup import. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-015 | `.agents/skills/sync-template/SKILL.md` | adopted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-016 | `.gitignore` | adapted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-017 | `AGENTS.md` | adapted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-018 | `CHANGELOG.md` | rejected | Preserve project identity/history, private domain boundary and completed initialization; no source release/task/idea/setup import. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-019 | `CODEX_CONFIGURATION.md` | adapted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-020 | `COLLABORATION.md` | adapted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-021 | `COMMIT_PACKAGES.md` | adopted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-022 | `DOCS_SETUP.md` | adapted | Generic workflow website uses output/website; mapped document outputs keep selected formats together, DOCX first. No conversation config is inherited from the website. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-023 | `DOCUMENTATION_PROCESS.md` | adapted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-024 | `FEEDBACK_WORKFLOW.md` | adapted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-025 | `GIT_TRANSPORT.md` | adopted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-026 | `PHILOSOPHY.md` | adopted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-027 | `PROJECT_CONTEXT.md` | rejected | Preserve project identity/history, private domain boundary and completed initialization; no source release/task/idea/setup import. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-028 | `PROJECT_SETUP.md` | rejected | Preserve project identity/history, private domain boundary and completed initialization; no source release/task/idea/setup import. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-029 | `QUARTO.md` | adapted | Generic workflow website uses output/website; mapped document outputs keep selected formats together, DOCX first. No conversation config is inherited from the website. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-030 | `README.de.md` | adapted | Mapped to TEMPLATE_README.de.md; local workflow identity, attribution, skill inventory and unversioned boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-031 | `README.md` | adapted | Mapped to TEMPLATE_README.md; local workflow identity, attribution, skill inventory and unversioned boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-032 | `REPOSITORY.md` | adapted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-033 | `STYLE_GUIDE.md` | adapted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-034 | `SYNCHRONIZED_STORAGE.md` | adapted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-035 | `TASK_HANDOFF.md` | rejected | Preserve project identity/history, private domain boundary and completed initialization; no source release/task/idea/setup import. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-036 | `VERSION` | rejected | Preserve project identity/history, private domain boundary and completed initialization; no source release/task/idea/setup import. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-037 | `_quarto.yml` | adapted | Generic workflow website uses output/website; mapped document outputs keep selected formats together, DOCX first. No conversation config is inherited from the website. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-038 | `input/README.md` | adopted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-039 | `output/README.md` | adapted | Generic workflow website uses output/website; mapped document outputs keep selected formats together, DOCX first. No conversation config is inherited from the website. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-040 | `review/README.md` | adopted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-041 | `temp/README.md` | adapted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-042 | `templates/DOCUMENT_CONTEXT.md` | adapted | Selected ongoing method; local authority and permanent conversation boundary retained. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-043 | `.agents/skills/record-idea/SKILL.md` | already present | Unchanged from the previously adopted source overlay. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-044 | `.agents/skills/record-idea/agents/openai.yaml` | already present | Unchanged from the previously adopted source overlay. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-045 | `IDEAS.md` | already present | Unchanged from the previously adopted source overlay. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-046 | `RETROSPECTIVE_PATHS.example.md` | already present | Unchanged from the previously adopted source overlay. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-047 | `templates/IDEAS.md` | already present | Unchanged from the previously adopted source overlay. | Next source delta or changed local rule; initialization remains separately selected. |
| NOV08-LOCAL | Storage contract, mapping example, render skill, generic context, README pair and ADR-0001 | adapted | Document-based output and companion preservation within existing mappings; permanent unversioned conversation boundary and exact file selection retained. | Selected new document/format/storage change. |
| NOV08-INVENTORY | Active skills and invocation metadata | adapted | 23 ongoing skills including preserved local draft-conversation-notes; two new config/storage methods; no retired initialization/creation aliases. | Changed source/local skills. |

### Project adaptation and migration boundary

[ADR-0001](decisions/ADR-0001-document-output-layout.md) records the generic
layout. Repository website output uses output/website/ as a complete site tree.
No prior configured website output tree existed to relocate. Conversation outputs
follow [CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md), not repository defaults:
mapped document folders keep DOCX and selected companions together. Use --no-clean
for shared destinations or isolated mapped staging, with collision/preservation checks.

The maintainer separately selected the concrete existing-output moves and related
private path updates. That bounded migration passed byte/hash and path readback
checks. Concrete names, selections, paths, hashes and original metadata backups
remain only in approved mapped unversioned storage. No conversation content was
opened, rendered, revised or copied into versioned project or Governance files.
Original sources and returned reviews were not selected. Remote synchronization
and receiving-device convergence were not checked; no review round-trip is closed.

PDR-0002 and local drafting/revision/clarification rules remain authoritative.
The local draft skill and asset are unchanged. Actual Codex configuration,
generic QMD pages, document lifecycle, ideas, version and changelog retain their
hashes. New settings/transport/storage guides activate no profile, native adapter
or host setting and grant no additional file access. Initialization stays complete.

### Independent validation — 2026-11-08

- Ten changed/new skills passed this project's Test-CodexSkill.ps1 using the
  existing Governance-managed Python/PyYAML 6.0.3; no installation.
- Full inventory: 23 active skills, with 17 source YAML files and five intentional
  source metadata omissions matching upstream; the local drafting skill and its
  metadata/asset retain their prior hashes. Unselected skill files are preserved.
- Both README language pairs have aligned headings and reviewed bilingual changes;
  both guides name the complete local skill inventory. Source/meaning review
  retained personal thematic recall, DOCX-first review and permanent Git exclusion.
- Pre-checkpoint link review passed 235 permitted local targets/anchors; eleven
  mapped/source/output/review references remain outside that generic link check.
  All 45 implementation files match reviewed candidates; seven selected generic
  source/catalog/history/config files retain their hashes.
- Isolated conversation-free probes rendered the bilingual website into its new
  complete tree, excluded internal context and preserved an unrelated output.
  Standalone DOCX followed by embedded HTML in one document folder preserved the
  earlier DOCX and another companion. No render warnings or dependency installation.
  These probes contained no actual or fictional conversation and did not use private mappings.
- Authorized private migration was checked separately within its exact selected
  scope; ignored/untracked placement, canonical paths, collision checks, byte
  preservation and updated reference readback passed. No protected Git action.

Final ledger/manifest/handoff receive focused readback and link verification.
Real/fictional conversation rendering, content or visual review, cloud/provider
qualification, native adapter execution, full suites, whitespace and family/milestone
gates were not required or run. Domain trial and remote-convergence evidence remain
open with their existing owners. No selected synchronization implementation remains.

## Source snapshot 2026-11-03

Source evidence retained in this ledger; no separate manifest is required.

| Field | Value |
| --- | --- |
| `source_repository` | ai-template-docs |
| `source_head` | c2ba938932f16cc67ab6d710489c662c04683a17 |
| `compared_from` | c2ba938932f16cc67ab6d710489c662c04683a17 |
| `source_snapshot_sha256` | 81aa1b1e4bb0e06e9acf560bf7d6054be0e42001b60b3a1a5efdf580a7538c00 |
| `hash_convention` | SHA-256 of UTF-8 text without BOM, CRLF normalized to LF |
| `note` | Local source snapshot; no remote freshness, commit or release is implied. |

### source working tree overlay

| Source path | SHA-256 / value |
| --- | --- |
| `.agents/skills/perform-retrospective/SKILL.md` | `2417a9ca381591e781a4dde2619a6dce8dd73dcfbdd8961b1be32840cce59a59` |
| `.agents/skills/record-idea/SKILL.md` | `16de4530e130945ce6a85e8aadcff4ff4f86fabc220046e25b1b443238848a8e` |
| `.agents/skills/record-idea/agents/openai.yaml` | `8619a54e8c098122a7f3881394f84ca89b684366e848233a29ad18b6ec363935` |
| `.agents/skills/start-project/SKILL.md` | `46b2e96efc4a149bac8ae277bfad58f891a065d5bc6ac738a7d40f858f509cf1` |
| `.agents/skills/sync-template/SKILL.md` | `3183117c9369bebf52f44f4c057de3cd6579d04ba2441106b7b339773fd5a719` |
| `AGENTS.md` | `894d917d9dc825c286c686f130a100554e265e822685a57d32d2ef429c56bb1f` |
| `CHANGELOG.md` | `74da2c1a010373ce2b8a10eb8f940253c085322353d04c244b65a9ed0bd90d7d` |
| `COLLABORATION.md` | `b466ca0791168ec0cad2c2765d4c525f0e753636c85506190ecc488455e94e73` |
| `IDEAS.md` | `6849ab2479317c78948d3de1ca1b5e85e3f2adb4b65297580aa62f48c0687c71` |
| `PROJECT_SETUP.md` | `6a10db95bc03c486c251a3f42db6f27a191931b3e4ff0c291b4cdeb4b47945c5` |
| `README.de.md` | `2d9b4e3d0a02865bd8bf57745fb20387820759e6953558bce15dae24234af49f` |
| `README.md` | `7c56d743113a9573005cd7b81af4e3cc786bf7590da07c689e2e4bbc35ece47e` |
| `RETROSPECTIVE_PATHS.example.md` | `c50e5eb14db0e60dcef596d540f793b6d0daa19277889b0a95bc0568803aef25` |
| `TASK_HANDOFF.md` | `652aae316d8b26459bfa794ee28c5cf2352bb80f48310b19f37456811aba84a9` |
| `templates/IDEAS.md` | `ec31f539adfe732b7f0592e78e82801897addcb75a396d42a2f733e4e6988a6b` |

### source delta

| Order | Source path / value |
| --- | --- |
| 1 | `.agents/skills/perform-retrospective/SKILL.md` |
| 2 | `.agents/skills/record-idea/SKILL.md` |
| 3 | `.agents/skills/record-idea/agents/openai.yaml` |
| 4 | `.agents/skills/start-project/SKILL.md` |
| 5 | `.agents/skills/sync-template/SKILL.md` |
| 6 | `AGENTS.md` |
| 7 | `CHANGELOG.md` |
| 8 | `COLLABORATION.md` |
| 9 | `IDEAS.md` |
| 10 | `PROJECT_SETUP.md` |
| 11 | `README.de.md` |
| 12 | `README.md` |
| 13 | `RETROSPECTIVE_PATHS.example.md` |
| 14 | `TASK_HANDOFF.md` |
| 15 | `templates/IDEAS.md` |

## Source snapshot 2026-11-08

Source evidence retained in this ledger; no separate manifest is required.

| Field | Value |
| --- | --- |
| `source_repository` | ai-template-docs |
| `source_head` | 95b7cf2f18f059875f6bbe8dc50b477b94a6e937 |
| `compared_from` | c2ba938932f16cc67ab6d710489c662c04683a17 |
| `previous_source_snapshot_sha256` | 81aa1b1e4bb0e06e9acf560bf7d6054be0e42001b60b3a1a5efdf580a7538c00 |
| `previous_source_manifest` | 2026-11-03-source.json |
| `hash_convention` | SHA-256 of UTF-8 text without BOM, CRLF normalized to LF |
| `adoption_scope` | Selected generic ongoing workflows and output-layout methods; private migration evidence remains in approved unversioned storage. Local boundaries/rejections in TEMPLATE_SYNC.md. |

### source working tree overlay

None.

### source delta

| Order | Source path / value |
| --- | --- |
| 1 | `.agents/skills/commit-changes/SKILL.md` |
| 2 | `.agents/skills/commit-milestone/SKILL.md` |
| 3 | `.agents/skills/manage-codex-config/SKILL.md` |
| 4 | `.agents/skills/manage-codex-config/agents/openai.yaml` |
| 5 | `.agents/skills/manage-restricted-storage/SKILL.md` |
| 6 | `.agents/skills/manage-restricted-storage/agents/openai.yaml` |
| 7 | `.agents/skills/manage-restricted-storage/assets/native_git_ssh.cs` |
| 8 | `.agents/skills/manage-restricted-storage/references/codex-permissions.md` |
| 9 | `.agents/skills/manage-restricted-storage/references/profile-usability.md` |
| 10 | `.agents/skills/perform-retrospective/SKILL.md` |
| 11 | `.agents/skills/record-decision/SKILL.md` |
| 12 | `.agents/skills/reuse-fixes/SKILL.md` |
| 13 | `.agents/skills/review-project/SKILL.md` |
| 14 | `.agents/skills/start-project/SKILL.md` |
| 15 | `.agents/skills/sync-template/SKILL.md` |
| 16 | `.gitignore` |
| 17 | `AGENTS.md` |
| 18 | `CHANGELOG.md` |
| 19 | `CODEX_CONFIGURATION.md` |
| 20 | `COLLABORATION.md` |
| 21 | `COMMIT_PACKAGES.md` |
| 22 | `DOCS_SETUP.md` |
| 23 | `DOCUMENTATION_PROCESS.md` |
| 24 | `FEEDBACK_WORKFLOW.md` |
| 25 | `GIT_TRANSPORT.md` |
| 26 | `PHILOSOPHY.md` |
| 27 | `PROJECT_CONTEXT.md` |
| 28 | `PROJECT_SETUP.md` |
| 29 | `QUARTO.md` |
| 30 | `README.de.md` |
| 31 | `README.md` |
| 32 | `REPOSITORY.md` |
| 33 | `STYLE_GUIDE.md` |
| 34 | `SYNCHRONIZED_STORAGE.md` |
| 35 | `TASK_HANDOFF.md` |
| 36 | `VERSION` |
| 37 | `_quarto.yml` |
| 38 | `input/README.md` |
| 39 | `output/README.md` |
| 40 | `review/README.md` |
| 41 | `temp/README.md` |
| 42 | `templates/DOCUMENT_CONTEXT.md` |

### unchanged previous overlay

| Order | Source path / value |
| --- | --- |
| 1 | `.agents/skills/record-idea/SKILL.md` |
| 2 | `.agents/skills/record-idea/agents/openai.yaml` |
| 3 | `IDEAS.md` |
| 4 | `RETROSPECTIVE_PATHS.example.md` |
| 5 | `templates/IDEAS.md` |

### source path sha256

| Source path | SHA-256 / value |
| --- | --- |
| `.agents/skills/commit-changes/SKILL.md` | `6ea584a6739be55b7d10a3f99c774246753a5a3f0b9ed88f8f61acd820483a4e` |
| `.agents/skills/commit-milestone/SKILL.md` | `8f9e1a2babb004aef230d502b343ede937f53aa8d222fa37fab66089ad790168` |
| `.agents/skills/manage-codex-config/SKILL.md` | `6b7a2dc4e277b3d3faa93a239cf428ddaca6353ef5a5039eb04a3aefa91dd965` |
| `.agents/skills/manage-codex-config/agents/openai.yaml` | `8619a54e8c098122a7f3881394f84ca89b684366e848233a29ad18b6ec363935` |
| `.agents/skills/manage-restricted-storage/SKILL.md` | `c990ab58910b33d7de755195fec5e75c5c79c277cbada960801d02ddd4eff116` |
| `.agents/skills/manage-restricted-storage/agents/openai.yaml` | `a1499d95abd8447558c535fe5554adcc3c9b988a0a39264a6283d430effe1e94` |
| `.agents/skills/manage-restricted-storage/assets/native_git_ssh.cs` | `08a40b564c7ee6e09283c62981da60616f480351eb1535d9a55ca93882ad53e4` |
| `.agents/skills/manage-restricted-storage/references/codex-permissions.md` | `0a7e8610d7514fe7e771b45805e38f181f10928f28b1565595790a0714c8bb37` |
| `.agents/skills/manage-restricted-storage/references/profile-usability.md` | `d1513d6eb7c98fdde41d13ed5fc74e0c667f46e82e4249aac588b025612653b5` |
| `.agents/skills/perform-retrospective/SKILL.md` | `935591ae8061a603b93f3035de6352bbb8a224802f17903184a0c8f4cd7737ad` |
| `.agents/skills/record-decision/SKILL.md` | `df45627bbdd6563dbee2f026b10d73d43668758b8c175dd9d3bf0aaefcf90d03` |
| `.agents/skills/reuse-fixes/SKILL.md` | `62cda2017ecbb8b8514905a95a1e89694a1f44b254ab7af50169e15105f3f874` |
| `.agents/skills/review-project/SKILL.md` | `0da72ca408d5326d836f1a29f105cd1afdedff714316b8651a1968b5fa316ee6` |
| `.agents/skills/start-project/SKILL.md` | `2d408a90e8873484525c58f9cce268f9c1e954ad7b7b39e7687336fe549cfc02` |
| `.agents/skills/sync-template/SKILL.md` | `a8cf3a3e3aaf2b4cce166e4e1908582c4a184cd9166add3acee6de043a0900c2` |
| `.gitignore` | `df868ce08194674cbf88637cc70ca56f9f362f7f8fdc739f3ef4a7854a1707d8` |
| `AGENTS.md` | `ebb9bf123cfada399513ce34353dd6672656d64d45911f206e07c7cee1f00522` |
| `CHANGELOG.md` | `d38bf3c944feb8217fb0906ef8f160bfced2b0d803b44d29853746305e5d1434` |
| `CODEX_CONFIGURATION.md` | `489115c797ab47a9a87cc40f7f83bc67abe3c43d19137410ded80ce1fc86003b` |
| `COLLABORATION.md` | `972580c50d4e90e5c44e9b262aa58f095238660ed19c96ccac4023a345faaca5` |
| `COMMIT_PACKAGES.md` | `75d0dd152f4bcb034d92c9b2a060cc3ea35f30815b674ead81d712142b1270af` |
| `DOCS_SETUP.md` | `bc3227cf7e4bfc11bb85a2f078a8585b678404db57878ec53cb1ab0b58184f69` |
| `DOCUMENTATION_PROCESS.md` | `e1a18e94d09d9eeb22a8ba09529f122e19b0ddf12a2fdf288a2aa63949c95d8e` |
| `FEEDBACK_WORKFLOW.md` | `a2c34ba9efc131c6c3fbc653c184fcfcb8bf7fb82be358a0f5e6cde297a837f4` |
| `GIT_TRANSPORT.md` | `cd76ac990abae288f8082aefe4958133dfe6beae8d634e4febe29cdad38b8d46` |
| `PHILOSOPHY.md` | `554e9381241dccbb63157d8738a1d3334635efe0bdedaf9c44e797c41d3ef3d4` |
| `PROJECT_CONTEXT.md` | `18455d991cbcaaa635003550110620f896daad160016e1d04235054f8a4b6915` |
| `PROJECT_SETUP.md` | `90f353679d7d35f4f2ab98718808ee99fa4329a4fa88290c0040ba9e3cf3b54e` |
| `QUARTO.md` | `2dcf33fc551f90bf853549fba626bb320bceb368dbab1d8463bdf9af5fe877c8` |
| `README.de.md` | `83aa029781a57b7371d00d9037aaf6bb413d715153fdcdb6845db46a4315b407` |
| `README.md` | `fd1b3bc6a8dc1a5160058d2462658089ff39735a6010985f6d578313299ee7f6` |
| `REPOSITORY.md` | `ee141e05e1e9942514f9f17c1decaba0a82e8f4d66931f06c82ee76233822e8e` |
| `STYLE_GUIDE.md` | `c35a01a45f3e17c0c432c8beb6bf8d6d128bd131f8bc7a8b4e1343ce30c5b69c` |
| `SYNCHRONIZED_STORAGE.md` | `3d8920e976fddcdded8c6856b9405f51723d886ca61093e53a7c4e5e8d4b4eb5` |
| `TASK_HANDOFF.md` | `e211ada6567a753d438453f5877ea04e9678aff2c7df6cddf69ee534254c59ee` |
| `VERSION` | `6ea2814d17647b954f24c55e02c3b0c65023fc301fc5ac80cc4f4a3bf2594d9a` |
| `_quarto.yml` | `b6715a3a4c047907ebaad39fd8dc3a3c2c23396d1ef4317117e4aae26f739d43` |
| `input/README.md` | `a1942e213f48e0be31304686e8e2fff21a49059481e012d5475e030fd437dd75` |
| `output/README.md` | `d1f18ac87f439dbdf789040464383da19189f3ba760ecb8d982745df442facf9` |
| `review/README.md` | `509607342fbb5b24d2ebcf2acd089b336a476680d27fab37838618f81fa9e2ec` |
| `temp/README.md` | `87f6294445e7e02be32eb9deb2f2bf7801d6f60ffed4acf087e74ed772194902` |
| `templates/DOCUMENT_CONTEXT.md` | `01c16817be99be994daafc8dfd3727497c323579d9f7bd3b0a08d53b7bafd32e` |
| `.agents/skills/record-idea/SKILL.md` | `16de4530e130945ce6a85e8aadcff4ff4f86fabc220046e25b1b443238848a8e` |
| `.agents/skills/record-idea/agents/openai.yaml` | `8619a54e8c098122a7f3881394f84ca89b684366e848233a29ad18b6ec363935` |
| `IDEAS.md` | `6849ab2479317c78948d3de1ca1b5e85e3f2adb4b65297580aa62f48c0687c71` |
| `RETROSPECTIVE_PATHS.example.md` | `c50e5eb14db0e60dcef596d540f793b6d0daa19277889b0a95bc0568803aef25` |
| `templates/IDEAS.md` | `ec31f539adfe732b7f0592e78e82801897addcb75a396d42a2f733e4e6988a6b` |
