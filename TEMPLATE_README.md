# AGIT Conversation Notes — Workflow Guide

> [!NOTE]
> **AI Collaboration**
>
> This project uses AI assistance for documentation practices, scoped workflows,
> source traceability and review. [COLLABORATION.md](COLLABORATION.md) records
> maintainer authority and the unversioned conversation-source exception.

[Deutscher Leitfaden](TEMPLATE_README.de.md) · [Project introduction](README.md)

This guide adapts inherited AI Documentation Template operating guidance.
[PROJECT_CONTEXT.md](PROJECT_CONTEXT.md) records verified source lineage,
synchronization baseline and intentional deviations. Local AGENTS.md and domain
rules remain authoritative. Initialization is complete; the inherited one-time
skills were removed. Routine bounded entry is start-task.

## Contents

- [Conversation workflow](#conversation-workflow)
- [Storage and access](#storage-and-access)
- [Collaboration Skills](#collaboration-skills)
- [Render Validation and Visual Inspection](#render-validation-and-visual-inspection)
- [Git Index and Protected Git Actions](#git-index-and-protected-git-actions)
- [Decision Records](#decision-records)
- [Repository and tooling](#repository-and-tooling)
- [License](#license)

## Conversation workflow

The [draft-conversation-notes skill](.agents/skills/draft-conversation-notes/SKILL.md)
provides instructions for detailed German thematic summaries for personal recall. It does not organize by who said
what. Relevant transcript references support checking; names are included only
when needed. Distinguish results, decisions, tasks and open questions, mark
uncertainty, keep suggestions distinct from decisions and invent no missing data.
First clarify ambiguity through contextual numbered questions in sequential
batches of at most ten. Then preserve important arguments, reasons and alternatives;
record actual conversation date/participants and adapt structure to the content.
Meaningful findings/highlights, categories, tables and overviews are optional;
use compact source footnotes. Review the provisional QMD after the first completed
test project and revise it no later than after the second. Original quotes appear only when wording matters or uncertainty
persists. The [generic QMD asset](.agents/skills/draft-conversation-notes/assets/conversation-notes.qmd)
is copied/populated at an approved unversioned location. The recorded first
trial has completed clarification, drafting and DOCX export; review and the
correction round-trip remain pending.

An optional generic test can use a small fictional transcript externally: reviewed
structure -> authoritative QMD -> DOCX -> maintainer comments/Track Changes ->
accepted corrections to QMD -> checked re-render. No real files are required.

For subsequent generic repository documents, explicitly invoke add-document.
Its confirmed contract and navigation stay conversation-free. It does not
register concrete conversations in the versioned catalog.
[DOCUMENTATION_PROCESS.md](DOCUMENTATION_PROCESS.md) and
[FEEDBACK_WORKFLOW.md](FEEDBACK_WORKFLOW.md) define the ongoing cycle.

## Storage and access

[CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md) overrides inherited placement
and versioning defaults. All conversation JSON, derivatives, QMD, rendered formats,
returned review copies, snapshots, trace, logs and temporary files remain
permanently unversioned and off GitHub, including fictional trials. Ignored local
repository locations are allowed when deliberately mapped and checked for Git
exclusion. Unversioned QMD remains authoritative without Git history. Never put
conversation content in versioned templates, docs or project records; never force-add it.

Use ignored CONVERSATION_PATHS.local.md: persistent external sync storage by
default, device-local ignored repository temp/conversation-work/ for intermediates.
Exact file access and
outside writes must be authorized per task. Non-sensitive classification and
mapping do not grant access. Sync storage is separately configured; transmission,
sharing, publication, backup and access remain separate decisions. Do not sync
temporary content. Preserve originals, use external working/trace storage and
reconcile the external export baseline before revision.

## Collaboration Skills

Skills are scoped workflows in [`.agents/skills/`](.agents/skills/). They guide
the agent through a particular task and load the relevant repository guidance.
Invoke a skill in chat with `$skill-name`, for example
`$review-project`. The linked skill files describe each full workflow.

- **Agent or explicit:** The agent may select the skill when the task fits;
  you can also invoke it directly.
- **Explicit:** The skill needs a deliberate invocation or explicit maintainer
  selection. An agent suggestion does not activate it.
- **Task-driven or explicit:** Rendering may follow a render request or
  necessary validation; unrestricted implicit skill selection is disabled.
  Direct invocation remains available.

Selecting a skill grants no additional permission for protected Git actions,
installation, external transmission or publication. Local access and domain
rules apply to every workflow.

In `commit-changes`, explicit commit authorization includes normal push to this
repository's verified existing upstream. In `commit-milestone`, explicit milestone
commit authorization also includes one matching annotated version tag and its
exact upstream push. "Commit only" excludes tags and pushes; "no push" retains
the local commit/tag; "no tag" excludes tags; "no tag push" keeps the tag local.
Other Git actions, tag movement/replacement and release publication stay separate.

`reuse-fixes` reads and updates only this repository's error knowledge. It does
not collect lessons across repositories or maintain global memory.
Active fixes use 4–8 lines per case in `TROUBLESHOOTING.md`.
[Detailed evidence](TROUBLESHOOTING_DETAILS.md) is preserved separately;
read only a matching detail section when needed.

| Skill | Invocation | Purpose |
| --- | --- | --- |
| [`start-task`](.agents/skills/start-task/SKILL.md) | Agent or explicit | Reconstruct only the context needed for a new bounded task. |
| [`handoff-task`](.agents/skills/handoff-task/SKILL.md) | Agent or explicit | Save the task outcome, evidence and next step in a compact `TASK_HANDOFF.md`. |
| [`commit-changes`](.agents/skills/commit-changes/SKILL.md) | Agent or explicit | Create an ordinary scoped commit and perform its normal upstream push with explicit commit authorization, unless push is excluded. |
| [`record-decision`](.agents/skills/record-decision/SKILL.md) | Agent or explicit | Document a durable decision using the applicable record type; source-template decisions route to Governance. |
| [`reuse-fixes`](.agents/skills/reuse-fixes/SKILL.md) | Agent or explicit | Reuse this repository's confirmed fixes, retain concise prevention and ask only for missing authority or blocking decisions. |
| [`review-project`](.agents/skills/review-project/SKILL.md) | Explicit | Produce a comprehensive neutral inventory of project state and evidence gaps. |
| [`manage-external-storage`](.agents/skills/manage-external-storage/SKILL.md) | Explicit | Set up optional external storage, connect a host or check selected local files. |
| [`sync-template`](.agents/skills/sync-template/SKILL.md) | Explicit | Compare a derived project with its verified source template and adopt selected updates while preserving project adaptations. |
| [`check-consistency`](.agents/skills/check-consistency/SKILL.md) | Explicit | Diagnose internal contradictions between intent, roadmap, decisions, content and documentation; develop bounded options. |
| [`perform-retrospective`](.agents/skills/perform-retrospective/SKILL.md) | Explicit | Review collaboration evidence and distinguish project findings from reusable template or family candidates. |
| [`add-document`](.agents/skills/add-document/SKILL.md) | Explicit | Add a maintained document or linked language versions, including catalog metadata and navigation. |
| [draft-conversation-notes](.agents/skills/draft-conversation-notes/SKILL.md) | Agent or explicit | Clarify external transcripts in batches of at most ten and draft content-led German QMD with date/participants, optional highlights and footnotes. |
| [`render-document`](.agents/skills/render-document/SKILL.md) | Task-driven or explicit | Render maintained Quarto sources in the required formats and check technical output and placement. |
| [`revise-document`](.agents/skills/revise-document/SKILL.md) | Explicit | Evaluate authorized annotated DOCX or PDF feedback and transfer accepted revisions into maintained sources. |
| [`review-document`](.agents/skills/review-document/SKILL.md) | Explicit | Critically review a document or section for correctness, reader success and clarity; return grounded findings and improvement proposals. |
| [`visual-inspection`](.agents/skills/visual-inspection/SKILL.md) | Explicit | Inspect named current HTML, PDF or DOCX renders visually and report exact coverage and limits. |
| [`commit-milestone`](.agents/skills/commit-milestone/SKILL.md) | Explicit | Close a reviewed milestone with metadata, comprehensive checks, a commit, annotated version tag and exact upstream pushes unless excluded. |

### Optional Planning Skills

`grill-me` and `grilling` are adopted MIT-licensed skills by Matt Pocock.
They complement the repository's own skills and are used only after explicit
selection. The normal lean document-setup path remains available.

| Skill | Invocation | Purpose |
| --- | --- | --- |
| [`grill-me`](.agents/skills/grill-me/SKILL.md) | Explicit | Start the optional intensive planning interview and route it to `grilling`. |
| [`grilling`](.agents/skills/grilling/SKILL.md) | Explicit | Explore a plan, decision or idea through detailed interview rounds; use only after explicit opt-in. |

## Render Validation and Visual Inspection

Routine render and output validation may run Quarto and inspect the generated
HTML technically without opening the Browser skill. It checks build success,
warnings, required files, HTML structure, links, referenced assets and obvious
unrendered source content as relevant. This does not count as visual
inspection.

Invoke `$visual-inspection` explicitly when the agent should inspect named
current renders in maintainer-selected formats. It opens rendered HTML with the
Browser skill or inspects selected PDF/DOCX pages as page images. A milestone,
render or visual change does not trigger this workflow. Missing output is not
rendered or replaced, and the report names inspected pages, routes, viewports,
findings and limitations. Visual inspection does not certify accessibility,
technical correctness, disclosure approval or publication readiness.

## Git Index and Protected Git Actions

The maintainer controls Git history. Assistants may inspect status, diffs and logs, prepare documentation changes and propose commit boundaries and metadata.

Staging and unstaging are index operations. They do not require a control word, but they may be performed only after a specific maintainer request or authorization of the corresponding commit. Existing staged selections and unrelated changes must be preserved.

Protected actions include commits, amendments, tags, pushes, pulls, merges, rebases, resets, branch changes, stash manipulation and other Git history operations. An assistant may perform a specific protected action only when the instruction for that action contains `explicit` or `explicitly` in English, or the German word family `explizit`. File-edit approval does not authorize Git history changes, and other protected actions remain separately authorized, with the bounded commit workflows above as the specific exceptions.

When this rule requires authorization, the assistant proposes one minimum-scope,
copy-ready instruction naming the exact action, repository and material
consequence. The proposal itself is not authorization.

Regular documentation commits normally use `docs:` or another fitting Conventional Commit prefix. Milestone commits omit the prefix, include the completed version and close documentation already drafted, reviewed and corrected in regular steps.

## Decision Records

Choose the record type by decision subject:

- **DDR — Documentation Decision Record:** information architecture, audience assumptions, terminology, bilingual model, screenshot policy, link model, visual standards, publication workflow or milestone scope.
- **PDR — Project Decision Record:** project scope, roadmap, collaboration, privacy, source governance or repository structure.
- **ADR — Architecture Decision Record:** Quarto structure, build pipeline, tooling, output model, automation or another durable technical documentation-system decision.

Templates live in [decisions/](decisions/). Create a record only when the rationale and consequences will matter to future maintainers; ordinary wording changes and routine corrections do not need one.

## Repository and tooling

[REPOSITORY.md](REPOSITORY.md) describes the current layout. docs/ and _quarto.yml
contain only generic workflow documentation; their optional HTML output stays
in ignored output/html/. Existing input guidance remains unchanged. Repository
folders may hold conversation files only in deliberately mapped ignored/untracked
locations. temp/conversation-work/ is the default temporary location.

Quarto 1.9.38 and Pandoc 3.8.3 are available. Plain external QMD -> DOCX needs no
TeX/R/Python. [QUARTO.md](QUARTO.md) documents the external command pattern, still
to be verified in the fictional trial. Python/PyYAML is separately needed for
the mandatory skill validator. The separately approved clone .venv now provides
Python 3.12.14/PyYAML 6.0.3 and both adapted skills passed. New-clone setup follows
[VALIDATION.md](VALIDATION.md) with separate installation approval.
Optional PDF and visual tooling is deferred.

CHANGELOG and TASK_HANDOFF now contain project-owned state. The inherited backlog
and one-time setup/creation skills were removed; setup provenance is retained.
Later template sync requires the original upstream commit to be verified; the
imported snapshot is not claimed as that commit.

## License

The repository retains its [MIT license](LICENSE), including the existing
Christian Treffenstaedt copyright notice. Template provenance is documented in
PROJECT_CONTEXT.md; it is not a separate project version or rights declaration.
The retained grill-me/grilling skills by Matt Pocock keep their MIT notices in
their skill directories. A repository license grants no conversation sharing or
publication authority.
