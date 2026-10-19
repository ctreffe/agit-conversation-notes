# Documentation Process

For any actual or fictional conversation, [CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md)
overrides the generic placement, catalog and promotion instructions below. All
conversation contexts, reports, data, identifiers and metadata remain permanently
unversioned in explicitly mapped storage. No implicit local fallback, Git promotion
or tracked conversation catalog/handoff entry is permitted. Repository docs and
these scaffolds remain conversation-free; populate only an approved unversioned copy.

Project defaults are in PROJECT_CONTEXT.md and the generic initial contract in
DOCUMENTS.md. [CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md) governs every
conversation artifact. [draft-conversation-notes](.agents/skills/draft-conversation-notes/SKILL.md)
implements the agreed clarification and QMD drafting instructions.

## Content-led document design

Start with a short conversation header recording the actual date and participants.
Use approved evidence or maintainer confirmation; ask if missing or uncertain.
Do not infer these facts from export dates, faulty speaker labels or people merely
mentioned in the conversation. Deliberately unresolved metadata stays marked unknown.

Adapt the document to the actual discussion rather than a minutes schema. Use
descriptive topic headings, prose or lists where helpful. Preserve important
content, arguments, reasons and alternatives; condense repetitions and fillers
without changing meaning. Do not organize by speaker or invent missing facts.

Light emphasis on supported results, decisions, tasks and open questions remains
useful where it helps the reader. These labels and separate sections are optional;
no empty categories or compulsory findings. An opening overview, closing recap or
table is likewise optional. Any recap adds no new claims or greater certainty.
Relevant content belongs in the narrative even without a separate label.

Keep compact footnotes on relevant claims with actual transcript evidence; quote
original wording only when wording matters or uncertainty persists. Distinguish
maintainer clarification from original evidence.

Use concise explanatory footnotes for specialist terms, internal structures and
background supplied in the clarification rounds when they help understanding.
Attach an explanation at the first relevant occurrence and condense it rather
than copying the question/answer exchange. Essential discussion content remains
in the main text. Distinguish explanation from transcript evidence: explanation
notes may start with Erläuterung aus der Klärung; source notes retain actual
locators. Both may share a note when still readable. Trace supplemental knowledge
to its clarification answer in the private unversioned trace and preserve the
maintainer's uncertainty. A correction alone does not require a knowledge note.
See [DDR-0003](decisions/DDR-0003-explanatory-clarification-footnotes.md).

See [DDR-0002](decisions/DDR-0002-content-led-provisional-notes.md) and the
[generic QMD template](.agents/skills/draft-conversation-notes/assets/conversation-notes.qmd).
This tracked asset contains placeholders only; populate a copy exclusively at an
authorized unversioned working location, including a deliberately mapped ignored
repository location.

## Agreed two-stage drafting workflow

### 1. Clarify the transcript

Before producing the structured document, inspect the exact authorized unversioned
transcript for unclear or implausible terms, recognition errors, contradictions
and missing context that affect meaning. Consider phonetic similarity and the
surrounding discussion when proposing an interpretation; a plausible guess is
not a confirmed correction. Ask about nonsensical or uncertain terms instead of
silently substituting them. Speaker labels are fallible. Clarify attribution when
it affects the content or an assignment, rather than reconstructing every speaker.

Present a numbered list of questions. Each item contains an actual transcript
locator when available, a short excerpt with enough surrounding context, the
unclear expression or claim, and a concrete question. An optional phonetic or
contextual interpretation is explicitly a suggestion. Never invent locators or
quotes. Group repeated occurrences of the same ambiguity where useful, keeping
their source references so the maintainer need not answer the same question again.

Each batch contains at most ten numbered points. If there are more, present the
first batch and wait for the maintainer's answers before the next. Keep numbering
stable across batches (1-10, then 11-20, etc.), accept answers by number and use
earlier corrections to reassess remaining questions. Follow up only where an
answer remains unclear or creates a new material ambiguity. If no relevant
ambiguities are found, state that briefly and proceed to stage two.

