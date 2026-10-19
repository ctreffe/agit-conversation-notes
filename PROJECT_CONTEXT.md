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
  is permanently unversioned and off GitHub. Mapped ignored repository storage
  is allowed; persistent files default to external sync, temporary files to
  ignored temp/conversation-work/. See
  [PDR-0002](decisions/PDR-0002-unversioned-conversation-storage.md) and
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

## Scope and available capability

- In scope: rules, generic tooling/templates and workflow documentation for
  external transcript -> external QMD -> external DOCX review -> corrected QMD.
- Available [draft-conversation-notes](.agents/skills/draft-conversation-notes/SKILL.md):
  transcript clarification and thematic QMD synthesis; distinguish results,
  decisions, tasks and open questions; link relevant transcript evidence; mark
  uncertainties. Proposals are not decisions; absent facts are not invented.
  Skill instructions and a generic QMD asset are implemented; the first
  conversation trial now has a technically checked QMD/DOCX draft in approved
  persistent external storage; review and the correction round-trip remain pending.
- Agreed method: first clarify transcript ambiguities through contextual numbered
  questions in sequential batches of at most ten; then prepare the structured
  content, with further questions where needed. Phonetically plausible corrections
  remain suggestions until clarified; preserve the original transcript unchanged.
  See [DOCUMENTATION_PROCESS.md](DOCUMENTATION_PROCESS.md) for the design contract.
- Agreed design: actual date/participants header, then flexible content-led prose,
  topics or lists preserving important arguments/reasons/alternatives. Lightly
  emphasized findings, category sections, opening/closing overviews and tables
  are optional. Use compact source footnotes; no mandatory minutes schema. See
  [DDR-0002](decisions/DDR-0002-content-led-provisional-notes.md), which supersedes
  the earlier fixed layout.
- Explanatory footnotes: condense useful specialist/internal knowledge from
  clarification answers, keeping it distinct from source evidence and preserving
  uncertainty/private provenance. See
  [DDR-0003](decisions/DDR-0003-explanatory-clarification-footnotes.md).
- Template checkpoint: provisional QMD; evaluate after the first completed test
  project and review/revise no later than the second. Zero test projects completed.
- Deferred: exact source JSON variants, available evidence locators, concrete
  external review trace format and specific conversation access.
- Non-goals: recording/transcription service, automatic speaker correction,
  shared participant review, real-content processing during initialization,
  publication and automatic transmission. Installations require
  separate approval; the local validator setup received that approval.

## Storage, access and source authority

[CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md) overrides inherited placement,
promotion and versioning defaults for all conversation files, including fictional
fixtures. Concrete paths use ignored CONVERSATION_PATHS.local.md. On 2026-10-13,
the maintainer-selected external synchronized project directory was created
with ID agit-conversation-notes, an identity marker and empty persistent folders.
The marker and selected directory availability were checked locally; remote
synchronization remains unchecked. The device-local temporary root is now mapped
to ignored repository temp/conversation-work/ following the maintainer's
clarification: physical placement within the project is allowed when permanently
excluded from versioning and GitHub. With scoped maintainer write/transmission
approval, the authoritative QMD, review DOCX and three retained revision evidence
files were copied into persistent storage and verified by SHA-256. The original
transcript remains unchanged in its supplied location; temporary processing files
remain device-local. This selected placement grants no broader transmission scope.

The maintainer considers intended transcripts non-sensitive. Exact access still
needs selection before processing. Sharing, publication and transmission remain
separate decisions and are scoped per task. Project catalogs,
handoffs, changelogs and Decision Records contain no concrete conversation
content or metadata. Selected unversioned QMD remains authoritative without Git history.
Unversioned baselines and review decisions provide traceability; backup/recovery
arrangements are deferred to storage setup.

## First useful outcome and roadmap

- Generic initial contract: [DOCUMENTS.md](DOCUMENTS.md), DOC-0001.
- Next: maintainer DOCX review, then accepted corrections returned to the
  authoritative QMD and re-rendered. Persistent and temporary roots are mapped.
- First trial: the maintainer selected an actual transcript after initialization.
  Clarification, thematic drafting, DOCX export and approved persistent placement
  are complete. One accepted correction still needs the QMD/render round-trip.
  Fictional input remains available for future generic trials but is not required.
- Success: faithful content and references, correct uncertainty/decision
  handling, all conversation files unversioned and off GitHub, accepted correction present
  in QMD and subsequent DOCX with external trace.
- Trial: drafting/export complete; annotated review and correction round-trip pending.
  No versioned milestone completed.

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
- Baseline/ledger stays unversioned; project status is generic only.
- Current trial has an externally retained authoritative QMD, DOCX, checked
  footnote links, source baseline, clarification snapshot and export ledger.
  No annotated review, correction round-trip or visual inspection.

## Current checkpoint and continuation

Initialization contracts and both bilingual introduction/guide pairs are complete.
Inherited histories were replaced with project-owned CHANGELOG/TASK_HANDOFF.
The inherited one-time initialization/creation skills and template backlog were
removed. Subsequent bounded work uses start-task and the current project handoff.

Checks: required skill validator passed; local navigation, YAML and invocation
policies checked; Quarto inspect selects only the two generic workflow pages;
local mappings are ignored. Persistent external storage and device-local ignored
repository temp/conversation-work/ are mapped. The first QMD/DOCX draft
and its unversioned revision evidence are retained externally for review;
selected copies match their local source hashes.

Next: review the DOCX and return accepted corrections to the authoritative QMD.
Verify the upstream template commit before later template sync. Selected persistent
placement is complete on this host; provider synchronization, backup and the actual DOCX
round-trip remain unverified. Initialization was committed and pushed as 4605e7a;
no publication occurred. Conversation artifacts stay unversioned. The subsequent work grants no
standing commit/push authority. The new skill passed Test-CodexSkill.ps1;
Pandoc parsed the minimal generic QMD metadata, emphasis and footnotes.
The first transcript clarification, draft/DOCX render and approved placement are complete;
preserve source/annotation baselines for the still-pending review round-trip.
