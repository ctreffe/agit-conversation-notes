# PDR-0002: Keep conversation files unversioned and off GitHub

Status: Accepted
Date: 2026-10-13
Supersedes: [PDR-0001](PDR-0001-external-conversation-files.md)

## Context

The earlier storage contract interpreted the maintainer's boundary as requiring
every conversation file to reside outside the Git working directory. The
maintainer clarified that the requirement concerns exclusion from versioning
and GitHub. Ignored files may reside inside the project directory.

## Decision

All conversation files, including fictional fixtures, authoritative QMD, review
copies, traces, logs and intermediates, remain permanently unversioned and off
GitHub. Deliberately mapped ignored local repository locations are permitted.
Persistent files default to the external synchronized project; temporary files
use ignored device-local temp/conversation-work/ and are never synchronized.
The selected unversioned QMD remains authoritative wherever stored.

## Rationale

This preserves the intended versioning/publication boundary while allowing the
established repository temp convention without unnecessary external directories.

## Consequences

Drafting, rendering and revision verify actual paths, ignore coverage and the
absence of tracked conversation files for in-repository processing locations.
Never force-add conversation files or put concrete contents into versioned
documentation, catalogs, handoffs or decisions. Generic templates remain generic.
Host mappings remain ignored. Access, outside writes, synchronization, backup,
sharing and publication retain their separate scopes; no Git write is authorized.

## Alternatives considered

- Require all files outside the repository: exceeds the clarified requirement.
- Version conversation QMD: violates the permanent versioning boundary.
- Synchronize temporary processing: conflicts with the device-local convention.

## Follow-up

Align project descriptions, resident rules, draft/render/revision skills and
local mappings. Verify ignored temp placement before the first conversation trial.
