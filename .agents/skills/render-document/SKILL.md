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