Apply the maintainer's clarifications to the working interpretation, preserving
original JSON unchanged. Store correction mappings, excerpts and question/answer
trace in mapped unversioned storage. Proceed to the structured draft after the clarification cycle
is completed. An item the maintainer cannot resolve or deliberately defers stays
explicitly uncertain; do not treat it as settled or fill in missing facts.

### 2. Prepare the structured content

Use the clarified interpretation to prepare the German content account. Where
such content occurs, preserve the distinction between results, decisions, tasks
and open questions without requiring category blocks. Maintain source references
and any deliberately unresolved uncertainty. Do not organize by speaker, invent
owners/deadlines or turn suggestions into decisions. Ask further targeted questions
when synthesis reveals unresolved meaning or uncertain classification; use the
same numbered batches of at most ten points. Clarify affected claims before
treating them as confirmed. Use the flexible content-led design above; findings
are distinguished where present, not manufactured as compulsory categories.

This is the agreed contract implemented by draft-conversation-notes. The recorded first trial has completed
drafting/export; maintainer review and the correction round-trip remain pending. All concrete excerpts, questions,
corrections, drafts and trace files remain unversioned and off GitHub under
CONVERSATION_STORAGE.md; mapped ignored repository storage is allowed, with
temp/conversation-work/ for device-local intermediates. Only
generic workflow rules are recorded here.

## Template review checkpoint

The generic QMD starter is provisional. Evaluate the document together after the
first completed test project; review and revise the generic QMD no later than
after the second. Consider natural structure, content detail, conversation header,
useful highlights and evidence readability. Completed test projects: zero.
Concrete trial files and feedback stay unversioned. Record only conversation-free
workflow conclusions and generic template changes in the repository.

## Planned conversation cycle

1. Select exact mapped unversioned files and scoped access/write authority.
2. Preserve original Whisper JSON; create derivatives in selected unversioned storage.
3. Clarify transcript ambiguities with the maintainer in batches of at most ten,
   then produce a German thematic QMD using draft-conversation-notes.
4. Verify content/evidence and render bounded external DOCX for maintainer review.
5. Return accepted corrections to QMD with external baseline/decision trace.
6. Re-render and check changed content, storage boundary and unresolved questions.

A small fictional excerpt remains available for a separately selected generic
test. The current recorded trial uses an already authorized transcript; its
private details remain outside versioned documentation. No new file access,
sync setup or participant sharing follows from this workflow description.
Repository status and handoffs contain generic progress only.

## Repository lifecycle

Use start-task for later bounded work. Explicit add-document concerns generic
repository document contracts; concrete conversation registration stays unversioned.
Record durable generic decisions in decisions/. Template sync needs verified
lineage and selected adoption. Review, consistency, retrospective and visual
inspection remain explicitly selected; Git actions need separate authority.

Initialization is complete with proportionate checks and required skill validation.
Inherited one-time skills/backlog were removed and project histories reset;
setup provenance and licensing are retained.

## Internal document contexts

[DOCUMENTS.md](DOCUMENTS.md) is the document/language-set index and lifecycle owner.
The linked `DOCUMENT_CONTEXT.md` owns the detailed contract, assembly/update
method, assigned catalog source IDs, evidence baseline and next actions.
Existing flat QMD source paths stay unchanged; their context is under
`docs/<document-slug>/`. New additions normally group context and sources there.
Populate the context during explicit `add-document`, read it at task entry and
refresh affected open questions and next steps before handoff. Reconstruct only
supported historical facts; record missing methods as gaps. Shared sources remain
centralized in input/material catalogs, with per-document assignments in contexts.
Keep contexts, research reports and scaffolds out of navigation, includes and
copied publication resources. Root-anchor render patterns and inspect their actual
input scope; render exclusions alone do not prevent resource copying.

Research runs only after explicit `investigate-question` invocation. Save a report
from templates/RESEARCH_REPORT.md for one or several related operationalized
questions, with individual source assessments and per-question answers/gaps.
Use materials/README.md#research-storage-and-reuse for placement and metadata.
