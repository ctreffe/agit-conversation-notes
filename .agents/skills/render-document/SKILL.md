---
name: render-document
description: Render a maintained Quarto document or report through the repository's established formats, output locations and technical validation workflow.
---

# Render Document

## Conversation storage takes precedence

Read [CONVERSATION_STORAGE.md](../../../CONVERSATION_STORAGE.md) before any
conversation-related work. For actual or fictional conversations, resolve the
context, source catalog, report/data destinations and trace only through approved
ignored CONVERSATION_PATHS.local.md and the selected unversioned catalog. Keep
all IDs, context contents, research metadata and detailed next steps out of
tracked catalogs, docs, decisions and TASK_HANDOFF.md. Their generic instructions
below apply only to conversation-free workflow documentation. An unset mapping
stops dependent work; never choose an implicit fallback or create a mapping.
Update conversation context in its approved unversioned location at task entry
and handoff; tracked handoff records generic workflow status only. Reports/data
and contexts for conversations are permanently unversioned, not eligible for
later Git promotion. Existing input/working/sources/output/review/trace layout
remains authoritative; no new generic directory layout replaces it.

Confirm the authoritative source, requested or required format, Quarto project
configuration and documented output location. For a cataloged document,
resolve its context from `DOCUMENTS.md` for required formats and validation
rules; navigation-only pages use the project configuration. Keep
`DOCUMENT_CONTEXT.md`, research reports and data not approved for publication
out of rendered pages, includes and copied resources; inspect the actual
output scope when resource/render rules change. Apply local source-access,
environment and disclosure rules before rendering. Use the existing project
toolchain and do not install or update dependencies without approval.

Run the narrowest documented render command that proves the requested result.
Inspect exit status, warnings, unresolved citations, missing resources and
output placement. Preserve maintained sources and unrelated generated files.

Rendering and technical output inspection are not visual inspection. Do not
invoke `$visual-inspection`, open the Browser skill or create page-image
inspection evidence as part of routine rendering. Report the exact source,
format, output, checks, warnings and skipped review surfaces, and do not infer
publication approval from a successful render.

## AGIT unversioned conversation scope

Before rendering a conversation document, read CONVERSATION_STORAGE.md and
QUARTO.md at the repository root. Resolve the exact selected unversioned QMD, format-specific
output, resources, cache/log and temporary destinations through ignored
CONVERSATION_PATHS.local.md. An Unset or unavailable mapping stops dependent work.
Require scoped access and authority for writes outside the repository. Check
canonical paths, reparse points and containing Quarto configuration. Every
artifact and intermediate stays unversioned and off GitHub; verify ignore
coverage and absence of tracked conversation files for mapped repository paths.
Use ignored temp/conversation-work/ for temporary processing. Work in the selected
source context; never populate versioned templates or documentation with content.

The selected QMD remains authoritative and permanently unversioned. Initially render
DOCX only, unless another format is specifically selected. Retain review baseline
and source/output evidence in mapped unversioned trace/; keep content-bearing diagnostics
unversioned. Persistent storage defaults to the external sync project. Report only generic workflow status into project docs/handoffs.
The repository _quarto.yml is for conversation-free workflow pages, never the
conversation render configuration. Follow existing no-install/no-publication
and separately explicit visual-inspection boundaries.
