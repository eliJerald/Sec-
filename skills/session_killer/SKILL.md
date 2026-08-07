---
name: session-killer
description: Automatically generates a session summary report of all changes and activities performed in the current session and appends it to the summaries.md file.
---

# Session Killer Skill

When the user asks you to execute the `session-killer` skill, run the `session-killer` command, or simply summarize the session, you must perform the following actions:

1. **Review Session History:** Look back over the current conversation and summarize all tasks, file updates, topics discussed, and practice questions answered.
2. **Format the Summary:** You MUST strictly follow the existing format found in the `/mnt/c/Users/ejera/projects/sec+/Sec-/summaries.md` file. The summary must include:
   - A date header formatted as: `### Session Date: YYYY-MM-DD HH:MM:SS TZ` (using the current local time).
   - A `#### Session Summary Report` header.
   - Numbered main topics (e.g., `**1. CompTIA Security+ SY0-701 Tutoring**`) with bulleted sub-topics describing the exact actions taken.
   - A `#### Next Steps & Future Work` section with bulleted action items for the user's next study session.
   - An exact 80-character divider line at the very end of the entry:
     `--------------------------------------------------------------------------------`
3. **Append to Log:** Append this generated summary report to the `/mnt/c/Users/ejera/projects/sec+/Sec-/summaries.md` file. Do not overwrite the file. Use a Python script to reliably append the text.
4. **Commit to Git (Optional):** If the user has requested it previously, you may also commit these changes to version control, but the primary task is updating the `summaries.md` file.
5. **Notify User:** Inform the user that the session summary has been successfully generated and logged.
