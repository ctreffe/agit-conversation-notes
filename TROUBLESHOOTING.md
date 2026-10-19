# Reusable Fixes

Search this repository's active cases and read only the matching entry.
Check current applicability; historical success is not device readiness.
A recorded fix grants no action or platform authority. Reuse only this
repository's records; never transfer lessons or maintain global memory.
Host-specific facts stay ignored in `TROUBLESHOOTING.local.md`; never store secrets or protected content.

## Compact entries

Use 4–8 nonblank source lines per case, including its stable KI heading:
**Recognize**, **Fix**, **Prevent or limit**. Keep necessary applicability
and authorization limits; dates and diagnostic detail are optional.
Add or update only useful prevention after recovery at the original operation.
Do not log every recurrence or require a detailed report.
Original evidence is preserved in [TROUBLESHOOTING_DETAILS.md](TROUBLESHOOTING_DETAILS.md).
Read only a matching detail section when the compact entry is insufficient;
the preserved historical schema is not the current workflow. Further detail is optional.

## KI-0001: Windows sandbox Git ownership check blocks a repository

- **Recognize:** Windows sandbox Git reports `detected dubious ownership`
  for an authorized repository; filesystem provisioning is a separate issue.
- **Fix:** With explicit persistent Git-trust approval, add only its exact path:
  `git config --global --add safe.directory <absolute-repository>`; verify normal `git status`.
- **Prevent or limit:** No wildcard/system trust or automatic derived-project trust.
  Source access, rendering, disclosure, publication and Git authority remain separate.
- [Evidence](TROUBLESHOOTING_DETAILS.md#ki-0001-windows-sandbox-git-ownership-check-blocks-a-repository)

## KI-0002: Skill validator lacks its YAML dependency

- **Recognize:** Skill validation stops with `No module named 'yaml'`.
- **Fix:** Use the managed Python environment and pinned `requirements-tools.txt`
  dependency via `scripts/Test-CodexSkill.ps1 -PythonPath <exact-interpreter>`.
- **Prevent or limit:** Check current interpreter readiness; a new clone has no transferred `.venv`.
  Environment creation, download and installation need authority; never change global Python.
- [Evidence](TROUBLESHOOTING_DETAILS.md#ki-0002-skill-validator-lacks-its-yaml-dependency)

## KI-0004: Context-sensitive patch application rejects a coordinated edit

- **Recognize:** `apply_patch` rejects expected context or malformed hunk lines.
- **Fix:** Read exact target spans and use the smallest stable semantic anchors.
  Preserve explicit line-level operation markers; inspect state after rejection.
- **Prevent or limit:** Do not retry the same patch; correct the mismatched hunk
  and prove uncertain patch shapes on a representative file within authorized scope.
- [Evidence](TROUBLESHOOTING_DETAILS.md#ki-0004-context-sensitive-patch-application-rejects-a-coordinated-edit)

## KI-0005: Default sandbox blocks an authorized Git metadata write

- **Recognize:** An authorized Git write meets the protected `.git` sandbox boundary.
- **Fix:** Once exact staging is requested or its commit authorized, request narrow
  platform escalation for that exact write on its first attempt; continue the original operation.
- **Prevent or limit:** Do not first provoke `.git/index.lock`; keep reads sandboxed.
  Never delete locks or change ACLs/trust to bypass this; action authority remains separate.
- [Evidence](TROUBLESHOOTING_DETAILS.md#ki-0005-default-sandbox-blocks-an-authorized-git-metadata-write)

## KI-0006: Windows sandbox temp blocks ensurepip during local venv setup

- **Recognize:** Approved clone-local venv creation stops in ensurepip with a
  PermissionError writing its bundled pip wheel to the platform temp directory.
- **Fix:** Reuse the partial clone venv; request narrow platform escalation for
  ensurepip and the already approved pinned dependency installation.
- **Prevent or limit:** No global Python/ACL/temp-policy changes; action and
  download authority remain separate. Verify the original skill-validation
  outcome with Test-CodexSkill.ps1, not merely successful package import.

## KI-0007: Windows sandbox blocks Quarto's local Deno project cache

- **Recognize:** An authorized render fails with PermissionDenied at Deno.openKv
  while initializing .quarto/project-cache inside the selected render project.
- **Fix:** Verify source/configuration, output, cache and temporary paths; request
  narrow platform escalation for the already authorized exact render command.
- **Prevent or limit:** Keep the project and TEMP/TMP/TMPDIR in mapped unversioned
  storage; no ACL/global-policy changes, installs or additional transmission.
