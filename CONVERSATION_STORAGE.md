# Conversation Storage and Access

This is the binding AGIT Conversation Notes exception to the inherited Docs
Template. See [PDR-0001](decisions/PDR-0001-external-conversation-files.md).

## Permanent boundary

All conversation files remain outside the Git working directory and permanently
unversioned: original Whisper JSON, prepared transcripts, authoritative QMD,
DOCX/PDF/HTML, returned review copies, attachments, extracts, logs, temporary
intermediates, source snapshots and revision evidence. This includes fictional
test conversations. Never copy conversation content into repository input,
materials, docs, temp, output, review, issues, commits, handoffs, Decision Records
or project documentation. Ignore rules are a fallback, not a storage location or
authorization. Do not create in-repository links/junctions to conversation folders.

The repository contains only skills, scripts, generic templates, configuration
and conversation-free project documentation. Repository docs/ is solely for
workflow documentation. Neither conversation sources nor accepted conversation
feedback may be promoted into repository documentation.

## Portable local mapping

Copy [CONVERSATION_PATHS.local.example.md](CONVERSATION_PATHS.local.example.md)
to ignored CONVERSATION_PATHS.local.md on each host. Map conversation:root
to an exact external project directory and conversation:temp to a device-local
external temporary directory. Both start as Unset. Keep concrete file paths,
provider details, participant metadata and conversation catalogs outside Git.
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
    <external-device-temp>/ # disposable processing, never synchronized

Before use, require exact maintainer-selected files and actions. Canonicalize
actual paths; ensure every conversation source, output, cache and intermediate
stays outside the repository, including through symlinks/junctions and inherited
Quarto configuration. Check local availability without scanning other folders.
An unset, conflicting or unavailable mapping stops dependent work; never fall
back to repository folders. Obtain outside-write authority before creating
folders or files. A non-sensitive classification is not blanket file access.
No real files are needed or approved for initialization.

## Source and revision trace

External QMD is authoritative despite having no Git history. Original transcripts
remain unchanged. Summaries organize content by topic, rather than reporting who
said what. Trace relevant claims to actual transcript segments/timestamps when
available. Do not invent identifiers, timestamps, speaker certainty,
responsibilities or dates. Mention people only where substantively needed, such
as a confirmed assignment; speaker labels remain fallible evidence. Distinguish
results, decisions, tasks, open questions and proposals. Mark uncertainty and
never present proposals as decisions.

Before DOCX review, retain a source snapshot or hash, source/output relationship
and review scope in external trace/. Keep feedback decisions and source-change
evidence there too. Reconcile a changed QMD against the export baseline before
applying feedback. Versioned project state records only generic workflow status,
never conversation IDs, excerpts, participant data or decisions.
Detailed trace format, protocol schema and drafting method are deferred to skill
design. Recovery/backup is a separate storage decision; no Git-backed document
history or recovery guarantee is implied.

## Synchronization and disclosure

Persistent files may later use separately configured sync storage.
[SYNCHRONIZED_STORAGE.md](SYNCHRONIZED_STORAGE.md) governs provider transmission,
availability, conflicts and backup; its repository-source convention is
overridden here for conversation QMD. Temporary processing stays external and
device-local. Sync grants no access, backup, sharing or publication.
University Whisper-v3 supplies input; transcription is outside the current scope.
No external service upload or participant sharing is authorized by initialization.
