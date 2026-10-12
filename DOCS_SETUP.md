# Documentation Setup

AGIT Conversation Notes was configured starting 2026-10-12 and initialization
completed on 2026-10-13; see [PROJECT_CONTEXT.md](PROJECT_CONTEXT.md).

## Confirmed fundamentals

- Purpose: detailed thematic preparation of discussed content as a personal
  memory aid; no speaker-by-speaker narrative.
- Document language: German. Repository introductions/guides: English/German.
- Type: conversation summary; detailed project-specific profile deferred.
- Lifecycle: planned, draft, review, stable, archived. Initial trial: planned.
- Source: university Whisper-v3 JSON; fallible recognition and speaker attribution.
- Output: external DOCX for maintainer comments/Track Changes, then accepted
  corrections back to authoritative external QMD.
- Access: no real files selected; exact files/actions need scoped approval.
- Publication, sharing, transmission and sync setup: separate decisions.
- Only the separately approved local validator setup was installed; no Git
  writes, sync setup or other installations are authorized.

## Intentional Docs Template deviation

All conversation sources, working files, QMD, outputs, review copies and traces
remain permanently external and unversioned, including fictional trial files.
Use ignored CONVERSATION_PATHS.local.md, never repository fallback folders.
External QMD remains authoritative. See
[CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md) and
[PDR-0001](decisions/PDR-0001-external-conversation-files.md).
Repository docs/ contains only conversation-free workflow documentation.
Protocol schema and the proposed drafting skill are deferred.

## Minimum trial evidence

After joint schema/skill design and external destination approval, use a small
fictional excerpt externally. Verify thematic structure, source references,
uncertainty and proposal/decision distinctions. Render DOCX externally, map a
clear maintainer correction back to QMD, retain external baseline evidence,
re-render and check changed content. No conversation data enters Git.
Visual inspection remains separately explicit.

## Tooling checkpoint

Quarto 1.9.38 and Pandoc 3.8.3 are present. Plain DOCX needs no TeX/R/Python.
The separately approved ignored .venv provides Python 3.12.14 and PyYAML 6.0.3.
Both adapted skills passed Test-CodexSkill.ps1. Reproduce on another clone through
[VALIDATION.md](VALIDATION.md), obtaining installation approval there.
No DOCX round-trip/render has been run. Revision-extraction libraries are
selected during concrete tooling design; PDF and visual tooling are deferred.
