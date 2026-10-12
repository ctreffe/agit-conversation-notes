# Local Conversation Paths

Copy to ignored CONVERSATION_PATHS.local.md. Concrete paths and conversation
metadata must never enter tracked files. This mapping is navigation only.

| Logical root | Absolute external directory on this host |
| --- | --- |
| conversation:root | Unset |
| conversation:temp | Unset |

Relative persistent locations: input/, working/, sources/, output/docx/,
optional output/pdf/ and output/html/, review/, trace/.
The temporary root is outside Git and outside any synchronized directory.
Exact file selection and access/write authority must be established per task.
Follow [CONVERSATION_STORAGE.md](CONVERSATION_STORAGE.md); never use repository
folders as fallback. Do not infer access from a path being present.
