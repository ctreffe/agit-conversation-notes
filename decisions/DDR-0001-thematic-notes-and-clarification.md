# DDR-0001: Clarify transcripts before thematic conversation notes

Status: Superseded by [DDR-0002](DDR-0002-content-led-provisional-notes.md)
Date: 2026-10-13

## Context

The maintainer needs German content preparation for personal recall from fallible
Whisper transcripts. Recognition can yield implausible but phonetically close
terms, and unreliable speaker labels. Detailed content should remain readable
while decisions, tasks and unresolved matters can be found quickly.

## Decision

First clarify material transcript ambiguities with contextual numbered questions.
Each batch contains at most ten points, with answers awaited between batches and
stable numbering. Phonetic interpretations remain suggestions until clarified.
Preserve originals and retain unresolved uncertainty rather than guessing.

Then prepare a short overview and detailed thematic sections, retaining important
arguments, reasons and alternatives without repetition or fillers. Lightly
highlight supported results, decisions, tasks and open questions within each
topic. Add a concise closing overview with links back to those topics; it
introduces no new content or greater certainty.

Use compact footnotes on relevant claims with actual transcript evidence locators.
Quote original wording only when wording is important or uncertainty persists.
Ask further questions when synthesis reveals unclear meaning/classification.
Speaker attribution matters where it changes content or an assignment, not as
the organizing principle. Never invent facts or promote proposals to decisions.

## Rationale

Clarification reduces unsupported interpretation before synthesis. Topic-local
findings preserve context, and the closing overview supports quick retrieval.
Footnotes preserve checkability while keeping the main text readable.

## Consequences

draft-conversation-notes and its generic QMD asset implement this contract.
All concrete questions, corrections, source references, QMD and outputs remain
external and unversioned under [PDR-0001](PDR-0001-external-conversation-files.md).
Bold inline labels provide light emphasis; DOCX presentation is still to be
checked in the fictional trial. Technical validation is not behavioral/visual QA.

## Alternatives considered

- Findings only in final sections: loses immediate thematic context.
- Findings only within topics: makes quick retrieval less convenient.
- Silent phonetic substitution: treats plausible guesses as established facts.
- Speaker-by-speaker narrative or pervasive original quotes: does not serve the
  agreed thematic memory-aid purpose.

## Follow-up

Select external destinations and scoped authority, then test a small fictional
clarification/QMD/DOCX/correction cycle. Refine the method from observed problems.
