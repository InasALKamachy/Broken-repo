# Task 1 Findings

## 1. Commit with mixed unrelated changes
- Commit: 2ee27fa ("quick fix")
- Issue: This commit modifies multiple unrelated files (README.md, config.txt, notes.txt). These changes should be split into separate logical commits.

## 2. Commit that introduced incorrect content
- Commit: 4a0530f ("refactor: Update todo list with progress")
- Issue: Added an incorrect line to todo.txt: "This line should not be here - it was added by mistake."

## 3. Commit containing sensitive information
- Commit: f6cd227 ("feat: Add configuration file")
- Issue: Added secrets.txt containing a hardcoded API key (API_KEY=sk_live_...).