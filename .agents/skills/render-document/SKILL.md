---
name: render-document
description: Render a maintained Quarto document or report through the repository's established formats, output locations and technical validation workflow.
---

# Render Document

Confirm the authoritative source, requested or required format, Quarto project
configuration and documented output location. Apply local source-access,
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

## AGIT external conversation scope

Before rendering a conversation document, read CONVERSATION_STORAGE.md and
QUARTO.md at the repository root. Resolve the exact external QMD, format-specific
output, resources, cache/log and temporary destinations through ignored
CONVERSATION_PATHS.local.md. An Unset or unavailable mapping stops dependent work.
Require scoped access and outside-write authority. Check canonical paths and
containing Quarto configuration, including reparse points, so every artifact and
intermediate remains outside Git. Work in the external source context and never
copy content into repository input/materials/docs/temp/output/review folders.

External QMD remains authoritative and permanently unversioned. Initially render
DOCX only, unless another format is specifically selected. Retain review baseline
and source/output evidence in external trace/; keep all content-bearing diagnostics
external. Report only generic workflow status into project docs/handoffs.
The repository _quarto.yml is for conversation-free workflow pages, never the
conversation render configuration. Follow existing no-install/no-publication
and separately explicit visual-inspection boundaries.
