# Screenshots and Visual Files

Screenshots are documentation files. They should be intentional, current, readable, and safe to publish.

## When to use screenshots

Use screenshots when they clarify:

- A concrete interface state.
- A configuration path.
- A workflow step.
- A visual result.
- A comparison or before-and-after state.

Do not use screenshots as decoration or as a substitute for explaining the important point in text.

## Privacy and sensitivity

Before the assistant reads, edits, or commits screenshots, confirm whether they contain:

- Personal data.
- Usernames, email addresses, or IDs.
- Internal URLs, hostnames, paths, tokens, or secrets.
- Customer, patient, student, employee, or ticket data.
- Operational details that should not be public.

Redact or recreate screenshots when needed.

## Capture rules

Project-specific rules should define:

- Browser, viewport, theme, and zoom level.
- Required UI state.
- Language and locale.
- Test data or demo data.
- Naming conventions.
- Storage location.

## Naming

Use stable, descriptive filenames. Include context rather than only dates.

Example:

```text
screenshots/admin-user-permissions-empty-state.png
screenshots/admin-user-permissions-configured.png
```

## Annotation

Annotations should improve clarity without hiding relevant UI. Keep them consistent and minimal.

## Review

Before publication, check that screenshots are current, readable, relevant, correctly referenced, and free of sensitive information.
