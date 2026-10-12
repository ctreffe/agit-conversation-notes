# PDR-0001: Keep all conversation files external and unversioned

Status: Accepted
Date: 2026-10-12

## Context

The inherited Docs Template versions maintained QMD and permits source/material
promotion. The maintainer requires every conversation-related file to remain
permanently outside Git, including authoritative document sources.

## Decision

Git contains only skills, scripts, generic templates, configuration and
conversation-free project documentation. All transcript JSON, derivatives,
QMD, outputs, review copies, traces and temporary conversation files remain
external and unversioned, including fictional trial files. External QMD remains
authoritative. Ignored local mappings contain actual locations; tracked contracts
use generic logical roots.

## Rationale

This maintains the content boundary while retaining a reusable workflow in Git.
Access classification cannot change the permanent versioning boundary.

## Consequences

Drafting, rendering and revision operate on authorized external files in place.
No conversation contents enter repository work areas or project records.
Private baselines and revision decisions stay external; Git provides no document
history. Sync, backup, scoped access, outside writes, transmission and sharing
are separate decisions.

## Alternatives considered

- Versioned QMD with ignored transcripts/outputs: violates the source boundary.
- Ignored conversation folders inside Git: violates external placement.
- External sync storage: permitted later, not configured or authorized here.

## Follow-up

Jointly design skill/schema, select exact external paths and permissions, test a
fictional DOCX round-trip and establish external backup/revision-trace details.
