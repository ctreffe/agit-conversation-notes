# Quarto Workflow

For any actual or fictional conversation, [CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md)
overrides the generic placement, catalog and promotion instructions below. All
conversation contexts, reports, data, identifiers and metadata remain permanently
unversioned in explicitly mapped storage. No implicit local fallback, Git promotion
or tracked conversation catalog/handoff entry is permitted. Repository docs and
these scaffolds remain conversation-free; populate only an approved unversioned copy.

The project separates repository workflow documentation from conversation renders.

## Repository workflow documentation

_quarto.yml renders only conversation-free docs/ entry pages as an optional
bilingual HTML website in ignored output/html/. Never include external
conversation sources. No website is published by initialization.

## Unversioned conversation documents

Selected QMD is authoritative and unversioned. Resolve the exact authorized
source and destination through ignored CONVERSATION_PATHS.local.md; follow
[CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md). Confirm source, resources,
containing project configuration, outputs, caches, logs and intermediates stay
unversioned and off GitHub, including through symlinks/junctions. Persistent
storage defaults to external sync; deliberately mapped ignored repository paths
are also allowed after verifying ignore coverage and absence of tracked content.
Use device-local ignored temp/conversation-work/ for temporary processing.
Work from the selected source context; never populate versioned templates or
documentation, or reuse the repository website configuration for conversation renders.
The initial plain-text trial needs no executable chunks or external fetches.

The locally checked Quarto 1.9.38 CLI supports this command pattern:

    quarto render <authorized-external-source.qmd> --to docx --no-execute --output-dir <authorized-external-docx-directory>

Output directories are input/project-relative unless absolute; resolve them
deliberately. This pattern is not yet a tested project render recipe. Check any
containing external Quarto project before use. Plain DOCX uses bundled Pandoc
without TeX/R/Python. Optional PDF/HTML need deliberate scope/toolchain selection.
All outputs and intermediates remain unversioned; local repository paths must be ignored.

## Review evidence

Check exit status, warnings, missing resources, actual placement and DOCX
technical structure. Retain source baseline and source/output relationship
in mapped unversioned trace/ before review. Transfer accepted comments/Track Changes into selected
QMD, reconcile baseline drift and re-render. See
[FEEDBACK_WORKFLOW.md](FEEDBACK_WORKFLOW.md).
Rendering is not content/visual/publication approval or backup.
No render or round-trip occurred during initialization.

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
