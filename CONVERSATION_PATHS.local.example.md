# Local Conversation Paths

Copy to ignored CONVERSATION_PATHS.local.md. Concrete paths and conversation
metadata must never enter tracked files. This mapping is navigation only.

| Logical root | Directory on this host (resolve repository-relative paths locally) |
| --- | --- |
| conversation:root | Unset |
| conversation:temp | temp/conversation-work/ relative to this repository |

Relative persistent locations: input/, working/, sources/, output/docx/,
optional output/pdf/ and output/html/, review/, trace/.
The temporary root is device-local, outside any synchronized directory, and
ignored/untracked. Repository temp/conversation-work/ is the default.
Exact file selection and access/write authority must be established per task.
Follow [CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md). Other local repository
locations require deliberate mapping and verified Git exclusion, not fallback.
Do not infer access from a path being present.
