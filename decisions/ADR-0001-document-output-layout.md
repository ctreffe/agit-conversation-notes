# ADR-0001: Website and Document Output Layout

Status: Accepted
Date: 2026-11-08

## Context

The maintainer selected current Docs template methods and document folders for
existing as well as future outputs. Conversation storage must preserve PDR-0002's
permanent exclusion from Git and its exact selection/access boundaries.

## Decision

Keep the complete generic workflow site in output/website/. Keep all selected
formats of a conversation document in mapped output/<document-slug>/, with DOCX
first and PDF/HTML only when selected. Apply the rule to existing outputs only
through exact approved file moves, collision/hash checks and authorized updates
to private mappings/configuration/trace. Keep all concrete slugs, paths and
evidence unversioned. This record selects no conversation files or new storage.

Use --no-clean when rendering into shared output, or mapped isolated staging and
selected-artifact transfer. Preserve companion formats and unrelated files.
Keep sources, returned reviews, inputs and private traces in their existing roles.

## Rationale

Document folders keep companion formats together while preserving the coherent
website tree and separate storage/access models. PDR-0002 remains authoritative.

## Consequences

Generic guidance, render methods and the mapping example must agree. Concrete
host mappings and migration evidence stay private; workflow adoption does not
complete a conversation review, activate a profile or authorize publication.

## Alternatives considered

Format-root directories separate companion files. A single repository output
root would violate approved mappings. Automatic broad migration exceeds exact
file/action selection. Rerendering would broaden a path-only move into content QA.

## Follow-up

Check selected moves without changing bytes, update approved path references and
verify generic rendering/preservation independently. Retain pending domain review,
receiving-device and remote-sync evidence separately.
