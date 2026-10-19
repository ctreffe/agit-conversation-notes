# Temporary Working Files

`temp/` contains disposable intermediate documentation files. All contents
outside `restricted/` are assistant-readable. Everything under `temp/` is
local-only, ignored by Git and must never be versioned.

Use `restricted/` for temporary files that assistants must not enumerate or
read. Temporary files are not cataloged. Move a durable file to `materials/`
and catalog it before any later promotion to maintained documentation.

## Conversation workflow

Use ignored device-local temp/conversation-work/ for authorized conversation
intermediates, logs and extracts. Never version or synchronize these files.
The generic promotion/catalog instruction above does not apply to conversation
content: retained files stay unversioned in the selected persistent location,
external sync storage by default. Follow CONVERSATION_STORAGE.md and the ignored
local path mapping. Do not put conversation content into this versioned README.
