### Repository Source of Truth

The user or other contributors may make changes to files between conversation turns or task runs.

If you encounter code that differs from a previous iteration, **you MUST NOT overwrite or undo** those human changes.  
Always treat the **current on-disk file contents** as the single source of truth.  
Do not rely on previous conversation history or cached code snapshots as authoritative.

Before starting a new task, always refresh your working copy:
git fetch --all --prune && git checkout main && git reset --hard origin/main && git clean -fdx
