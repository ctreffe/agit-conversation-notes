# Conversation Storage and Access

This is the binding AGIT Conversation Notes exception to the inherited Docs
Template. See [PDR-0002](decisions/PDR-0002-unversioned-conversation-storage.md),
which supersedes the earlier blanket external-placement interpretation.

## Permanent boundary

All conversation files remain permanently unversioned and excluded from GitHub:
original Whisper JSON, prepared transcripts, authoritative QMD,
DOCX/PDF/HTML, returned review copies, attachments, extracts, logs, temporary
intermediates, source snapshots and revision evidence. This includes fictional
test conversations. Physical placement inside the repository is allowed in
deliberately selected ignored locations. Never stage, commit or force-add
conversation content, or put it into versioned project documentation, catalogs,
handoffs, Decision Records, issues or publication. Ignore rules exclude local
files from normal Git operations; they grant no access or processing authority.
Do not create repository links/junctions to conversation folders.

The versioned repository contains only skills, scripts, generic templates, configuration
and conversation-free project documentation. Repository docs/ is solely for
workflow documentation. Neither conversation sources nor accepted conversation
feedback may be promoted into repository documentation.

## Portable local mapping

Copy [CONVERSATION_PATHS.local.example.md](CONVERSATION_PATHS.local.example.md)
to ignored CONVERSATION_PATHS.local.md on each host. Map conversation:root
to the selected persistent project directory (external sync storage by default)
and conversation:temp to device-local ignored temp/conversation-work/ in this
repository. Other ignored local conversation folders are allowed when deliberately
mapped. Keep concrete host paths, provider details, participant metadata and
conversation catalogs out of versioned files. The persistent root starts Unset;
the example supplies the repository-relative temporary convention.
The mapping grants neither access nor writes, transmission or publication.

The generic layout below is a storage contract, not a fixed protocol schema:

    <external-project>/
      input/       # unchanged originals; scoped access only
      working/     # prepared transcripts and retained derivatives
      sources/     # authoritative, editable QMD
      output/docx/ # initially required review output
      output/pdf/  # optional, only when selected
      output/html/ # optional, only when selected
      review/      # unchanged returned annotated copies
      trace/       # private baseline snapshots and revision decisions
    <repository>/temp/conversation-work/ # ignored disposable processing, never synchronized

Before use, require exact maintainer-selected files and actions. Canonicalize
actual paths, including reparse points and inherited Quarto configuration. For
every in-repository conversation source, output, cache and intermediate, verify
that its resolved location is ignored and contains no tracked conversation files.
Keep all processing in mapped locations; do not use versioned generic templates
or documentation as working copies. Check availability without scanning other
folders. An unset, conflicting or unavailable mapping stops dependent work; never
silently select another location. Obtain outside-write authority for writes outside
the repository. A non-sensitive classification is not blanket file access.
No real files are needed or approved for initialization.

## Source and revision trace

The selected unversioned QMD is authoritative despite having no Git history,
whether externally stored or in an approved ignored local folder. Original transcripts
remain unchanged. Summaries organize content by topic, rather than reporting who
said what. Trace relevant claims to actual transcript segments/timestamps when
available. Do not invent identifiers, timestamps, speaker certainty,
responsibilities or dates. Mention people only where substantively needed, such
as a confirmed assignment; speaker labels remain fallible evidence. Distinguish
results, decisions, tasks, open questions and proposals. Mark uncertainty and
never present proposals as decisions.

Before DOCX review, retain a source snapshot or hash, source/output relationship
and review scope in mapped unversioned trace/. Keep feedback decisions and source-change
evidence there too. Reconcile a changed QMD against the export baseline before
applying feedback. Versioned project state records only generic workflow status,
never conversation IDs, excerpts, participant data or decisions.
The two-stage method and thematic layout are defined in DOCUMENTATION_PROCESS.md
and implemented in draft-conversation-notes; concrete external trace format is
selected for the authorized trial. Recovery/backup is a separate storage decision;
no Git-backed document
history or recovery guarantee is implied.

## Synchronization and disclosure

Persistent files default to the separately configured external sync project.
[SYNCHRONIZED_STORAGE.md](SYNCHRONIZED_STORAGE.md) governs provider transmission,
availability, conflicts and backup; its repository-source convention is
overridden here for conversation QMD. Temporary processing stays device-local in
ignored repository temp/conversation-work/ and is never synchronized. Sync grants
no access, backup, sharing or publication.
University Whisper-v3 supplies input; transcription is outside the current scope.
No external service upload or participant sharing is authorized by initialization.
