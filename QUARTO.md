# Quarto Workflow

The project separates repository workflow documentation from conversation renders.

## Repository workflow documentation

_quarto.yml renders only conversation-free docs/ entry pages as an optional
bilingual HTML website in ignored output/html/. Never include external
conversation sources. No website is published by initialization.

## External conversation documents

External QMD is authoritative and unversioned. Resolve the exact authorized
source and destination through ignored CONVERSATION_PATHS.local.md; follow
[CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md). Confirm source, resources,
containing project configuration, outputs, caches, logs and intermediates stay
outside Git, including through symlinks/junctions. Work from the external source
directory; never copy into the repository or reuse its website configuration.
The initial plain-text trial needs no executable chunks or external fetches.

The locally checked Quarto 1.9.38 CLI supports this command pattern:

    quarto render <authorized-external-source.qmd> --to docx --no-execute --output-dir <authorized-external-docx-directory>

Output directories are input/project-relative unless absolute; resolve them
deliberately. This pattern is not yet a tested project render recipe. Check any
containing external Quarto project before use. Plain DOCX uses bundled Pandoc
without TeX/R/Python. Optional PDF/HTML need deliberate scope/toolchain selection.
All outputs and intermediates remain external.

## Review evidence

Check exit status, warnings, missing resources, actual placement and DOCX
technical structure. Retain source baseline and source/output relationship
externally before review. Transfer accepted comments/Track Changes into external
QMD, reconcile baseline drift and re-render. See
[FEEDBACK_WORKFLOW.md](FEEDBACK_WORKFLOW.md).
Rendering is not content/visual/publication approval or backup.
No render or round-trip occurred during initialization.
