# Feedback Workflow

## Authoritative source and storage

External conversation QMD remains authoritative despite being unversioned.
Rendered formats and annotations are review evidence. All review files, extracts,
baseline snapshots and decisions stay external; repository review/, output/ and
temp/ are never conversation storage. Follow
[CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md).
Repository-documentation feedback concerns only conversation-free workflow rules.

## Review cycle

1. Select exact source/review file, scope, external destinations and permitted
   actions. Mapping/non-sensitive classification alone grants no access or writes.
2. Render externally; retain the QMD snapshot/hash and output relationship in
   external trace/. Git commit IDs do not identify an external source baseline.
3. Keep returned copies unchanged in external review/. Identify reviewer and
   reconcile changes since export before incorporation.
4. Extract comments/Track Changes locally into external temporary storage.
   Never put conversation extracts or decisions into repository records/logs.
5. Clear maintainer instructions may be applied when intent/source is unambiguous.
   Uncurated external feedback needs acceptance, rejection, qualification or
   deferral; a Maintainer: comment may curate it. Clarify ambiguous evidence.
6. Apply accepted changes to external QMD with external source mapping and
   revision evidence; do not replace QMD with the edited DOCX export.
7. Re-render and technically verify changes; record unresolved/rejected/deferred
   items externally. Repository status reports generic workflow progress only.

Direct source comments remain possible. Optional PDF annotations require careful
source mapping. Visual inspection remains separately explicit.
Access, sharing, transmission and publication are separate decisions.
Conversation review files are permanently excluded from Git without exceptions.
