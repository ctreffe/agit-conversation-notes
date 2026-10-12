# Project Context

## Identity and initialization

- Project: AGIT Conversation Notes; repository: agit-conversation-notes.
- Repository URL: https://github.com/ctreffe/agit-conversation-notes.
- Maintainer: Christian Treffenstaedt (existing license notice retained).
- Role: derived working project, not source-template maintenance.
- Initialization: completed on 2026-10-13; configured starting 2026-10-12.
  Both adapted skills passed the required validator; final cleanup completed.
- Source template: AI Documentation Template; inherited VERSION: 0.7.0 plus
  inherited Unreleased changes.
- Verified imported snapshot / initial synchronization baseline:
  7af11ba2d132334baa9949666ae9391146649872 (this repository's initial commit).
  The upstream template commit was not supplied and cannot be inferred from
  this fresh initial commit. Verify it before upstream synchronization.
- Last harmonization / collaboration retrospective: not performed.
- Source-template and Governance clone mappings: Unset in ignored
  RETROSPECTIVE_PATHS.local.md; no clone paths guessed or searched.
- Intentional deviation: every conversation file, including authoritative QMD,
  is permanently external and unversioned; see
  [PDR-0001](decisions/PDR-0001-external-conversation-files.md) and
  [CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md).
- Retained initialization method: [PROJECT_SETUP.md](PROJECT_SETUP.md).

## Purpose, audience and language

AI-assisted workflow for turning speaker-attributed transcripts into structured
conversation notes, with Quarto outputs and traceable document revision.
Recordings are made with colleagues' consent and transcribed by university
Whisper-v3 into speaker-attributed JSON. Recognition and attribution can be wrong.

The intended document is a detailed thematic preparation of the discussed
content, initially a personal memory aid. It does not report who said what.
Source references enable verification without a speaker-by-speaker narrative.
Names matter only where content needs them, such as a confirmed assignment.
Default document language: German. Repository introductions and guides remain
an English/German pair; conversation documents need no bilingual copies.

## Scope and planned capability

- In scope: rules, generic tooling/templates and workflow documentation for
  external transcript -> external QMD -> external DOCX review -> corrected QMD.
- Planned draft-conversation-notes: thematic synthesis; distinguish results,
  decisions, tasks and open questions; link relevant transcript evidence; mark
  uncertainties. Proposals are not decisions; absent facts are not invented.
  This skill is not implemented or available for invocation.
- Deferred: protocol schema, JSON variants, evidence granularity, drafting
  method, review trace format and specific conversation access.
- Non-goals: recording/transcription service, automatic speaker correction,
  shared participant review, real-content processing during initialization,
  publication, automatic transmission and sync setup. Installations require
  separate approval; the local validator setup received that approval.

## Storage, access and source authority

[CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md) overrides inherited placement,
promotion and versioning defaults for all conversation files, including fictional
fixtures. Concrete paths use ignored CONVERSATION_PATHS.local.md; roots remain
Unset. No external storage locations were created, enumerated or inspected.

The maintainer considers intended transcripts non-sensitive. Exact access still
needs selection before processing. Sharing, publication and transmission remain
separate decisions. No real files are currently authorized. Project catalogs,
handoffs, changelogs and Decision Records contain no concrete conversation
content or metadata. External QMD remains authoritative without Git history.
External baselines and review decisions provide traceability; backup/recovery
arrangements are deferred to storage setup.

## First useful outcome and roadmap

- Generic initial contract: [DOCUMENTS.md](DOCUMENTS.md), DOC-0001.
- Next: jointly design draft-conversation-notes and protocol schema.
- First trial: small fictional transcript externally stored, reviewed thematic
  structure, external QMD, external DOCX, one maintainer correction returned to
  QMD and re-rendered. No real conversation is needed.
- Success: faithful content and references, correct uncertainty/decision
  handling, all files external and absent from Git, accepted correction present
  in QMD and subsequent DOCX with external trace.
- Trial: planned, not performed. No versioned milestone completed.

## Quarto and feedback model

- Repository _quarto.yml: optional workflow-documentation website only;
  docs/ contains no conversations, HTML uses ignored output/html/.
- Conversation model: separate external standalone QMD or external project;
  initially DOCX, optional PDF/HTML deferred. Repository website configuration
  must never control conversation rendering.
- Verified runtime: Quarto 1.9.38 and its Pandoc 3.8.3.
- Plain QMD -> DOCX needs no R, Python or TeX. PDF toolchain deferred.
- Skill validation: approved ignored clone .venv, Python 3.12.14 and PyYAML 6.0.3
  from requirements-tools.txt. Both adapted skills passed Test-CodexSkill.ps1.
  No global Python changes; later installations still require separate authority.
- Review: maintainer DOCX comments/Track Changes returned to external QMD.
  Ambiguous or external feedback requires decisions.
- Baseline/ledger stays outside Git; project status is generic only.
- No current review file, validated render or visual inspection.

## Current checkpoint and continuation

Initialization contracts and both bilingual introduction/guide pairs are complete.
Inherited histories were replaced with project-owned CHANGELOG/TASK_HANDOFF.
The inherited one-time initialization/creation skills and template backlog were
removed. Subsequent bounded work uses start-task and the current project handoff.

Checks: required skill validator passed; local navigation, YAML and invocation
policies checked; Quarto inspect selects only the two generic workflow pages;
local mappings are ignored and Unset. No conversation artifacts were created.

Next: jointly design skill/schema, then select external destinations and scoped
access/write authority for the fictional trial. Verify the upstream template
commit before later sync. Sync setup, backup and actual DOCX round-trip remain
unperformed. No Git writes or publication occurred.
