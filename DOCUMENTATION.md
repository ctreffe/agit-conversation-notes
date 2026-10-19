# Documentation Architecture

For any actual or fictional conversation, [CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md)
overrides the generic placement, catalog and promotion instructions below. All
conversation contexts, reports, data, identifiers and metadata remain permanently
unversioned in explicitly mapped storage. No implicit local fallback, Git promotion
or tracked conversation catalog/handoff entry is permitted. Repository docs and
these scaffolds remain conversation-free; populate only an approved unversioned copy.

The repository contains a reusable workflow and conversation-free project docs.
[CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md) overrides inherited source
placement/promotion defaults. Selected unversioned QMD is authoritative for each conversation;
repository Markdown/QMD is authoritative for generic project rules.

README.md and README.de.md introduce the project; TEMPLATE_README.md and
TEMPLATE_README.de.md retain adapted operating guidance. Each pair is a close
English/German translation with reciprocal links and project/guide navigation.
Retained guides omit inherited badges.

PROJECT_SETUP.md retains the setup method; PROJECT_CONTEXT.md records the
verified import baseline and status. DOCS_SETUP.md holds confirmed defaults;
DOCUMENTS.md contains generic contracts, never a conversation index.
AGENTS.md/COLLABORATION.md define authority; REPOSITORY.md defines layout.
QUARTO.md/FEEDBACK_WORKFLOW.md govern unversioned render/revision; decisions/ contains
durable generic records without conversation contents.

[draft-conversation-notes](.agents/skills/draft-conversation-notes/SKILL.md) and its
[QMD asset](.agents/skills/draft-conversation-notes/assets/conversation-notes.qmd)
implement the agreed clarification/drafting method; the conversation trial is pending.
Conversation files are excluded from versioning and GitHub. Persistent storage
defaults to external sync; deliberately mapped ignored repository locations are
allowed, with temp/conversation-work/ for device-local temporary processing.
The inherited one-time setup/creation
skills and template backlog were removed after successful initialization.
CHANGELOG/TASK_HANDOFF now contain project-owned state. Subsequent work uses
start-task. No workflow grants Git/publication authority.

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
