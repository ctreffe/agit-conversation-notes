# Repository Model

For any actual or fictional conversation, [CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md)
overrides the generic placement, catalog and promotion instructions below. All
conversation contexts, reports, data, identifiers and metadata remain permanently
unversioned in explicitly mapped storage. No implicit local fallback, Git promotion
or tracked conversation catalog/handoff entry is permitted. Repository docs and
these scaffolds remain conversation-free; populate only an approved unversioned copy.

Git contains skills, scripts, generic templates, configuration and conversation-
free project documentation. All concrete conversation files, including fictional
trials, remain permanently unversioned and off GitHub. Deliberately mapped ignored
repository locations are allowed; selected unversioned QMD is authoritative;
[CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md) is binding.

## Layout

- README.md / README.de.md: project introductions.
- TEMPLATE_README.md / TEMPLATE_README.de.md: adapted operating guides.
- AGENTS.md / COLLABORATION.md: authority and collaboration.
- PROJECT_CONTEXT.md / DOCS_SETUP.md / DOCUMENTS.md: project defaults and generic
  planned contract; no conversation catalog or review ledger.
- PROJECT_SETUP.md: retained initialization method.
- CONVERSATION_STORAGE.md: binding conversation versioning/storage deviation.
- CONVERSATION_PATHS.local.example.md: generic mapping example; ignored
  CONVERSATION_PATHS.local.md: host paths; persistent sync and local temp mappings.
- .agents/skills/, scripts/, styles/: reusable methods/tooling/generic styles.
- .agents/skills/draft-conversation-notes/assets/conversation-notes.qmd: generic
  drafting template, copied/populated only at authorized unversioned locations.
- docs/ / _quarto.yml: optional conversation-free workflow website.
- decisions/: durable generic DDR/PDR/ADR records and templates.
- input/: inherited classification guidance; unchanged, no conversation import.
- materials/, output/, review/: generic guidance plus deliberately mapped ignored
  local storage when selected; never populate their versioned guidance with content.
- temp/conversation-work/: ignored device-local conversation intermediates;
  never synchronized or versioned. Do not inspect temp/restricted/.
- CHANGELOG.md: project-owned Unreleased history; TASK_HANDOFF.md: current bounded
  task checkpoint. No inherited template backlog is retained.

Concrete external paths/provider details never enter tracked project state.
No classification, mapping or sync grants access/transmission.
No repository symlink/junction may expose conversation folders.

## Git workflow

Inspect branch/worktree/staging read-only and preserve selections/unrelated work.
Staging/unstaging needs an exact request or corresponding commit authority.
Commits, tags, pushes, pulls, merges, rebases, resets, reverts, branches, stashes,
destructive restores, publication and direct .git changes require a specific
instruction containing explicit, explicitly or German explizit.
Authorized index writes use narrow platform escalation on their first attempt.

Ordinary commits use direct Conventional Commit prefixes and real multiline
descriptions. Milestones close reviewed work separately with version metadata.
Within commit-changes, explicit commit authority includes normal verified-upstream
push unless excluded. Within commit-milestone it also includes the matching
annotated tag and exact tag push unless excluded. Other refs, force push, tag
replacement and releases need separate authority. No Git write is authorized here.

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
