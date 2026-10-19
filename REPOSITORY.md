# Repository Model

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
