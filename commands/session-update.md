Update the current development session by:

1. Check if `.claude/sessions/.current-session` exists to find the active session
2. If no active session, inform user to start one with `/project:session-start`
3. If session exists, append to the session file with:
   - Current timestamp
   - The update: $ARGUMENTS (or if no arguments, summarize recent activities)
   - Todo list status:
     * Number of completed/in-progress/pending tasks
     * List any newly completed tasks
   - Clarifying and exploratory questions asked
   - Responses and tradeoffs related to questions
   - Decisions made with any reasoning if provided
   - Any issues encountered
   - Solutions implemented
   - Code changes made

Keep updates concise but comprehensive for future reference.

Example format:
```
### Update - 2025-06-16 12:15 PM

**Summary**: Implemented user authentication

**Todo Progress**: 3 completed, 1 in progress, 2 pending
- ✓ Completed: Set up auth middleware
- ✓ Completed: Create login page
- ✓ Completed: Add logout functionality

**Details**: [user's update or automatic summary]
```
