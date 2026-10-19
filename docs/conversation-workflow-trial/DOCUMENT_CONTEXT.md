# Document Context — generic conversation workflow trial

This is a conversation-free workflow contract, not a conversation instance or
fixture. [DOCUMENTS.md](../../DOCUMENTS.md) owns its planned lifecycle. Actual
conversation contexts, IDs, source versions, questions and next steps belong
exclusively in mapped unversioned storage under CONVERSATION_STORAGE.md.
No conversation content may be entered here, including fictional content.

## Generic contract and requirements

- ID: DOC-0001 identifies a generic planned trial, not a real conversation.
- Maintained source: planned external QMD beneath conversation:root/sources/;
  exact path selected locally before the trial.
- Purpose: test transcript -> QMD -> DOCX -> revised QMD.
- In scope: thematic content, source references, results, decisions, tasks,
  open questions, uncertainty, contextual transcript clarification in batches of
  at most ten numbered points before drafting, and one accepted DOCX correction.
- Out of scope: real data, speaker-by-speaker reporting, final schema during
  initialization, automatic approval, shared review and publication.
- Profile: content-led conversation summary with actual date/participants header;
  flexible headings/prose/lists, optional findings/highlights/recap and compact
  source footnotes. No compulsory minutes categories or hierarchy.
- Audience/task: inherited from PROJECT_CONTEXT.md: personal memory aid;
  verify discussed content and correct the draft.
- Language: inherited from PROJECT_CONTEXT.md: German, no bilingual source set.
- Required output: external DOCX. PDF/HTML only after deliberate selection.
- Source/access: invented excerpt, created only after external destination/write
  authorization. All files permanently unversioned and off GitHub. Mapped ignored
  repository locations are allowed; local temp/conversation-work/ holds intermediates.
- Navigation: generic contract here; no repository website page for the trial.
- Validation: content/evidence fidelity, uncertainty/decision handling, mapped
  unversioned placement and Git exclusion, contextual questions and phonetic suggestions distinguished from
  confirmed corrections, batch size/order when more than ten questions arise,
  verified or explicitly unresolved conversation metadata, content-driven
  structure without empty categories, DOCX checks, accepted edit and re-render.
  Evaluate the provisional template after the first test; revise by the second.
- Review: maintainer comments/Track Changes; external trace identifies source
  baseline, output and applied correction.
- Next action: select external storage and exact authorized trial paths, then
  exercise draft-conversation-notes and its generic QMD asset before DOCX review.
- Decision: [PDR-0002](../../decisions/PDR-0002-unversioned-conversation-storage.md).
  Current design: [DDR-0002](../../decisions/DDR-0002-content-led-provisional-notes.md).

## Assembly and update method

Follow DOCUMENTATION_PROCESS.md and the unchanged draft-conversation-notes skill:
clarify transcript ambiguities in bounded numbered batches, then create thematic
QMD from confirmed evidence while preserving uncertainty and explanatory/source
footnote distinctions. Retain actual decisions, source snapshots, review baselines
and update rules in the mapped unversioned per-conversation context/trace. Update
that context at task entry/handoff without leaking its IDs or contents to tracked
project files. All mapping, processing, disclosure and Git-exclusion gates in
CONVERSATION_STORAGE.md remain mandatory. No new trial is implied by this sync.

## Assigned sources and open work

No actual source is assigned to this generic contract. A fictional trial remains
optional; no source or output is created here. The project-wide current trial's
generic progress and remaining review/correction round-trip stay in
PROJECT_CONTEXT.md, with concrete evidence only in private unversioned trace.
