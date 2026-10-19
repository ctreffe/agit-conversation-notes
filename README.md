# AGIT Conversation Notes

> [!NOTE]
> **AI Collaboration**
>
> AI assists workflow design and project documentation. Transcript-based
> drafting and review are the intended workflow.
> [COLLABORATION.md](COLLABORATION.md) documents maintainer authority, source
> traceability, revision practices and the conversation versioning boundary.

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

## Workflow

External JSON -> external QMD -> external DOCX for maintainer review -> accepted
comments/Track Changes back to authoritative QMD -> checked re-render.

[draft-conversation-notes](.agents/skills/draft-conversation-notes/SKILL.md) first
clarifies transcript ambiguities with contextual numbered questions in batches
of at most ten, then prepares the German thematic QMD. Important arguments,
reasons and alternatives remain; repetitions and fillers are condensed.
Actual date and participants appear in a short header. Structure follows the
conversation contents; meaningful findings/highlights, categories and recaps are
optional. Compact footnotes provide source evidence. Concise explanatory footnotes
from clarification answers are included
where specialist or internal context helps understanding. The provisional QMD is
reviewed after the first test project and revised no later than after the second.
Suggestions never become decisions and absent facts are not invented. The
[generic QMD template](.agents/skills/draft-conversation-notes/assets/conversation-notes.qmd)
is copied to an approved unversioned working location before being populated.
The first conversation trial has produced a QMD draft and DOCX, now placed in
the approved external sync project; review and the correction round-trip remain pending.

## Permanent versioning boundary

All conversation files stay permanently unversioned and off GitHub, including
JSON, derivatives, QMD, DOCX/PDF/HTML, annotated copies, traces, intermediates and
fictional trial files. They may reside inside the project directory in deliberately
selected ignored locations. The selected unversioned QMD remains authoritative.
Versioned Git content holds only skills,
scripts, generic templates, configuration and conversation-free project docs.

[CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md) defines this deliberate Docs
Template deviation and the clarification in PDR-0002. Ignored
CONVERSATION_PATHS.local.md maps the persistent external sync project and
device-local repository temp/conversation-work/. Both are configured on this host;
remote synchronization is unchecked. Other mapped ignored local folders are
allowed after verifying Git exclusion. Exact file access, outside writes, sync
transmission, sharing and publication remain separate decisions. Temporary files
are never synchronized; conversation content is never staged, committed or force-added.

## Current state and next step

Project rules and external render/revision instructions are configured.
Quarto 1.9.38/Pandoc 3.8.3 are present. The separately approved local validator
setup provides Python 3.12.14/PyYAML 6.0.3; both adapted skills and the new drafting
skill passed validation. Pandoc parsed the generic QMD structure and footnotes.
A selected transcript was clarified and a QMD/DOCX draft technically checked.
The authoritative QMD, DOCX and retained revision evidence were placed in the
approved external sync project and their copies verified by SHA-256.
Its content remains unversioned; no publication occurred. Remote sync is unchecked.
No versioned project milestone is complete.

Next review the DOCX and transfer accepted corrections to the authoritative QMD.
The generic trial contract
is [DOCUMENTS.md](DOCUMENTS.md); tooling prerequisites are in
[DOCS_SETUP.md](DOCS_SETUP.md). Repository docs/ contains workflow guidance only.

## License

[MIT](LICENSE). Existing copyright/attribution is retained.
This repository license grants no access to or sharing of conversation files.
