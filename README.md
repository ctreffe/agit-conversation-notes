# AGIT Conversation Notes

> [!NOTE]
> **AI Collaboration**
>
> AI assists workflow design and project documentation. Transcript-based
> drafting and review are the intended workflow.
> [COLLABORATION.md](COLLABORATION.md) documents maintainer authority, source
> traceability, revision practices and the external-storage boundary.

[Deutsch](README.de.md)

## Workflows and Skills

The [workflow guide](TEMPLATE_README.md) describes available skills and rules.
[PROJECT_CONTEXT.md](PROJECT_CONTEXT.md) records current state. Initialization
is complete; subsequent bounded work uses start-task.

## Purpose

AI-assisted workflow for turning speaker-attributed transcripts into structured
conversation notes, with Quarto outputs and traceable document revision.
University Whisper-v3 supplies JSON from consensually recorded conversations.
Transcription and speaker labels can be wrong.

The aim is a detailed German thematic preparation of the discussed content,
initially a personal memory aid. Who said each sentence is not the organizing
principle. Transcript references support checking; names matter where needed,
such as a confirmed task assignment.

## Planned workflow

External JSON -> external QMD -> external DOCX for maintainer review -> accepted
comments/Track Changes back to authoritative QMD -> checked re-render.

The planned draft-conversation-notes skill will distinguish results, decisions,
tasks and open questions, retain evidence and mark uncertainty. Suggestions must
not become decisions, and missing information must not be invented.
Skill and protocol schema will be designed together; they are not implemented.

## Permanent storage boundary

All conversation files stay outside Git and permanently unversioned, including
JSON, derivatives, QMD, DOCX/PDF/HTML, annotated copies, traces, intermediates and
fictional trial files. External QMD remains authoritative. Git holds only skills,
scripts, generic templates, configuration and conversation-free project docs.

[CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md) defines this deliberate Docs
Template deviation. Ignored CONVERSATION_PATHS.local.md maps external roots,
currently Unset. Exact file access, outside writes, sync transmission, sharing and
publication remain separate decisions. Sync setup is deferred.

## Current state and next step

Project rules and external render/revision instructions are configured.
Quarto 1.9.38/Pandoc 3.8.3 are present. The separately approved local validator
setup provides Python 3.12.14/PyYAML 6.0.3; both adapted skills passed validation.
No real-file processing, conversation render, Git write or publication occurred.
No project version/milestone is complete.

Next jointly design the skill/schema, then test a small fictional excerpt using
external storage, DOCX review and correction transfer. The generic trial contract
is [DOCUMENTS.md](DOCUMENTS.md); tooling prerequisites are in
[DOCS_SETUP.md](DOCS_SETUP.md). Repository docs/ contains workflow guidance only.

## License

[MIT](LICENSE). Existing copyright/attribution is retained.
This repository license grants no access to or sharing of conversation files.
