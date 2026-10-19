# Documentation Setup

AGIT Conversation Notes was configured starting 2026-10-12 and initialization
completed on 2026-10-13; see [PROJECT_CONTEXT.md](PROJECT_CONTEXT.md).

## Confirmed fundamentals

- Purpose: detailed thematic preparation of discussed content as a personal
  memory aid; no speaker-by-speaker narrative.
- Document language: German. Repository introductions/guides: English/German.
- Type: thematic conversation summary; the agreed profile is documented in
  [DDR-0002](decisions/DDR-0002-content-led-provisional-notes.md): actual conversation
  header and flexible content-led structure, with optional findings/highlights.
- Lifecycle: planned, draft, review, stable, archived. Current trial: draft/export complete; review round-trip pending.
- Source: university Whisper-v3 JSON; fallible recognition and speaker attribution.
- Output: external DOCX for maintainer comments/Track Changes, then accepted
  corrections back to authoritative external QMD.
- Access: exact files/actions need scoped approval; classification or mapping
  does not grant blanket access.
- Publication, sharing, transmission and sync setup: separate decisions.
- Only the separately approved local validator setup was installed. Persistent
  sync folder setup and local temp placement are now configured; further Git
  writes, transmission or installations retain their separate approval boundaries.

## Intentional Docs Template deviation

All conversation sources, working files, QMD, outputs, review copies and traces
remain permanently unversioned and off GitHub, including fictional trial files.
Use ignored CONVERSATION_PATHS.local.md: external sync storage is the persistent
default; ignored device-local repository temp/conversation-work/ holds temporary
files. Other deliberately mapped ignored repository locations are allowed after
checking Git exclusion. Selected unversioned QMD remains authoritative. See
[CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md) and
[PDR-0002](decisions/PDR-0002-unversioned-conversation-storage.md).
Repository docs/ contains only conversation-free workflow documentation.
draft-conversation-notes and its generic QMD asset implement the agreed method
and layout. Current persistent placement and private trace are recorded in the
ignored mapping. The optional fictional test contract remains available; the
repository template is never filled with conversation content.

## Minimum trial evidence

Use an exactly authorized transcript or a selected fictional excerpt at the
approved unversioned destination. Verify content-led structure, conversation header,
useful optional emphasis, source references,
uncertainty and proposal/decision distinctions. Render DOCX externally, map a
clear maintainer correction back to QMD, retain external baseline evidence,
re-render and check changed content. No conversation data enters Git.
Visual inspection remains separately explicit.

## Tooling checkpoint

Quarto 1.9.38 and Pandoc 3.8.3 are present. Plain DOCX needs no TeX/R/Python.
The separately approved ignored .venv provides Python 3.12.14 and PyYAML 6.0.3.
The two adapted skills and new drafting skill passed Test-CodexSkill.ps1.
Pandoc parsed the generic QMD structure/footnotes. The later recorded trial
produced a technically checked DOCX; its review/correction round-trip is pending.
Reproduce on another clone through
[VALIDATION.md](VALIDATION.md), obtaining installation approval there.
No completed DOCX correction round-trip is recorded. Revision-extraction libraries are
selected during concrete tooling design; PDF and visual tooling are deferred.
