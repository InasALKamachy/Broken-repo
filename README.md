# Task 1 — Inspect the Repository I used Git history commands to find problems such as:

A commit with unrelated changes

Incorrect content added in a commit

A leaked API key

I documented these findings in TASK1_FINDINGS.md.

# Task 2 — Clean Up Commit History I used interactive rebase to split a commit that mixed multiple changes. Each logical change became its own commit to keep the history clean.

# Task 3 — Fix Incorrect Content I corrected the wrong content in todo.txt using a normal commit (no history rewriting), which is the safest approach on shared branches.

# Task 4 — Resolve Merge Conflicts Merging feature/login into main caused conflicts in:

notes.txt

README.md

I resolved them manually and completed the merge.

# Task 5 — Remove Leaked Secrets I removed the hardcoded API key from secrets.txt and committed the fix.

In a real project, I would also:

Revoke the leaked key

Generate a new one

Remove the secret from Git history

Add the file to .gitignore

# Task 6 — Rebase and Sync Branches I rebased feature/login on top of main and resolved the conflicts. The branch now has a clean, linear history.

# Task 7 — Recover Lost Commit (Bonus) I checked git reflog to look for dropped commits. No commits were actually lost, but I explained how I would recover one using:

- git checkout -b

- or git cherry-pick