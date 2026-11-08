---
name: manage-restricted-storage
description: Configure, confirm or roll back a project-local Codex profile for closed storage. Use only on deliberate invocation; project initialization is complete.
---

# Manage Restricted Storage

This skill owns protection design and qualification. Route every selected
config edit through [manage-codex-config](../manage-codex-config/SKILL.md).
Pass the approved profile delta and any pending configuration transaction;
reuse one original-state/recovery record and combine changes before restart.
Do not call start-project or create a second config writer. Preserve local
domain boundaries and the profile verification requirements below.

Apply AGENTS.md and the [input rules](../../../input/README.md). Use the
[profile procedure](references/codex-permissions.md) for an approved setup,
activation check or rollback. Confirm the exact project, scope and missing
action authority before a configuration change.

Resolve the standard denies from the known project root. Keep
`input/intake/`, `input/restricted/` and `temp/restricted/` closed to listing,
reading, processing and writing by Codex. Never inspect them to establish
coverage. Add external denies only for exact paths supplied and approved by
the maintainer. Keep the project’s readable working paths available.

Use the [existing input catalog](../../../input/CATALOG.md) for approved
source metadata and ignored `input/CATALOG.local.md` for approved sensitive
details. Update metadata only from maintainer reports. A catalog entry grants
no source access. Keep temporary files outside the catalog.

Keep maintained documentation and its document context authoritative.
A profile change grants no approval to render, include or publish screenshots,
logs or source excerpts.

Report saved configuration, post-restart active scope and rollback separately.
The short check confirms declared settings for ordinary local commands.
Refer concrete doubts about actual behavior to Governance.

## Required workflow usability

During selected profile setup, follow the
[usability procedure](references/profile-usability.md) for required project
operations and any bounded adapter. Keep protection and usability evidence
separate. Reuse current evidence; do not add checks to ordinary task entry.

## Initialized project boundary

Initialization is complete. Keep config and recovery files ignored and untracked.
Never recreate retired setup skills. Preserve the project source-access, rendering,
visual-inspection and publication gates; profile work grants none of those actions.
CONVERSATION_STORAGE.md overrides generic catalog/source rules for all actual or
fictional conversations. Resolve only exactly approved mappings and files; keep
all content, paths, metadata and processing permanently unversioned. Do not probe
conversation folders or infer access from a mapping or readable local directory.
