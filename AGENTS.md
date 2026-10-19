# AGENTS.md

For any actual or fictional conversation, [CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md)
overrides the generic placement, catalog and promotion instructions below. All
conversation contexts, reports, data, identifiers and metadata remain permanently
unversioned in explicitly mapped storage. No implicit local fallback, Git promotion
or tracked conversation catalog/handoff entry is permitted. Repository docs and
these scaffolds remain conversation-free; populate only an approved unversioned copy.

Resident contract.

## Safety

- Inspect repository, branch, worktree and staging; preserve changes and
  selections.
- Maintainers own intent, information architecture, technical truth and
  publication decisions. Maintained sources outrank generated review files.
- Authorized reads and edits are allowed. Commits, tags, pushes, pulls, merges,
  rebases, resets, reverts, branches, stashes, destructive restores,
  publication and direct `.git/` changes each require an instruction containing
  `explicit`, `explicitly` or German `explizit`.
- In `commit-changes`, explicit repository commit authorization includes normal
  verified-upstream push unless excluded. In `commit-milestone`, explicit milestone
  commit authorization also includes its matching annotated version tag and exact
  tag push. Honor commit-only/no-push/no-tag restrictions. Other Git actions,
  tag movement/replacement and release publication remain separately controlled.
- When such a control-word instruction is needed, propose one minimal copy-ready
  wording that names the exact action, repository and material consequence;
  the proposal is not authorization.
- Once exact staging is requested or its commit is authorized, run Git commands
  that write `.git` through narrow sandbox escalation on their first attempt;
  do not probe the expected `workspace-write` `.git/index.lock` denial. Keep
  read-only Git inspection sandboxed. Escalation grants no additional Git or
  standing authority.
- Use normal sandboxed execution when it is equally effective. If an already
  authorized in-scope action requires crossing a platform boundary, promptly
  request the narrowest sufficient escalation through the platform mechanism;
  do not omit or replace the action merely to avoid approval. Ask separately in
  prose only when action authority is missing or unclear. Escalation grants no
  broader repository, action, path, source, rendering, disclosure, publication,
  Git or standing authority.
- Ask before sensitive sources, installation, privilege, outside writes or
  transmission; access, versioning and publication are separate.
- Retry unchanged once only if plausibly transient. For clear or recurring
  failures, use `reuse-fixes` to consult this repository's confirmed fixes,
  continue within existing authority and ask only for a missing approval or
  blocking decision. Verify at the original operation and retain useful prevention.
- `input/intake/` grants no access; keep `input/` unchanged. Registered
  `materials/` and unrestricted `temp/` are readable; never version temporary
  content or inspect `temp/restricted/`. Synchronization grants no access.

## Routing

- Bounded work uses `start-task`, `TASK_HANDOFF.md`, targets and checks. Load
  `PROJECT_CONTEXT.md` only for project-wide state or unclear scope.
- For maintained-document work in an initialized project, resolve `DOCUMENTS.md`
  and read its `DOCUMENT_CONTEXT.md` for the local contract, assigned evidence
  and assembly/update rules; keep it current when accepted rules or evidence
  baselines change.
- Read `COLLABORATION.md` for initialization, full review, authority conflicts
  or collaboration-model changes. Load setup, documentation-process, audience,
  style, links, screenshots, Quarto and feedback guidance as needed.
- Task entry, handoff, ordinary commits and Decision Records route
  automatically. Rendering routes only when an artifact is requested or
  supplies necessary evidence. Invoke initialization, document addition,
  visual inspection, review, `investigate-question`, sync, consistency,
  retrospective, revision, local creation and `commit-milestone` explicitly.

## Validation

Codex skill edits use `scripts/Test-CodexSkill.ps1`; on first use follow
`VALIDATION.md` without creating a rendering or general authoring prerequisite.

Scale evidence by stage: a bounded source change needs the smallest useful
review, an ordinary commit needs targeted evidence for a good reviewable state,
and a milestone owns comprehensive link, bilingual, render and disclosure
checks. Whitespace and all-format rendering are not defaults before the
milestone unless affected or required by a stated risk. Only explicit
`$visual-inspection` inspects selected current renders. Report limits; rendering
alone establishes neither correctness nor publication readiness.

## Conversation workflow exception

- Follow CONVERSATION_STORAGE.md before conversation tasks. All conversation
  files, including fictional fixtures, JSON, working copies, QMD, outputs,
  review evidence, logs and intermediates stay permanently unversioned and off
  GitHub. Ignored local repository storage is allowed. Never copy content into
  versioned project docs, catalogs, handoffs or decisions; never force-add it.
- External QMD is authoritative despite being unversioned. Resolve exact source,
  output/review/trace and temporary locations through ignored
  CONVERSATION_PATHS.local.md; Unset stops dependent work. Mapping/non-sensitive
  classification grants no access, outside writes, transmission or sharing.
- Apply this exception to drafting, rendering, revision and document registration.
  Persistent storage defaults to the external sync project; temporary processing
  uses ignored temp/conversation-work/. Other repository conversation locations
  must be deliberately mapped, ignored and untracked, never implicit fallback.
  Verify canonical paths/configuration, including reparse points, caches and
  intermediates, and exclusion from Git tracking before processing.
- Use draft-conversation-notes for transcript clarification and thematic QMD drafts.
  Summaries prepare thematic German
  content for personal recall, using transcript evidence without speaker-by-speaker
  narration; preserve uncertainty and distinguish proposals from decisions.
  Follow the clarification batches, actual date/participants header, flexible
  content-led structure and footnote model in DOCUMENTATION_PROCESS.md. Findings,
  highlights and recaps are optional. Review/revise the provisional QMD after
  the first and no later than the second completed test project.
  Its generic asset is never populated
  with conversation content in the repository.
